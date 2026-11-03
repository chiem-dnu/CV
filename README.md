# Portfolio cá nhân — Hoàng Diệu Chiêm

Website portfolio cá nhân giới thiệu thông tin, kỹ năng, lĩnh vực quan tâm và các dự án mẫu. Giao diện được xây dựng trong một trang HTML, có bố cục responsive và nội dung tiếng Việt.

## Nội dung và tính năng

- Các khu vực Trang chủ, Giới thiệu, Kỹ năng, Công việc, Dự án và Liên hệ.
- Menu điều hướng thu gọn trên màn hình nhỏ và hiệu ứng xuất hiện khi cuộn.
- Biểu mẫu liên hệ kiểm tra các trường bắt buộc ở trình duyệt và hiển thị thông báo xác nhận. Biểu mẫu hiện chỉ là minh họa: không gửi hoặc lưu dữ liệu.
- Trang đăng nhập demo (`Login.html`) sử dụng `sessionStorage`; đây không phải hệ thống xác thực thật.
- Ảnh nằm trong `assets/img/`; CSS và JavaScript của portfolio được đặt trực tiếp trong `index.html`.

## Chạy website

Mở `index.html` bằng trình duyệt hiện đại. Không cần cài dependency hoặc chạy bước build.

Để chạy qua máy chủ HTTP cục bộ, mở terminal tại thư mục dự án và chạy:

```powershell
py -m http.server 8000
```

Sau đó truy cập `http://localhost:8000`. Nếu chưa có lệnh `py`, có thể dùng `python -m http.server 8000`.

## Cấu trúc chính

```text
.
├── index.html
├── Login.html
├── assets/
│   ├── css/
│   └── img/
├── docs/
│   ├── screenshots/
│   └── test_report.md
└── test_report.md
```

## Lưu ý trước khi phát hành

- Thay nội dung dự án mẫu, địa chỉ email và các liên kết mạng xã hội bằng thông tin thật.
- Biểu mẫu liên hệ chưa kết nối backend; không nhập thông tin nhạy cảm.
- Trang đăng nhập chỉ phục vụ minh họa giao diện, không bảo vệ nội dung.
- Font chữ được tải từ Google Fonts khi có kết nối Internet.

## Tài liệu

- [Báo cáo kiểm thử](docs/test_report.md)
- [Ảnh chụp giao diện](docs/screenshots/)
