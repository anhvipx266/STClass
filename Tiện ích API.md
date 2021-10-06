## Signal 
### function
**Signal new()**: contructor\
**boolean is(any)**: kiểm trả xem nó có phải là Signal không!\
### method
**void Connect(func, boolean run, ...:para)**: kết nối với một chức năng, gọi và truyền vào tham số nếu run là `true`\
**void Connects(funcs[func],boolean run,...:para)**: tương tự `Connect` nhưng áp dụng cho một mảng chức năng.\
**void Disconnect(func)**: gắt kết nối đến một chức năng.\
**void Disconnects()**: gắt kết nối tất cả các chức năng.\
**void Fire(...)**: kích hoạt sự kiện với các tham số.\
**... Wait()**: đợi đến khi sự kiện được kích hoạt và trả về tương ứng với tham số `Fire`
## RemoteSignal:Signal
