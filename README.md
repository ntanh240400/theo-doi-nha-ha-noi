# Theo dõi nhà Hà Nội

App web tĩnh (1 file `index.html`, không build, không server) hiển thị danh sách nhà đang theo dõi.
Dữ liệu được đọc **trực tiếp từ Google Sheet** mỗi lần mở trang — Sheet cập nhật là trang tự cập nhật.

- **Nguồn dữ liệu:** Google Sheet “Tìm nhà Hà Nội — Nino 2026”
  (ID `1Te44C8dwth9vSWuEX1BxI0s3V_sWi-OgSajlrIZtEa8`), tab **“Nhà trên Facebook”**
- **Cột dùng:** A Giá · B Ngày đăng · C Tiêu đề · D Diện tích · E Khu vực · F SĐT ·
  G Ghi chú · H Link · I Đã nhắn · J Đã check · K Comment
- **Tính năng:** tìm kiếm, lọc theo khu vực / giá tối đa, sắp xếp (thứ hạng, giá, giá/m²),
  ẩn căn đã loại (ghi chú chứa “LOẠI”), thẻ căn có giá/m² tự tính, nút mở tin Facebook và gọi điện.

## Điều kiện để trang đọc được Sheet

Sheet phải bật chia sẻ: **Share → General access → “Anyone with the link” → Viewer**.
Nếu chưa bật, trang sẽ hiện thông báo hướng dẫn thay vì danh sách.

## Deploy

Trang chạy bằng GitHub Pages từ branch `gh-pages` (hoặc `main` nếu bật Pages trong
Settings → Pages → Deploy from a branch). Sửa `index.html` rồi push lại là trang tự cập nhật.
