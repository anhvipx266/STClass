1. STClass:Folder->Module
1. Tạo bảng cơ sở bao gồm func, var
1. Cấu trúc Meta sử dụng cho các lớp.
1. Meta\
1.1. Func\
1.1.1. index method\
rawindex(self,k) trả về thông qua rawget() áp dụng cho từ khóa có "_" ở đầu\
1.1.1. newindex method
rawnewindex(self,k,v) set key: _<key>\
readonly(self,k) lỗi tham chiếu\
1.1.1. index/newindex method
readServer(self,k) lỗi tham chiếu Client\
readClient(self,k) lỗi tham chiếu Server\
  
1.1  Var
  

1. Chuyển đổi cách index của các lớp từ key:lower()-> bảng _property.( Sử dụng Meta ở trên)
1. Add func: Run(string|table) để chạy các lớp STClass(sử dụng bởi một script ở cả 2 phía)
