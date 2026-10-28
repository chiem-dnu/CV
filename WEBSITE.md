# HER.STORY — Personal Portfolio

## 1. Tên dự án

**HER.STORY — Personal Portfolio** là website portfolio cá nhân giới thiệu thông tin, học vấn, kỹ năng, dự án và hành trình phát triển của chủ sở hữu.

## 2. Mô tả

Website được định hướng là một trang tĩnh theo phong cách editorial, sử dụng nội dung tiếng Việt kết hợp một số tiêu đề tiếng Anh. Người xem có thể dùng menu và các liên kết neo để chuyển đến từng phần trên cùng một trang.

> **Tình trạng mã nguồn:** Tài liệu này mô tả mã nguồn hiện có, không phải một hệ thống đã có backend. `index.html` đang tham chiếu `style.css`, trong khi stylesheet trong dự án nằm tại `assets/css/styles.css`. Ngoài ra, `index.html` hiện kết thúc giữa phần Mục tiêu. Cần hoàn thiện HTML và kiểm tra, kết nối stylesheet trước khi xem website là bản chạy hoàn chỉnh.

## 3. Chức năng

### Các phần nội dung

- Trang chủ/hero giới thiệu và liên kết khám phá, liên hệ.
- Giới thiệu bản thân.
- Học vấn.
- Kỹ năng.
- Danh sách dự án mẫu.
- Thư viện ảnh.
- Hành trình và mục tiêu.
- Khu vực liên hệ.
- Menu điều hướng bằng liên kết neo.

Tên, trường học, ngành học, ảnh, dự án và nội dung cá nhân trong HTML hiện là nội dung mẫu; hãy thay bằng dữ liệu được phép công khai.

### Đăng nhập và đăng ký

**Đăng nhập và đăng ký chưa được triển khai.** Mã nguồn hiện tại không có giao diện biểu mẫu xác thực, xử lý tài khoản, API, backend hay cơ sở dữ liệu. Vì vậy, người dùng hiện không thể tạo tài khoản hoặc đăng nhập; không nhập hoặc lưu mật khẩu trên website này.

Nếu bổ sung chức năng này trong phiên bản sau, cần xây dựng giao diện đăng ký/đăng nhập, xác thực dữ liệu ở cả máy khách và máy chủ, backend/API, lưu trữ thông tin tài khoản an toàn và quản lý phiên đăng nhập. Không xem các màn hình tĩnh hoặc dữ liệu lưu trong trình duyệt là cơ chế xác thực thực tế.

## 4. Công nghệ

- **HTML5:** cấu trúc và nội dung trang.
- **CSS3:** stylesheet hiện có tại `assets/css/styles.css`, có các quy tắc bố cục và breakpoint mobile-first.
- **JavaScript:** chưa có tệp JavaScript độc lập trong dự án; không có quy trình build.
- **Thư viện/framework:** chưa sử dụng.
- **Backend/cơ sở dữ liệu:** chưa có.
- **Docker:** chưa có `Dockerfile` hoặc tệp Docker Compose; có thể dùng image Nginx có sẵn để phục vụ tệp tĩnh (xem hướng dẫn bên dưới).

## 5. Yêu cầu môi trường

- Windows, macOS hoặc Linux.
- Trình duyệt hiện đại như Chrome, Firefox, Edge hoặc Safari.
- Không cần cài Node.js, trình quản lý gói hoặc dependency.
- **Tùy chọn:** Python 3 để chạy máy chủ HTTP cục bộ.
- **Tùy chọn:** Docker Desktop trên Windows/macOS hoặc Docker Engine trên Linux để chạy bằng container.
- **Tùy chọn:** Visual Studio Code để chỉnh sửa mã nguồn.

## 6. Cài đặt và cấu hình

1. Tải hoặc sao chép mã nguồn về máy.
2. Giữ nguyên cấu trúc thư mục để các đường dẫn tương đối hoạt động:

   ```text
   .
   ├── index.html
   ├── assets/
   │   ├── css/
   │   │   └── styles.css
   │   └── img/
   └── docs/
   ```

3. Mở `index.html` trong trình soạn thảo để cập nhật nội dung mẫu và các đường dẫn ảnh.
4. Trước khi chạy, sửa tham chiếu stylesheet trong `index.html` để trỏ đến `assets/css/styles.css` (hoặc đặt stylesheet đúng tại đường dẫn đang được tham chiếu).
5. Hoàn thiện phần HTML đang bị dở ở cuối `index.html`.
6. Dự án hiện không có tệp `.env`, cấu hình bí mật, bước cài dependency hoặc bước biên dịch.

## 7. Giao diện responsive và clean code

### Responsive

Stylesheet hiện có ghi nhận thiết kế mobile-first với các breakpoint từ `768px` (tablet) và `1280px` (desktop); lưới dự án được định hướng hiển thị một cột trên mobile, hai cột trên tablet và ba cột trên desktop.

