## Control
### Property
table **\_property**: chứa các thuộc tính\
table **\_table**: chứa TableClass là bản sao trỏ đến 1 table trong **\_property**\
table **\_readonly**: chứa các khóa dạng `table[k] = true` nếu tồn tại k khi thay đổi giá trị thì sẽ có thông báo lỗi\ 
### Method
void **Start()**: nếu tồn tại nó sẽ được gọi ngay sau setmetatable và không làm gián đoạn tập lệnh\
[Client] void **Init(chr:Character)**: nếu tồn tại nó sẽ được gọi khi nhân vật được thêm (CharacterAdded)\
------------------------------------------------
## Service
### Property
table **\_property**: chứa các thuộc tính\
table **\_table**: chứa TableClass là bản sao trỏ đến 1 table trong **\_property**\
table **\_readonly**: chứa các khóa dạng `table[k] = true` nếu tồn tại k khi thay đổi giá trị thì sẽ có thông báo lỗi\ 
table **\_readServer**: chứa các khóa dạng `table[k] = true` nếu tồn tại k khi tham chiếu hoặc thay đổi giá trị ở máy khách thì sẽ có thông báo lỗi\ 
table **\_readClient**: chứa các khóa dạng `table[k] = true` nếu tồn tại k khi tham chiếu hoặc thay đổi giá trị ở máy khách thì sẽ có thông báo lỗi\ 
### Method
void **Start()**: nếu tồn tại nó sẽ được gọi ngay sau setmetatable và không làm gián đoạn tập lệnh\
[Client] void **StartClient()**: nếu tồn tại nó sẽ được gọi ngay sau *Start()* ở máy khách và không làm gián đoạn tập lệnh\
[Server] void **StartServer()**: nếu tồn tại nó sẽ được gọi ngay sau *Start()* ở máy chủ và không làm gián đoạn tập lệnh\
