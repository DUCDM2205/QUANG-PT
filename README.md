# FORGE PT — Demo HTML/CSS/JS

## Mở demo
Mở index.html hoặc dùng VS Code Live Server. Không cần npm hay build.

## Font tiếng Việt
Font DejaVu Sans được nhúng tại assets/fonts, kèm giấy phép. Không cần Google Fonts hay Internet để tải font. Giữ nguyên thư mục assets khi upload. Các HTML dùng UTF-8; lưu file trong VS Code bằng UTF-8.

## Upload GitHub bằng trình duyệt
1. Đăng nhập GitHub, chọn New repository, đặt tên forge-pt, chọn Public, rồi Create repository.
2. Chọn uploading an existing file (hoặc Add file → Upload files).
3. Giải nén ZIP này. Kéo TOÀN BỘ nội dung bên trong forge-pt-source lên, gồm 5 file HTML, style.css, app.js, assets, README.md và .nojekyll. index.html phải nằm ngay ở gốc repository.
4. Chọn Commit changes.
5. Vào Settings → Pages → Build and deployment → Deploy from a branch, chọn main và /(root), bấm Save.
6. Chờ GitHub hoàn tất triển khai; mở URL hiển thị tại Settings → Pages.

## Upload bằng Git tại VS Code
Tạo repository GitHub rỗng trước (không thêm README). Mở terminal ngay trong thư mục có index.html:

```bash
git init
git add .
git commit -m "Add FORGE PT demo with Vietnamese fonts"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/forge-pt.git
git push -u origin main
```
Thay YOUR_USERNAME và tên repo cho đúng. Đăng nhập theo hướng dẫn GitHub; không dùng mật khẩu tài khoản làm mật khẩu Git. Sau đó bật Pages như trên.

## Cập nhật lần sau
```bash
git add .
git commit -m "Update website"
git push
```

## Nội dung cần thay
Hồ sơ, thương hiệu, kết quả học viên và ảnh là mẫu. Nút gọi/Zalo hiện mở thông báo demo; thay bằng thông tin thật khi triển khai chức năng. Ảnh minh họa Unsplash. Không có backend hoặc form lưu dữ liệu.
