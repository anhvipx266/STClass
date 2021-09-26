STClass\
STClass.Meta\

STClass.Meta.Func\
**rawindex(self,k)**\
Trả về thông qua rawget() áp dụng cho từ khóa có "\_" ở đầu\
**get(self,k)**\
Trả về bằng tham chiếu đến \_property nếu nó là một table cơ bản thì trả về TableClass tương ứng\
**insget(self,k)**\
Trả về thuộc tính của self.\_ins[k] nếu có.\
**index(self,k,...[string])**\
Tham chiếu đến theo thứ tự các hàm Meta.\

**rawnewindex(self,k,v)** \
Set key: \_\<key>\
**readonly(self,k)** \
Lỗi tham chiếu\
**rawfunc(self,k,func**) \
Tạo tham chiếu thô hàm\
**set(self,k,v)** 
Thông qua \_property, Fire event lên đối tượng cao nhất.\
**insset(self,k,v)**\
Set self.\_ins[k]=v nếu có\
**newindex(self,k,v,...[string])** \
Tham chiếu theo thứ tự các hàm Meta\

**readServer(self,k)** \
Lỗi tham chiếu Client\
**readClient(self,k)** \
Lỗi tham chiếu Server\
  
STClass.Meta.Var\
