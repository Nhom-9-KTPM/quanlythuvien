
QuanLyThuVien_KTPM_Nhom99/
└── libmaster/
    ├── api/                <- Chứa các file PHP xử lý logic (backend)
    │   ├── auth/           # Xác thực người dùng
    │   ├── books/          # Quản lý sách
    │   ├── borrow/         # Xử lý mượn - trả sách
    │   └── users/          # Quản lý người dùng
    ├── assets/             <- Chứa tài nguyên tĩnh
    │   ├── css/            # Các file CSS
    │   ├── js/             # Các file JavaScript
    │   └── icon/           # Icon giao diện
    ├── config/             <- Cấu hình cơ sở dữ liệu
    │   └── db_connect.php
    ├── page/               <- Các trang chính của ứng dụng
    │   ├── auth/
    │   │   └── login.php   <- Trang đăng nhập / đăng ký
    │   ├── dashboard.php   <- Trang tổng quan (Admin / Thủ thư)
    │   └── books.php       <- Trang danh sách và tìm kiếm sách
    └── sql/
        └── create_database.sql <- File khởi tạo CSDL
