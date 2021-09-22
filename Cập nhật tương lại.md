 STClass:Folder->Module
 Tạo bảng cơ sở bao gồm func, var
 Cấu trúc Meta sử dụng cho các lớp.
Meta = {
  Func={
    -- index method
    rawindex(self,k) trả về thông qua rawget() áp dụng cho từ khóa có "_" ở đầu
    -- newindex method
    rawnewindex(self,k,v) set key: _<key>
    readonly(self,k) lỗi tham chiếu
    --index/newindex method
    readServer(self,k) lỗi tham chiếu Client
    readClient(self,k) lỗi tham chiếu Server
  },
  Var={
    ...
  }
}
 Chuyển đổi cách index của các lớp từ key:lower()-> bảng _property.( Sử dụng Meta ở trên)
 Add func: Run(string|table) để chạy các lớp STClass(sử dụng bởi một script ở cả 2 phía)
