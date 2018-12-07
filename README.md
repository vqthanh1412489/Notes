## Notes

## Push heroku Nodejs
- Xóa tất cả các dòng code dứ thừa phát sinh phục vụ quá trình dev (vd: reload, test...)
- Sửa trong file package.json
  "scripts": { "start": "node index"  }
- Sửa trong  app.listen(process.env.PORT || 3009 , () => console.log('Server Started')); 
## Plugin VS Code
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

## Plugin Sublime Text
- Emmet
- AutoFileName
- SideBarEnhancements
- Advanced New File (ctrl + alt + n)
- Color HighLighter
- Color Picker (Ctrl +shift + C)
- Sublime CodeIntel

## NODEJS TIP
  1. Create new folder:
  - Module: mkdirp
      mkdirp(‘’/public/jpg’);
## Vietnamese
```à','á','ạ','ả','ã','â','ầ','ấ','ậ','ẩ','ẫ','ă','ằ','ắ','ặ','ẳ','ẵ','è','é','ẹ','ẻ','ẽ','ê','ề','ế','ệ','ể','ễ','ì','í','ị','ỉ','ĩ','ò','ó','ọ','ỏ','õ','ô','ồ','ố','ộ','ổ','ỗ','ơ','ờ','ớ','ợ','ở','ỡ','ù','ú','ụ','ủ','ũ','ư','ừ','ứ','ự','ử','ữ','ỳ','ý','ỵ','ỷ','ỹ','đ','À','Á','Ạ','Ả','Ã','Â','Ầ','Ấ','Ậ','Ẩ','Ẫ','Ă','Ằ','Ắ','Ặ','Ẳ','Ẵ','È','É','Ẹ','Ẻ','Ẽ','Ê','Ề','Ế','Ệ','Ể','Ễ','Ì','Í','Ị','Ỉ','Ĩ','Ò','Ó','Ọ','Ỏ','Õ','Ô','Ồ','Ố','Ộ','Ổ','Ỗ','Ơ','Ờ','Ớ','Ợ','Ở','Ỡ','Ù','Ú','Ụ','Ủ','Ũ','Ư','Ừ','Ứ','Ự','Ử','Ữ','Ỳ','Ý','Ỵ','Ỷ','Ỹ','Đ```

## MySQL
Khi mới cài đặt kết nối với MySQL có lỗi: 
Client does not support authentication protocol.....
Vô MySQL chạy lệnh sau:
ALTER USER 'root'@'localhost' IDENTIFIED WITH mysql_native_password BY 'sinhvien1T'

## JavaScript - TypeScript
1. Different between: CONST - LET - VAR
VAR: Tạo biến có giá trị trong 1 Function. Không tạo ra thuộc tính mới cho THIS
LET: Tạo biến có giá trị trong 1 Block. Không tạo ra thuộc tính mới cho THIS
CONST: Tạo hằng.
2.  Các giá trị đặc biệt:
False
Null: Giá trị rỗng. Khi thực hiện các Operator thì coi như là 0
Undifined
0
Infinity: Số vô cùng (Vd: Chia cho 0...)
NaN (Not a number): Không phải số (Vd: undifined/ 2, null / null ...)
3.  Console.log(typeof null) => object ??????
4. Tham trị và Tham biến
Tham trị: gồm những giá trị mang kiểu String, Number, Boolean, Null, Undifine. 
Tham biến: Những giá trị kiểu Object.
5.  Array
.push(‘Thanh’): Thêm vào cuối mảng. Làm thay đổi. Output: New length của mảng
.pop(): Xóa phần tử cuối. Làm thay đổi. Output:  Phần tử bị xóa.
.shift(): Xóa phần tử đầu của mảng. Làm thay đổi. Output: Phần tử bị xóa
.unshift(‘Thanh’): Thêm phân tử vào đẩu mảng. Làm thay đổi. Output:n New length của mảng.
.splice(indexStart, countDelete, itemAdd...). Làm thay đổi. Output: Phần tử bị xóa. Nếu không xóa, chỉ thêm thì return [];
Array.isArray(arrNumber): Check có phải là array hay k? hoặc có thể dùng:
 function isArray(x) {
return x.constructor.toString().indexOf(“Array”) > -1;
};
fruits instanceof Array     // trả về kết quả true
6. String
7.  Khởi tạo file init ts và biên dịch code qua js.
tsc --init: auto chay
tsc -w: theo doi thay doi

## Ubuntu
<img src="https://imgur.com/a/27ALp4j">
```sh
sudo apt-get autoremove
```

```sh sudo apt-get clean
sudo apt-get autoclean
```

```sh 
du -sh ~/.cache/thumbnails
rm -rf ~/.cache/thumbnails/*
```

```sh 
sudo dpkg --list 'linux-image*'
sudo apt-get remove linux-image-VERSION // add version 
```

Minimiza windows
```sh 
gsettings set org.gnome.shell.extensions.dash-to-dock click-action 'minimize'
```

Install Nodejs & npm
```sh 
sudo apt install nodejs
sudo apt install npm
```

Install Yarn
```sh
curl -sS https://dl.yarnpkg.com/debian/pubkey.gpg | sudo apt-key add -
$ echo "deb https://dl.yarnpkg.com/debian/ stable main" | sudo tee /etc/apt/sources.list.d/yarn.list
sudo apt-get update && sudo apt-get install --no-install-recommends yarn
```


Install nodemon
```sh 
sudo npm install -g nodemon
```

Install mongodb
```sh
sudo apt install -y mongodb
```

Managing the Service
```sh 
sudo systemctl status mongodb
sudo systemctl stop mongodb
sudo systemctl start mongodb
sudo systemctl restart mongodb

service --status-all
systemctl disable mongodb
systemctl enable mongodb
```

Save ssh-key githup
```sh
git config credential.helper store
```


Classic menu
```sh
sudo apt-add-repository ppa:diesch/testing
sudo apt-get update
sudo apt-get install classicmenu-indicator
```


