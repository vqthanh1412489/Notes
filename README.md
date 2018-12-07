# Notes

# Push heroku Nodejs
- Xóa tất cả các dòng code dứ thừa phát sinh phục vụ quá trình dev (vd: reload, test...)
- Sửa trong file package.json
  "scripts": { "start": "node index"  }
- Sửa trong  app.listen(process.env.PORT || 3009 , () => console.log('Server Started')); 
# Plugin VS Code
- Auto remane tag
- Auto close tag
- HTML Snippets
- HTML-LESS-Class Complition
- Node.js Modules Intellisense
- npm Intellisense
- Path Intellisense
- Angular 4 and Typescript/HTML VS..
- Angular language service
- Angular v5 Snippets
- angular2 - switcher
- icon-vscode
- Prettier - Code formater (Esben Petersen): Crtl + Shift + I

# Plugin Sublime Text
 - Emmet
- AutoFileName
- SideBarEnhancements
- Advanced New File (ctrl + alt + n)
- Color HighLighter
- Color Picker (Ctrl +shift + C)
- Sublime CodeIntel

# NODEJS TIP
  1. Create new folder:
  - Module: mkdirp
      mkdirp(‘’/public/jpg’);
# Vietnamese
à','á','ạ','ả','ã','â','ầ','ấ','ậ','ẩ','ẫ','ă','ằ','ắ','ặ','ẳ','ẵ','è','é','ẹ','ẻ','ẽ','ê','ề','ế','ệ','ể','ễ','ì','í','ị','ỉ','ĩ','ò','ó','ọ','ỏ','õ','ô','ồ','ố','ộ','ổ','ỗ','ơ','ờ','ớ','ợ','ở','ỡ','ù','ú','ụ','ủ','ũ','ư','ừ','ứ','ự','ử','ữ','ỳ','ý','ỵ','ỷ','ỹ','đ','À','Á','Ạ','Ả','Ã','Â','Ầ','Ấ','Ậ','Ẩ','Ẫ','Ă','Ằ','Ắ','Ặ','Ẳ','Ẵ','È','É','Ẹ','Ẻ','Ẽ','Ê','Ề','Ế','Ệ','Ể','Ễ','Ì','Í','Ị','Ỉ','Ĩ','Ò','Ó','Ọ','Ỏ','Õ','Ô','Ồ','Ố','Ộ','Ổ','Ỗ','Ơ','Ờ','Ớ','Ợ','Ở','Ỡ','Ù','Ú','Ụ','Ủ','Ũ','Ư','Ừ','Ứ','Ự','Ử','Ữ','Ỳ','Ý','Ỵ','Ỷ','Ỹ','Đ

# MySQL
Khi mới cài đặt kết nối với MySQL có lỗi: 
Client does not support authentication protocol.....
Vô MySQL chạy lệnh sau:
ALTER USER 'root'@'localhost' IDENTIFIED WITH mysql_native_password BY 'sinhvien1T'
