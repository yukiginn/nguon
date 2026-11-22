# Kho Plugin Nguồn Truyện Rời (Manifest v2)

Thư mục này là một **kho Git độc lập** nằm hoàn toàn bên ngoài ứng dụng Android (APK không đóng gói sẵn nguồn truyện). Bạn có thể đẩy nguyên thư mục `novel-plugins-repo` này lên **GitHub**, **GitLab** hoặc **Gitee**, sau đó dán đường dẫn kho Git vào ứng dụng để nạp nguồn truyện chỉ với 1 chạm.

## Danh sách 14 nguồn truyện đi kèm

### Nguồn Trung (8 nguồn — tự động dịch VietPhrase)
1. **69 Thư Ba (`69shuba_cn`)** — Hỗ trợ bảng mã GBK, tìm kiếm POST, nhiều tên miền dự phòng.
2. **Phiêu Thiên Văn Học (`piaotia_cn`)** — Nguồn lâu đời sạch chữ, bảng mã GBK.
3. **Đài Loan Khán Thư (`twkan_cn`)** — Tự động chuyển Phồn Thể sang Giản Thể trước khi dịch.
4. **UU Khán Thư (`uukanshu_cn`)** — Kho miễn phí lớn, hỗ trợ tên miền dự phòng.
5. **Thư Hải Các (`shuhaige_cn`)** — Bản di động nhanh, tự động ghép các trang chương bị chia nhỏ.
6. **Bút Thú Các (`biquge_cn`)** — Hệ thống nguồn kinh điển kèm nhiều mirror dự phòng.
7. **Cà Chua Tiểu Thuyết (`fanqie_cn`)** — Hỗ trợ đăng nhập tài khoản WebView & dán Cookie.
8. **Thất Miêu & Khởi Điểm (`qimao_qidian_cn`)** — Hỗ trợ đăng nhập tài khoản cá nhân để đọc chương VIP đã mua.

### Nguồn Việt (6 nguồn)
9. **Tàng Thư Viện (`tangthuvien_vi`)** — Kho truyện Tiên Hiệp, Kiếm Hiệp, Ngôn Tình nổi tiếng.
10. **Sáng Tác Việt (`sangtacviet_vi`)** — Hỗ trợ đăng nhập tài khoản & tên miền dự phòng.
11. **Truyện Chữ & SSTruyen (`truyenchu_sstruyen_vi`)** — Nguồn miễn phí đa thể loại.
12. **Truyện Full (`truyenfull_vi`)** — Phiên bản v2 kèm danh sách tên miền dự phòng.
13. **Mê Truyện Chữ (`metruyenchu_vi`)** — Hỗ trợ đăng nhập WebView / Cookie cho chương VIP.
14. **WikiDịch & Dtruyen (`wikidich_dtruyen_vi`)** — Hỗ trợ đăng nhập WebView / Cookie & mirror dự phòng.

### Nguồn Xem Phim / YouTube rời (`phimai_sources.plugin.json`)
- Gói nguồn **Xem Phim AI Youtube** đã được tách hoàn toàn khỏi APK và đặt tại tệp `phimai_sources.plugin.json` ở thư mục gốc của kho Git này.
- Để nạp trong ứng dụng: mở mục **Phim** → dán thẳng liên kết kho Git của bạn (`https://github.com/<ten-cua-ban>/truyen-plugins`) hoặc đường dẫn tới tệp `phimai_sources.plugin.json` → bấm **Nạp nguồn từ Git / JSON**.

## Cách đẩy lên GitHub và nạp vào ứng dụng

1. Tạo một repository công khai (Public) trên GitHub, ví dụ: `https://github.com/<ten-cua-ban>/truyen-plugins`.
2. Đẩy toàn bộ nội dung trong thư mục `novel-plugins-repo/` lên nhánh `main` sao cho `catalog.json` và `phimai_sources.plugin.json` nằm ở thư mục gốc, còn các tệp `.plugin.json` nguồn truyện nằm trong `plugins/`.
3. **Nạp nguồn truyện:** Mở **Quản lý Nguồn truyện** → tab **Kho Git** → bấm **Thêm Kho Git** → dán đường dẫn `https://github.com/<ten-cua-ban>/truyen-plugins`.
4. **Nạp nguồn phim YouTube:** Mở mục **Phim** → dán đường dẫn kho Git trên (hoặc đường dẫn raw `phimai_sources.plugin.json`) → bấm **Nạp nguồn**.

## Lưu ý về đăng nhập & Chống chặn mạng
- Mọi phiên đăng nhập (Cookie WebView hoặc Cookie dán thủ công) được lưu **mã hóa cục bộ trên thiết bị**, chỉ dùng cho tài khoản hợp lệ của chính bạn.
- Khi một tên miền bị nhà mạng chặn hoặc đổi địa chỉ, hãy mở **Quản lý Nguồn → tab Mạng & Proxy** để bật **DNS-over-HTTPS (1.1.1.1 / 8.8.8.8)**, thiết lập **Proxy (HTTP/SOCKS5)**, hoặc bấm **Tên miền & Kiểm tra** ngay trên thẻ nguồn truyện để đổi sang tên miền dự phòng.
