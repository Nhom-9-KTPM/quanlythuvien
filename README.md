📚 App Quản Lý Thư Viện - LibMaster

LibMaster là ứng dụng web quản lý thư viện trực quan và hiện đại, giúp quản trị viên, thủ thư và độc giả dễ dàng quản lý sách, theo dõi mượn – trả, và tra cứu tài liệu một cách nhanh chóng, hiệu quả và chính xác.
Dự án được phát triển theo kiến trúc Client–Server, sử dụng PHP & MySQL cho backend và JavaScript cho frontend.

👥 Thành viên nhóm

Dự án được thực hiện bởi nhóm KTPM - Nhóm 99:

🧑‍💻 Phạm Lê Đình An

🧑‍🏫 Hà Lê Quang Minh

🧑‍🎓 Nguyễn Duy Anh Tuấn

🧑‍💼 Nguyễn Đức Tuấn

📘 Giới thiệu

LibMaster được xây dựng nhằm hỗ trợ công tác quản lý thư viện trong các trường học, trung tâm và cơ quan, giúp số hóa quy trình truyền thống, tiết kiệm thời gian và hạn chế sai sót.
Ứng dụng cung cấp giao diện dễ sử dụng, thao tác nhanh gọn và hệ thống phân quyền rõ ràng giữa độc giả, thủ thư và quản trị viên.

🚀 Chức năng chính
🔹 Dành cho Người dùng / Độc giả

Đăng ký / Đăng nhập / Đăng xuất
→ Quản lý tài khoản người dùng, phân quyền rõ ràng (Độc giả, Thủ thư, Admin).

Xem danh sách sách trong thư viện
→ Hiển thị danh mục gồm tên sách, tác giả, thể loại, năm xuất bản, số lượng.

Tìm kiếm sách
→ Tìm theo tên sách, tác giả, thể loại hoặc mã ISBN.

Xem chi tiết sách
→ Thông tin mô tả, tình trạng hiện tại (Còn / Đã mượn / Đặt trước).

Đặt mượn sách
→ Gửi yêu cầu mượn khi sách có sẵn trong thư viện.

Xem lịch sử mượn – trả
→ Danh sách các sách đã mượn, đang mượn, và ngày trả dự kiến.

🔹 Dành cho Quản trị viên / Thủ thư

Quản lý sách
→ Thêm, sửa, xóa thông tin sách.
→ Cập nhật số lượng, tình trạng sách (còn, đã mượn, mất, hỏng...).

Quản lý độc giả
→ Thêm mới hoặc khóa tài khoản người dùng.
→ Xem thông tin mượn – trả của từng độc giả.

Quản lý mượn – trả sách
→ Xác nhận khi người dùng mượn hoặc trả sách.
→ Cập nhật ngày mượn, ngày trả thực tế và dự kiến.

🛠️ Công nghệ sử dụng

Dự án được xây dựng trên kiến trúc Client-Server với các công nghệ chính:

Backend:

Ngôn ngữ: PHP

Cơ sở dữ liệu: MySQL

Mô tả: Xử lý logic nghiệp vụ, quản lý phiên đăng nhập và giao tiếp với CSDL.

Frontend:

Ngôn ngữ: HTML, CSS, JavaScript

Thư viện: Chart.js, Bootstrap

Mô tả: Xây dựng giao diện thân thiện, trực quan và responsive.

🗂️ Cấu trúc thư mục
QuanLyThuVien_KTPM_Nhom99/
└── libmaster/
├── api/ <- Chứa các file PHP xử lý logic (backend)
│ ├── auth/ # Xác thực người dùng
│ ├── books/ # Quản lý sách
│ ├── borrow/ # Xử lý mượn - trả sách
│ └── users/ # Quản lý người dùng
├── assets/ <- Chứa tài nguyên tĩnh
│ ├── css/ # Các file CSS
│ ├── js/ # Các file JavaScript
│ └── icon/ # Icon giao diện
├── config/ <- Cấu hình cơ sở dữ liệu
│ └── db_connect.php
├── page/ <- Các trang chính của ứng dụng
│ ├── auth/
│ │ └── login.php <- Trang đăng nhập / đăng ký
│ ├── dashboard.php <- Trang tổng quan (Admin / Thủ thư)
│ └── books.php <- Trang danh sách và tìm kiếm sách
└── sql/
└── create_database.sql <- File khởi tạo CSDL

⚙️ Hướng dẫn cài đặt (Local - XAMPP)
1️⃣ Cài đặt XAMPP

Tải và cài đặt XAMPP (phiên bản có PHP & MySQL).
Khởi động Apache và MySQL trong XAMPP Control Panel.

2️⃣ Sao chép dự án

Copy thư mục QuanLyThuVien_KTPM_Nhom99 vào:

C:\xampp\htdocs

3️⃣ Tạo cơ sở dữ liệu

Mở trình duyệt → truy cập http://localhost/phpmyadmin/

Tạo database mới tên là libmaster, mã hóa utf8mb4_unicode_ci

4️⃣ Import dữ liệu

Chọn database libmaster → tab Import

Tải file create_database.sql từ thư mục /sql

Nhấn Go để thực thi.

5️⃣ Chạy ứng dụng

Truy cập:

http://localhost/QuanLyThuVien_KTPM_Nhom99/libmaster/page/auth/login.php


Bây giờ bạn có thể đăng ký tài khoản và bắt đầu sử dụng ứng dụng 🎉

📬 Liên hệ

Nếu bạn có câu hỏi hoặc muốn đóng góp cho dự án, vui lòng liên hệ:

📧 Email: nhom99@gmail.com

📄 License: MIT License © 2025

“Tri thức là sức mạnh — Hãy để LibMaster giúp bạn quản lý tri thức hiệu quả hơn.”
