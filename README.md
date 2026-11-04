# Phạm Hoàng Phúc — Portfolio CV

## 1. Tên dự án

**Portfolio CV cá nhân của Phạm Hoàng Phúc**

## 2. Mô tả

Đây là website portfolio/CV tĩnh giới thiệu Phạm Hoàng Phúc, định hướng Frontend Developer. Trang tổng hợp phần giới thiệu, kỹ năng, các dự án tiêu biểu và thông tin liên hệ. Giao diện được thiết kế responsive để hiển thị trên điện thoại, máy tính bảng và máy tính.

## 3. Chức năng

- Điều hướng nhanh tới các mục Giới thiệu, Kỹ năng, Dự án và Liên hệ.
- Hiển thị ảnh đại diện, thông tin cá nhân và các nút liên hệ/xem dự án.
- Trình bày kỹ năng dưới dạng thẻ.
- Hiển thị danh sách dự án dưới dạng lưới responsive.
- Cung cấp email, GitHub và LinkedIn để liên hệ.
- Hỗ trợ cuộn mượt và các trạng thái tương tác cơ bản.

> Các thẻ “Xem chi tiết” hiện là nội dung minh họa; hãy cập nhật liên kết khi có trang dự án thực tế.

## 4. Công nghệ

- HTML5: cấu trúc và nội dung trang.
- CSS3: giao diện, Flexbox, CSS Grid và responsive design.
- Không sử dụng framework, backend, cơ sở dữ liệu hay bước build.

## 5. Yêu cầu môi trường

Để mở trang trực tiếp:

- Trình duyệt hiện đại như Chrome, Edge, Firefox hoặc Safari.

Để chạy bằng máy chủ cục bộ:

- Python 3 (hoặc một máy chủ web tĩnh tương đương).

Để chạy bằng Docker:

- Docker Engine trên Linux, hoặc Docker Desktop trên Windows/macOS.
- Có kết nối Internet lần đầu để tải image `nginx:alpine`.

Không cần cài Node.js hoặc chạy lệnh cài đặt thư viện.

## 6. Cài đặt

Tải hoặc clone mã nguồn về máy, sau đó mở terminal tại thư mục dự án:

```bash
git clone https://github.com/Phucdzok99/My-CV.git
cd My-CV
```

Nếu đã có mã nguồn trên máy, chỉ cần mở thư mục chứa `index.html`. Dự án không có bước cài dependency.

## 7. Cấu hình và tùy chỉnh

- **Nội dung, tiêu đề, thông tin liên hệ:** chỉnh sửa `index.html`.
- **Giao diện, màu sắc và bố cục:** chỉnh sửa `assets/css/styles.css`.
- **Ảnh đại diện và ảnh dự án:** thay các ảnh trong `assets/img/`; giữ nguyên tên hiện tại hoặc cập nhật đường dẫn `src` tương ứng trong `index.html`.
- **Thông tin liên hệ:** cập nhật cả nội dung hiển thị và liên kết `mailto:`, GitHub, LinkedIn trong mục Liên hệ.
- **Tên/giới thiệu trang:** cập nhật thẻ `<title>`, phần mô tả và nội dung giới thiệu trong `index.html`.

Trang không cần file cấu hình môi trường hay khóa API.

## 8. Chạy thử

### Mở trực tiếp

Mở file `index.html` bằng trình duyệt. Cách này phù hợp để xem nhanh giao diện; dùng máy chủ cục bộ bên dưới nếu trình duyệt giới hạn một số tài nguyên khi mở file trực tiếp.

### Windows

Mở PowerShell tại thư mục dự án và chạy:

```powershell
py -m http.server 8000
```

Nếu lệnh `py` không có nhưng đã cài Python, thử:

```powershell
python -m http.server 8000
```

Mở `http://localhost:8000` trên trình duyệt. Dừng máy chủ bằng `Ctrl+C`.

### macOS

Mở Terminal tại thư mục dự án và chạy:

```bash
python3 -m http.server 8000
```

Mở `http://localhost:8000` trên trình duyệt. Dừng máy chủ bằng `Ctrl+C`.

### Linux

Mở terminal tại thư mục dự án và chạy:

```bash
python3 -m http.server 8000
```

Mở `http://localhost:8000` trên trình duyệt. Dừng máy chủ bằng `Ctrl+C`.

### Docker (Windows, macOS và Linux)

Đảm bảo Docker đang chạy, mở terminal tại thư mục chứa `index.html`, rồi khởi động Nginx để phục vụ các file tĩnh.

**Windows PowerShell:**

```powershell
docker run --rm -d --name my-cv -p 8080:80 -v "${PWD}:/usr/share/nginx/html:ro" nginx:alpine
```

**macOS/Linux (Terminal):**

```bash
docker run --rm -d --name my-cv -p 8080:80 -v "$(pwd):/usr/share/nginx/html:ro" nginx:alpine
```

Mở `http://localhost:8080` trên trình duyệt. Dừng container và tự động xóa container bằng lệnh:

```bash
docker stop my-cv
```

Các lệnh trên mount thư mục dự án ở chế độ chỉ đọc vào Nginx, vì vậy không cần Dockerfile hay bước build image riêng.

## 9. Cấu trúc thư mục

```text
My-CV/
├── index.html
├── README.md
└── assets/
    ├── css/
    │   └── styles.css
    └── img/
        ├── anh1.jpg
        ├── anh2.jpg
        ├── anh3.jpg
        └── hhhh.jpg
```

## 10. Thông tin liên hệ

- **Email:** [zikphuczik@gmail.com](mailto:zikphuczik@gmail.com)
- **GitHub:** [Phucdzok99](https://github.com/Phucdzok99)
- **LinkedIn:** [Phạm Hoàng Phúc](https://www.linkedin.com/in/phamphuc2008)
