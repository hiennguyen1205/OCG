Họ và tên: Nguyễn Quang Hiển

BACKEND
	Code backend nằm trong thư mục backend
	Chạy code backend trên cổng http://localhost:3000/
	Cấu trúc
		```
.
├── config  <-- Đọc cấu hình sử dụng Viper
│   └── config.go
├── controller <-- Các controller xử lý request đến
│   ├── ManufactureController.go
│   └── ProductController.go
├── model <-- Định nghĩa các model
│   ├── Category.go
│   ├── Country.go
│   ├── Manufacturer.go
│   └── Product.go
├── repo <-- Lưu các phương thức xử lý dữ liệu chuyên cho từng Model
│   ├── CategoryRepo.go
│   ├── CountryRepo.go
│   ├── ManufactureRepo.go
│   ├── ProductRepo.go
│   └── Repo.go  <-- Lưu biến toàn cục Database Connection `var Db *gorm.DB`
├── routes <-- Cấu hình định tuyến các request đến ứng với phương thức của Controller`
│   └── ConfigRouter.go
├── sql <-- Lưu các file SQL script tạo bảng và xoá bảng
│   ├── DropTable.sql  <-- Tạo cấu trúc bảng
│   └── OnlineShop.sql <-- Drop các bảng
├── app.go <-- File chạy chính
├── dev.yml <-- File cấu hình ở môi trường development
├── go.mod
├── go.sum
├── GORM.md
└── ReadMe.md <-- File này quan trọng nhất, làm gì thì làm, luôn phải viết document!
```
	
FRONTEND
	Code frontend nằm trong thư mục frontend
	Code frontend chạy trên cổng 8080
	Cấu trúc
	```
.
├── public  <-- Chứa file index.html cho cả trang web
│   └── index.html
├── src <-- chứa code chính của dự án
│   ├── assets <-- chứa ảnh và file css
│   └── component <-- chứa các component con
│   ├── pages <--- chứa các trang view 
│   ├── router <--chứa file cấu hình router
│   └── store <-- sử dụng và cấu hình vuex
├── App.vue 
│   
├── main.js
```
	