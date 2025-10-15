QuanLyTaiChinh_KTPM_Nhom99-main/
└── jfins/
    ├── api/                <- Chứa các file PHP xử lý logic (backend)
    │   ├── auth/           # Xác thực người dùng
    │   ├── expense/        # Xử lý chi tiêu
    │   ├── income/         # Xử lý thu nhập
    │   └── jar/            # Xử lý liên quan đến các hũ
    ├── assets/             <- Chứa tài nguyên tĩnh
    │   ├── css/            # Các file CSS
    │   ├── js/             # Các file JavaScript
    │   └── icon/           # Các icon
    ├── config/             <- Chứa file kết nối CSDL
    │   └── db_connect.php
    ├── page/               <- Chứa các trang chính của ứng dụng
    │   ├── auth/
    │   │   └── auth.php    <- Trang đăng nhập/đăng ký
    │   └── index.php       <- Trang tổng quan chính
    └── sql/
        └── create_database.sql <- File mã lệnh để tạo CSDL
