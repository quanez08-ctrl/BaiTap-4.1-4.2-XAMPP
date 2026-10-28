# Bài tập 4.1 và 4.2 – PHP + MySQL (XAMPP)

Hai bài được triển khai thành website PHP chạy trên XAMPP, sử dụng MySQL/MariaDB để lưu dữ liệu.

## Yêu cầu
- XAMPP có Apache và MySQL/MariaDB
- Trình duyệt web

## Cài đặt
1. Giải nén thư mục `BaiTap_4_1_4_2_XAMPP` vào `C:\xampp\htdocs\`.
2. Mở XAMPP Control Panel, nhấn **Start** ở Apache và MySQL.
3. Mở `http://localhost/phpmyadmin`.
4. Chọn tab **Import**, chọn file `database.sql`, rồi nhấn **Import**.
5. Truy cập:
   - Bài 4.1: `http://localhost/BaiTap_4_1_4_2_XAMPP/bai4_1/`
   - Bài 4.2: `http://localhost/BaiTap_4_1_4_2_XAMPP/bai4_2/`

## Tài khoản demo bài 4.1
- Tên đăng nhập: `admin`
- Mật khẩu: `Admin@123`

Mật khẩu được lưu trong CSDL dưới dạng hash, không lưu dạng văn bản thuần.

## Nội dung
- `bai4_1/`: Đăng nhập, xác thực tài khoản từ bảng `users`, tạo tài khoản mới, đăng xuất.
- `bai4_2/`: Form đăng ký khóa học; lưu họ tên, số điện thoại, ngày sinh, khóa học, giới tính, các nội dung quan tâm vào bảng `registrations`; có trang xem danh sách đăng ký.
- `database.sql`: Tạo database, bảng và dữ liệu mẫu.

## Đưa lên GitHub
Tạo repository mới trên GitHub, sau đó mở Terminal tại thư mục project và chạy:
```bash
git init
git add .
git commit -m "Nang cap bai tap 4.1 va 4.2 voi MySQL"
git branch -M main
git remote add origin https://github.com/<TEN_TAI_KHOAN>/<TEN_REPOSITORY>.git
git push -u origin main
```
Thay `<TEN_TAI_KHOAN>` và `<TEN_REPOSITORY>` bằng thông tin repository của bạn.

## Lưu ý về bài 4.1 gốc
File bạn gửi trong cuộc trò chuyện là file `.sln` tham chiếu tới `LoginForm\LoginForm.csproj`, chưa có mã nguồn `.cs`/`.csproj` và tài nguyên giao diện. Vì vậy bản PHP này dựng lại chức năng đăng nhập để chạy bằng XAMPP, chưa thể bảo toàn chính xác giao diện và logic riêng của project C# gốc.
