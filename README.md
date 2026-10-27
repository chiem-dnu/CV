# Portfolio CV - Nguyễn Văn An

Trang portfolio/CV cá nhân giới thiệu Nguyễn Văn An, Frontend Developer. Dự án được xây dựng bằng HTML và CSS thuần, trình bày thông tin giới thiệu, kỹ năng, các dự án tiêu biểu và phương thức liên hệ trong một trang web responsive.

## Chức năng

- Điều hướng đến các phần Giới thiệu, Kỹ năng, Dự án và Liên hệ.
- Hiển thị thông tin cá nhân, vai trò nghề nghiệp và ảnh đại diện.
- Trình bày kỹ năng chuyên môn dưới dạng danh sách.
- Giới thiệu bốn dự án mẫu: Landing Page Sản Phẩm, Ứng dụng Todo List, Weather Dashboard và Blog Cá Nhân.
- Cung cấp email và liên kết GitHub, LinkedIn.
- Tương thích với màn hình điện thoại, máy tính bảng và máy tính.
- Hỗ trợ điều hướng bằng liên kết neo, cuộn mượt và một số thuộc tính hỗ trợ trình đọc màn hình.

> **Lưu ý:** Nội dung dự án và thông tin liên hệ trên trang hiện mang tính minh họa. Hãy cập nhật thông tin cá nhân, liên kết dự án và ảnh đại diện trước khi sử dụng chính thức.

## Công nghệ sử dụng

- **HTML5:** cấu trúc nội dung và các phần tử ngữ nghĩa.
- **CSS3:** giao diện, bố cục Flexbox/Grid, hiệu ứng và responsive theo hướng mobile-first.
- **JavaScript:** chưa được sử dụng trong phiên bản hiện tại.
- **Không sử dụng framework, thư viện bên ngoài, trình quản lý gói hoặc quy trình build.**

## Yêu cầu môi trường

- Windows, macOS hoặc Linux.
- Trình duyệt web hiện đại như Chrome, Firefox, Edge hoặc Safari.
- Không cần cài Node.js hay tải thêm thư viện để xem trang.
- **Tùy chọn:** Python 3 nếu muốn chạy trang qua máy chủ HTTP cục bộ thay vì mở trực tiếp tệp HTML.
- **Tùy chọn:** Visual Studio Code và tiện ích Live Server để thuận tiện xem trước khi phát triển.

## Cấu trúc dự án

```text
.
├── index.html
├── assets/
│   ├── css/
│   │   └── styles.css
│   └── img/
│       └── avatar.jpg
└── README.md
```

## Cài đặt và cấu hình

1. Tải hoặc sao chép mã nguồn dự án về máy.
2. Giữ nguyên cấu trúc thư mục để các đường dẫn tới CSS và ảnh hoạt động:
   - CSS: `assets/css/styles.css`
   - Ảnh đại diện: `assets/img/avatar.jpg`
3. Mở `index.html` bằng trình soạn thảo để chỉnh sửa nội dung.
4. Trước khi xuất bản, cập nhật thông tin mẫu trong `index.html`, bao gồm email, URL GitHub, LinkedIn, mô tả và liên kết các dự án. Thay ảnh tại `assets/img/avatar.jpg` nếu cần; nên giữ nguyên tên tệp hoặc cập nhật đường dẫn ảnh tương ứng trong HTML.

Dự án không có tệp cấu hình môi trường `.env` và không cần cài đặt dependency.

## Chạy thử

### Cách nhanh: mở trực tiếp bằng trình duyệt

Mở thư mục dự án rồi nhấp đúp vào `index.html`, hoặc chọn mở tệp này bằng trình duyệt. Cách này phù hợp để xem giao diện cơ bản.

### Chạy bằng máy chủ HTTP cục bộ

Máy chủ cục bộ giúp xem trang qua địa chỉ `http://localhost:8000` và phản ánh sát hơn cách website được phục vụ. Cài Python 3 trước nếu máy chưa có Python.

#### Windows

1. Mở **PowerShell** hoặc **Windows Terminal**.
2. Chuyển đến thư mục dự án (thay đường dẫn mẫu bằng vị trí thực tế của bạn):

   ```powershell
   cd "C:\duong-dan\den\thu-muc-du-an"
   ```

3. Khởi chạy máy chủ:

   ```powershell
   py -m http.server 8000
   ```

   Nếu lệnh `py` không có sẵn, thử:

   ```powershell
   python -m http.server 8000
   ```

4. Mở `http://localhost:8000` trong trình duyệt.
5. Nhấn `Ctrl+C` trong cửa sổ terminal để dừng máy chủ.

#### macOS

1. Mở **Terminal**.
2. Chuyển đến thư mục dự án:

   ```bash
   cd "/duong-dan/den/thu-muc-du-an"
   ```

3. Khởi chạy máy chủ:

   ```bash
   python3 -m http.server 8000
   ```

4. Mở `http://localhost:8000` trong trình duyệt.
5. Nhấn `Control+C` trong Terminal để dừng máy chủ.

#### Linux

1. Mở ứng dụng **Terminal**.
2. Chuyển đến thư mục dự án:

   ```bash
   cd "/duong-dan/den/thu-muc-du-an"
   ```

3. Khởi chạy máy chủ:

   ```bash
   python3 -m http.server 8000
   ```

4. Mở `http://localhost:8000` trong trình duyệt.
5. Nhấn `Ctrl+C` trong Terminal để dừng máy chủ.

> Nếu cổng `8000` đang được sử dụng, thay `8000` trong lệnh chạy và địa chỉ truy cập bằng một cổng khác, ví dụ `8080`.

### Xem trước bằng Visual Studio Code (tùy chọn)

Mở thư mục dự án trong Visual Studio Code, cài tiện ích **Live Server** nếu chưa có, sau đó nhấp chuột phải vào `index.html` và chọn **Open with Live Server**. Trình duyệt sẽ mở trang qua máy chủ cục bộ.

## Thông tin liên hệ

- **Tên hiển thị:** Nguyễn Văn An
- **Email mẫu:** [an.nguyen@example.com](mailto:an.nguyen@example.com)
- **GitHub mẫu:** `github.com/nguyenvanan`
- **LinkedIn mẫu:** `linkedin.com/in/nguyenvanan`

Các địa chỉ trên là dữ liệu minh họa từ trang hiện tại, không nên xem là thông tin liên hệ đã được xác minh. Hãy thay bằng thông tin thật trước khi công khai website.