Do stylesheet chưa được liên kết đúng trong HTML và HTML hiện chưa hoàn chỉnh, các breakpoint này **chưa thể được xác nhận là đang áp dụng cho giao diện thực tế**. Sau khi hoàn thiện mã nguồn:

1. Kiểm tra tối thiểu ở chiều rộng 360px (mobile), 768px (tablet) và 1280px (desktop).
2. Xác nhận không có cuộn ngang, nội dung không bị cắt, menu và liên kết có thể thao tác bằng cảm ứng/bàn phím.
3. Kiểm tra ảnh co giãn theo khung và chữ dễ đọc ở từng kích thước.

### Quy ước clean code

- Dùng phần tử HTML ngữ nghĩa và cấu trúc thụt lề nhất quán.
- Tách cấu trúc HTML khỏi kiểu trình bày CSS; dùng tên lớp rõ nghĩa và tái sử dụng quy tắc chung.
- Giữ đường dẫn tài nguyên tương đối và cập nhật chúng khi đổi vị trí tệp.
- Cung cấp văn bản thay thế cho ảnh và trạng thái focus dễ nhận biết cho điều hướng.
- Xóa nội dung mẫu, mã không dùng và các xử lý lỗi nội tuyến trước khi phát hành; kiểm tra HTML/CSS sau mỗi thay đổi.

## 8. Chạy thử

### Mở trực tiếp

Mở thư mục dự án và mở `index.html` bằng trình duyệt. Cách này không cần cài thêm công cụ, nhưng không thay thế việc kiểm tra website qua máy chủ HTTP. Lưu ý các vấn đề về HTML chưa hoàn chỉnh và đường dẫn CSS ở mục **Cài đặt và cấu hình**.

### Chạy trên Windows

1. Mở PowerShell hoặc Windows Terminal.
2. Chuyển đến thư mục dự án:

   ```powershell
   cd "C:\duong-dan\den\thu-muc-du-an"
   ```

3. Chạy máy chủ HTTP:

   ```powershell
   py -m http.server 8000
   ```

   Nếu lệnh `py` không có sẵn, thử:

   ```powershell
   python -m http.server 8000
   ```

4. Mở `http://localhost:8000` trong trình duyệt.
5. Nhấn `Ctrl+C` trong terminal để dừng máy chủ.

### Chạy trên macOS

1. Mở Terminal và chuyển đến thư mục dự án:

   ```bash
   cd "/duong-dan/den/thu-muc-du-an"
   ```

2. Chạy máy chủ:

   ```bash
   python3 -m http.server 8000
   ```

3. Mở `http://localhost:8000` trong trình duyệt.
4. Nhấn `Control+C` trong Terminal để dừng máy chủ.

### Chạy trên Linux

1. Mở Terminal và chuyển đến thư mục dự án:

   ```bash
   cd "/duong-dan/den/thu-muc-du-an"
   ```

2. Chạy máy chủ:

   ```bash
   python3 -m http.server 8000
   ```

3. Mở `http://localhost:8000` trong trình duyệt.
4. Nhấn `Ctrl+C` trong Terminal để dừng máy chủ.

> Nếu cổng `8000` đang được sử dụng, thay `8000` trong lệnh và URL bằng một cổng khác, chẳng hạn `8080`.

### Chạy bằng Docker

Docker chỉ phục vụ các tệp tĩnh bằng Nginx; dự án hiện không có Dockerfile, Docker Compose hoặc backend. Cài và khởi động Docker trước khi chạy lệnh.

**Windows PowerShell:**

```powershell
docker run --rm --name her-story -p 8000:80 -v "${PWD}:/usr/share/nginx/html:ro" nginx:alpine
```

**macOS/Linux:**

```bash
docker run --rm --name her-story -p 8000:80 -v "$PWD:/usr/share/nginx/html:ro" nginx:alpine
```

Mở `http://localhost:8000` để xem trang. Nhấn `Ctrl+C` trong terminal để dừng container. Nếu cổng `8000` đang bận, đổi phần `8000:80` và URL sang cổng trống khác, ví dụ `8080:80` và `http://localhost:8080`.

### Xem trước với Visual Studio Code (tùy chọn)

Mở thư mục dự án trong Visual Studio Code, cài tiện ích Live Server nếu cần, sau đó mở `index.html` bằng Live Server.

## 9. Thông tin liên hệ

Thông tin liên hệ cá nhân chưa được xác nhận trong mã nguồn hiện tại. Trước khi công khai website, hãy cập nhật phần Liên hệ trong `index.html` bằng thông tin thật mà chủ sở hữu đồng ý chia sẻ, ví dụ:

- **Tên hiển thị:** `[Tên của bạn]`
- **Email:** `[email-của-bạn]`
- **GitHub:** `[liên kết GitHub]`
- **LinkedIn:** `[liên kết LinkedIn]`
