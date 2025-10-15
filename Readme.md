Hệ thống Quản lý Thư viện
Đây là một dự án web quản lý thư viện đơn giản, được xây dựng bằng PHP thuần ở phía backend và HTML, CSS, JavaScript (Vanilla JS) ở phía frontend. Dự án áp dụng mô hình API RESTful để giao tiếp giữa frontend và backend.

✨ Các chức năng chính
Dự án phân chia rõ ràng hai luồng chức năng cho Quản trị viên (Admin/Thủ thư) và người dùng thông thường (Độc giả).

👨‍💼 Dành cho Quản trị viên (Admin)
Quản lý Sách: Thêm, sửa, xóa sách trong thư viện.

Quản lý Độc giả: Thêm, sửa, xóa thông tin độc giả.

Quản lý Mượn/Trả:

Tạo phiếu mượn sách mới cho độc giả.

Cập nhật trạng thái của một giao dịch (BORROWED, OVERDUE, RETURNED).

Tìm kiếm: Tìm kiếm sách nhanh chóng theo tên hoặc tác giả.

📖 Dành cho Độc giả (Reader)
Xác thực: Đăng ký, đăng nhập, đăng xuất.

Xem & Tìm kiếm sách: Xem danh sách tất cả sách có trong thư viện và tìm kiếm theo tên hoặc tác giả.

Mượn sách: Gửi yêu cầu mượn một quyển sách còn trong kho.

Lịch sử cá nhân: Xem lại lịch sử các sách đã và đang mượn.

💻 Công nghệ sử dụng
Backend: PHP 8+ (không sử dụng framework)

Frontend: HTML5, CSS3, JavaScript (ES6+, Vanilla JS)

Cơ sở dữ liệu: MySQL / MariaDB

Web Server: Apache (thông qua XAMPP)

📁 Cấu trúc thư mục
Dự án được tổ chức theo cấu trúc rõ ràng, tách biệt logic:

/quanlythuvien
├── backend/            # Chứa các file API endpoints
│   ├── book/
│   ├── reader/
│   ├── transaction/
│   └── user/
├── config/             # Chứa file kết nối CSDL
│   └── db_connect.php
├── models/             # Chứa các class xử lý logic 
│   ├── Book.php
│   ├── Reader.php
│   └── Transaction.php
├── js/                 # Chứa các file JavaScript cho frontend
│   ├── dashboard.js    # Logic cho trang admin
│   ├── login.js
│   └── user_dashboard.js # Logic cho trang độc giả
│
├── create_database.sql # File kịch bản khởi tạo CSDL
├── dashboard.html      # Giao diện trang admin
├── user_dashboard.html # Giao diện trang độc giả
└── Readme.md           # File hướng dẫn và giới thiệu dự án

🚀 Hướng dẫn Cài đặt & Chạy dự án
Để chạy dự án này trên máy cục bộ, bạn cần có XAMPP được cài đặt.

1. Sao chép Project:

Clone repository này về máy:

git clone [https://github.com/thanhtohieu/quanlythuvien]

Hoặc tải về và giải nén vào thư mục C:\xampp\htdocs\quanlythuvien.

2. Khởi tạo Cơ sở dữ liệu:

Khởi động Apache và MySQL trong XAMPP Control Panel.

Truy cập http://localhost/phpmyadmin.

Tạo một cơ sở dữ liệu mới với tên là library.

Chọn CSDL library vừa tạo, vào tab Import (Nhập) và tải lên file create_database.sql có trong dự án.

3. Cấu hình kết nối:

Mở file config/db_connect.php và đảm bảo các thông tin sau là chính xác (thường là mặc định của XAMPP):

private $host = "127.0.0.1";
private $db_name = "library";
private $username = "root";
private $password = "";

4. Truy cập trang web:

Mở trình duyệt và truy cập vào địa chỉ:

http://localhost/quanlythuvien/login.html

(Nếu bạn đã đổi cổng Apache, hãy dùng http://localhost:[PORT]/quanlythuvien/)

🔑 Tài khoản Admin mặc định
Để truy cập các chức năng quản trị, hãy sử dụng tài khoản sau:

Tên đăng nhập: admin

Mật khẩu: admin1234