> ***Ghi chú***
- Có hai dạng dữ liệu:
- - Cục bộ(Local): chỉ được tạo ở máy khách hoặc máy chủ.
- - Toàn cục(Global): được tạo ở cả máy khách và máy chủ, đồng thời tuân theo mô hình sao chép Máy chủ -> Máy khách.
> Các khóa đặc biệt:[]
- **Local**: được sử dụng cục bộ
- **Global**: được sử dụng toàn cục
- **InMeta**: chỉ hoạt động khi có trong Meta, tức là trước khi trở thành một lớp cao cấp.
- **Server**: được sử dụng ở máy chủ.
- **Client**: được sử dụng ở máy khách.
> ***Tham chiếu***
## Property
- `[Local]` table **\_property**: chứa các thuộc tính
- `[Local]` table **\_table**: chứa TableClass là bản sao trỏ đến 1 table trong **\_property**
- `[Local]` table **\_readonly**: chứa các khóa dạng `table[k] = true` nếu tồn tại k khi thay đổi giá trị thì sẽ có thông báo lỗi
- `[Local]` table **\_readServer**: chứa các khóa dạng `table[k] = true` nếu tồn tại k khi tham chiếu hoặc thay đổi giá trị ở máy khách thì sẽ có thông báo lỗi
- `[Local]` table **\_readClient**: chứa các khóa dạng `table[k] = true` nếu tồn tại k khi tham chiếu hoặc thay đổi giá trị ở máy khách thì sẽ có thông báo lỗi
- `[Local]` any **any**: tham chiếu đến một khóa bất kì trong **\_property**
## Method
- `[Local]` void **Start()**: nếu tồn tại nó sẽ được gọi ngay sau setmetatable và không làm gián đoạn tập lệnh
- `[Local] [Client]` void **StartClient()**: nếu tồn tại nó sẽ được gọi ngay sau *Start()* ở máy khách và không làm gián đoạn tập lệnh
- `[Local] [Server]` void **StartServer()**: nếu tồn tại nó sẽ được gọi ngay sau *Start()* ở máy chủ và không làm gián đoạn tập lệnh
- `[Local] [Client]` void **Init(chr:Character)**: nếu tồn tại nó sẽ được gọi khi nhân vật được thêm (CharacterAdded)
- `[InMeta] [Global]` any **[Server]any**: tạo một chức năng được gọi ở máy chủ với khóa **any**
- `[InMeta] [Global]` any **[Client]any**: tạo một chức năng được gọi ở máy khách với khóa **any**
