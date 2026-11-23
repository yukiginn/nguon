# Kho Plugin Truyện TTS (v3.0 — 100% Khai Báo Rời, Zero Code Trang Web Trong APK)

Kho chứa toàn bộ plugin nguồn truyện & phim rời (đã tách hoàn toàn khỏi file APK). Ứng dụng APK chỉ chứa bộ đọc tổng quát (`configurable_css`), **không chứa bất kỳ tên trang web, tên miền, thể loại hay bộ xử lý riêng của trang nào**. Mọi thể loại, đường dẫn, mirror, API và bộ chọn CSS đều nằm 100% trong từng file `.plugin.json`.

## 9 Nguồn Đọc Truyện Đã Kiểm Chứng Live HTTP 200

| # | Tên nguồn | Tên miền chính | Driver | Số thể loại |
|---|---|---|---|---|
| 1 | **Truyện Full** | `https://truyenfull.live` | `configurable_css` | 59 danh mục & thể loại |
| 2 | **Mê Truyện Chữ** | `https://metruyenchu.com.vn` | `configurable_css` | 52 danh mục & thể loại |
| 3 | **WebTruyen (DTruyen)** | `https://wetruyen.com` (gương `webtruyen.com`, `dtruyen.com`) | `configurable_css` | 46 danh mục & thể loại Full |
| 4 | **Truyện Wiki Dịch** | `https://truyenwikidich.net` (gương `wikicv.org`) | `configurable_css` | 4 mục chính (Truyện Nam, Nữ Tần, Đam Mỹ, Chương Mới) |
| 5 | **69 Thư Ba (69shuba)** | `https://www.69shuba.com` (gương `69shuba.com`, `69shu.com`, `69shuba.cx`) | `configurable_css` | 17 bảng xếp hạng & thể loại |
| 6 | **Cà Chua (Fanqie)** | `https://fanqienovel.com` | `configurable_css` (JSON API + cipher) | 14 danh mục API trực tiếp |
| 7 | **Bút Thú Các (Biquge)** | `https://www.bqg9.xyz` (gương `biquge5200.cc`) | `configurable_css` | 9 danh mục & thể loại |
| 8 | **Phiêu Thiên Văn Học (Piaotia)** | `https://www.piaotia.com` | `configurable_css` (GB18030) | 12 bảng xếp hạng & thể loại |
| 9 | **Truyện YY (TruyenYY.co)** | `https://truyenyy.co` | `configurable_css` | 14 danh sách & chủ đề |

## Plugin Xem Phim

- `phimai_sources.plugin.json`: Nguồn phim tách rời cho tab Phim (nạp bằng nút **Nguồn phim** trong tab Phim).

## Cách sử dụng

1. Giải nén file `novel-plugins-repo.zip` và đẩy toàn bộ thư mục (`catalog.json`, `phimai_sources.plugin.json`, thư mục `plugins/`) lên kho GitHub/GitLab của bạn.
2. Mở ứng dụng **Truyện TTS → Cài đặt → Quản lý Plugin → Kho Git**.
3. Dán link kho Git của bạn và nhấn **Đồng bộ**, sau đó cài đặt/cập nhật các nguồn mong muốn.
