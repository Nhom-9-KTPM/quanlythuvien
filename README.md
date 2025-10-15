📚 LIBMAN - Hệ Thống Quản Lý Thư Viện Hiện Đại
<!-- Badges: Thêm các biểu tượng công nghệ và trạng thái dự án tại đây -->

🚀 1. Giới Thiệu Dự Án
LIBMAN (Library Manager) là ứng dụng web quản lý thư viện số hóa, được xây dựng theo kiến trúc Client-Server. Mục tiêu là tối ưu hóa các quy trình nghiệp vụ như Quản lý Sách, Quản lý Độc giả, và xử lý giao dịch Mượn/Trả, giúp Thủ thư làm việc hiệu quả và cung cấp trải nghiệm tốt nhất cho Độc giả.

Vấn đề giải quyết
Số hóa quy trình mượn/trả, tránh sai sót thủ công.

Cung cấp giao diện trực quan cho Thủ thư để theo dõi sách tồn kho và các giao dịch trễ hạn.

Giúp Độc giả dễ dàng tìm kiếm và kiểm tra tình trạng sách.

📸 2. Giao Diện (Minh Họa)
[Chèn ảnh hoặc GIF động minh họa màn hình Dashboard chính của dự án]

💡 3. Chức Năng Chính
Dự án phân chia chức năng theo ba vai trò chính: Độc giả, Thủ thư và Quản trị viên.

👤 Chức Năng dành cho Độc giả
Tìm kiếm & Lọc: Tìm kiếm sách theo Tên, Tác giả, ISBN, Thể loại.

Xem Chi tiết Sách: Thông tin mô tả, năm xuất bản và tình trạng tồn kho (Available/Total).

Lịch sử Mượn: Xem danh sách sách đang mượn và đã trả, bao gồm Hạn trả dự kiến.

🛠️ Chức Năng dành cho Thủ thư / Quản trị viên
Chức năng

Mô tả

Chi tiết kỹ thuật

Quản lý Sách

CRUD sách. Cập nhật Số lượng tồn và Số lượng có sẵn.

Gửi request POST/PUT/DELETE đến endpoint /api/book.

Quản lý Độc giả

Quản lý hồ sơ độc giả, khóa/mở khóa tài khoản.

Liên kết thông tin độc giả với user_id.

Xử lý Mượn/Trả

Xác nhận giao dịch, tự động cập nhật tồn kho.

Cập nhật bảng transactions và trường available_quantity trong bảng books.

Dashboard

Báo cáo trực quan

Sử dụng biểu đồ để hiển thị Top sách mượn và thống kê thể loại.

⚙️ 4. Công Nghệ Sử Dụng
Dự án được xây dựng trên kiến trúc Client-Server.

Thành phần

Công nghệ

Phiên bản

Backend Logic

PHP

>= 7.4

Database

MySQL



Frontend

HTML5, CSS3



Styling

Tailwind CSS

(Nếu có)

Giao tiếp

JavaScript (Fetch API)



🗂️ 5. Cấu Trúc Thư Mục
Cấu trúc dự án được tổ chức theo mô hình MVC (Model-View-Controller) kết hợp với RESTful API endpoints:

QuanLyThuVien_LIBMAN-main/
└── libman/
    ├── backend/              # Chứa các API endpoints
    │   ├── book/             # API CRUD Sách
    │   ├── reader/           # API CRUD Độc giả
    │   └── user/             # API Đăng ký, Đăng nhập
    ├── models/               # Chứa các Class PHP (Book.php, User.php, ...)
    ├── config/               # db_connect.php
    ├── assets/               # js/, css/
    ├── page/                 # login.html, dashboard.html
    └── sql/                  # create_database.sql

🚀 6. Hướng Dẫn Cài Đặt (Local)
Để chạy dự án, bạn cần môi trường XAMPP/WAMP và thực hiện các bước sau:

Clone Repository: Tải dự án về máy:

git clone [Link-Repository-Của-Bạn]

Thiết lập Môi trường:

Sao chép thư mục libman vào thư mục htdocs của XAMPP.

Khởi động Apache và MySQL.

Thiết lập Database:

Truy cập http://localhost/phpmyadmin/.

Tạo database mới tên là libman.

Import file libman/sql/create_database.sql vào database vừa tạo.

Chạy Ứng dụng:

Mở trình duyệt và truy cập: http://localhost/libman/page/login.html

🤝 7. Thành Viên Nhóm & Liên Hệ
Dự án được thực hiện bởi:

👨‍💻 Phạm Lê Đình An - [Link GitHub]

👨‍💻 Hà Lê Quang Minh - [Link GitHub]

👨‍💻 Nguyễn Duy Anh Tuấn - [Link GitHub]

👨‍💻 Nguyễn Đức Tuấn - [Link GitHub]

📧 Email Liên hệ chung: nhom99@gmail.com
