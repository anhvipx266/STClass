# STClass
Tập hợp module cho Roblox!

Trong đó có tập hợp cao cấp gồm các đối tượng cao cấp nhất mà từ đó có thể thực hiện tất cả mọi thứ!
Đối tượng cao cấp không là hậu duệ của TableClass.
Ngoài ra còn có một số tiện ích khác sẽ được chạy và try xuất thông qua getUtility(name) [lấy tiện ích] hoặc thô bằng require()\
## Tập hợp Cao Cấp
*Nếu có Folder STFolder trong ReplicatedStorage hoặc ServerStorageScript thì các lớp cao cấp bên trong sẽ được chạy. 
- Control: Cung cấp điều khiển để kiểm soát tại một phía.
- Service: Cung cấp dịch vụ, sự kiện cho Ser-Cli
- System: Cung cấp hệ thống, có thêm khả năng gọi hàm so với Service
- Store: Cung cấp kho lưu trữ cho Ser, chỉ đọc ở Cli
- Replicate: Tương tự Store nhưng được tạo riêng cho mỗi plr
- MInstance: Tương tự như Instance nhưng được tham chiếu bằng require()
## Tiện ích(Utility)
- Cloner: Dùng để nhân bản
- Signal: Sử dụng để tạo sự kiện
- TableClass: Thay thế cho table để đạt được các sự kiện thay đổi.
- ResultDetect: Kiểm soát, điều hướng kết quả, chẳng hạn: Thắng thua một trận đấu
- RemoveDetect: Sự kiện Remove cho đối tượng có Parent
- RemoteSignal: Tạo sự kiện giữa khách-chủ.
