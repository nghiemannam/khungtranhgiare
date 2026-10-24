# Kế hoạch SEO hằng ngày: "khung bằng khen a4"

Trang chính (trang trụ cột): `bai-viet/khung-bang-khen-a4.html`
URL: https://khungtranhgiare.com/bai-viet/khung-bang-khen-a4.html

Mục tiêu: đưa trang trụ cột lên top Google cho "khung bằng khen a4" bằng cách
mỗi ngày thêm 1 bài viết phụ hữu ích (hoặc cải thiện 1 trang có sẵn), tất cả
đều liên kết về trang trụ cột.

## Quy tắc cho mỗi lần chạy

1. Lấy từ khoá đầu tiên chưa đánh dấu `[x]` trong "Danh sách từ khoá" bên dưới.
2. Viết 1 bài mới trong `bai-viet/<slug>.html`, copy khung giao diện từ
   `bai-viet/khung-bang-khen-a4.html` (header, menu, CSS, footer, FAQ chung).
   - 900–1.500 chữ, tiếng Việt tự nhiên, có ích thật cho người đọc. Không nhồi từ khoá.
   - Không bịa giá, số liệu, đánh giá khách hàng hay chứng nhận. Giá luôn là "liên hệ báo giá".
   - Chỉ dùng ảnh có sẵn trong `hinh-webp/`, alt mô tả đúng ảnh.
   - Cập nhật đủ: `<title>` (≤ 65 ký tự), meta description (≤ 160 ký tự), canonical,
     og:*, JSON-LD Article + BreadcrumbList + FAQPage (FAQ phải hiển thị trong bài).
   - Ít nhất 2 liên kết tới trang trụ cột với anchor khác nhau
     (ví dụ "khung bằng khen A4", "khung giấy khen 21x30"), và liên kết tới
     sản phẩm `../Chi-tiet-san-pham.html#khung-bang-khen-a4-mau-vang|-vang-den|-go`.
3. Thêm thẻ bài mới vào đầu lưới `bai-viet-moi.html` và vào JSON-LD ItemList của trang đó.
4. Thêm bài mới vào "Bài viết liên quan" của trang trụ cột (giữ tối đa ~8 mục).
5. Thêm URL vào `sitemap.xml`; cập nhật `<lastmod>` của trang trụ cột và các trang đã sửa.
6. Kiểm tra JSON-LD hợp lệ (json.loads) và mọi liên kết nội bộ trỏ tới file có thật.
7. Đánh dấu `[x]` từ khoá, ghi 1 dòng vào "Nhật ký", commit và push lên `main`.
8. Cứ mỗi 7 lần chạy, thay vì viết bài mới thì rà lại trang trụ cột: làm mới nội dung,
   thêm câu hỏi thường gặp mới, cập nhật ngày "Cập nhật".

## Danh sách từ khoá

- [ ] khung bằng khen a4 giá rẻ → `khung-bang-khen-a4-gia-re.html`
- [ ] khung giấy khen a4 cho học sinh → `khung-giay-khen-a4-cho-hoc-sinh.html`
- [ ] kích thước khung bằng khen a4 → `kich-thuoc-khung-bang-khen-a4.html`
- [ ] khung bằng khen a4 màu vàng → `khung-bang-khen-a4-mau-vang.html`
- [ ] khung bằng khen 21x30 → `khung-bang-khen-21x30.html`
- [ ] mua khung bằng khen số lượng lớn cho trường học → `khung-bang-khen-so-luong-lon-truong-hoc.html`
- [ ] khung bằng khen a4 màu gỗ → `khung-bang-khen-a4-mau-go.html`
- [ ] khung chứng nhận a4 cho doanh nghiệp → `khung-chung-nhan-a4-doanh-nghiep.html`
- [ ] khung bằng khen a4 vàng đen → `khung-bang-khen-a4-vang-den.html`
- [ ] cách lồng giấy khen vào khung → `cach-long-giay-khen-vao-khung.html`
- [ ] khung bằng khen mica hay kính → `khung-bang-khen-mica-hay-kinh.html`
- [ ] khung giấy khen treo tường đẹp → `khung-giay-khen-treo-tuong-dep.html`
- [ ] khung bằng khen để bàn → `khung-bang-khen-de-ban.html`
- [ ] khung bằng khen tân phú tphcm → `khung-bang-khen-tan-phu-tphcm.html`
- [ ] cách treo nhiều khung bằng khen lên tường → `cach-treo-nhieu-khung-bang-khen.html`
- [ ] khung giấy phép kinh doanh a4 → `khung-giay-phep-kinh-doanh-a4.html`
- [ ] quà tặng khung bằng khen tri ân nhân viên → `khung-bang-khen-qua-tang-nhan-vien.html`
- [ ] cách bảo quản giấy khen không bị ố vàng → `cach-bao-quan-giay-khen.html`
- [ ] khung bằng khen tốt nghiệp → `khung-bang-khen-tot-nghiep.html`
- [ ] khung giấy khen giá sỉ → `khung-giay-khen-gia-si.html`
- [ ] khung bằng khen a4 giao hàng toàn quốc → `khung-bang-khen-a4-giao-toan-quoc.html`

Khi hết danh sách: thêm 10 từ khoá dài liên quan mới (không trùng ý bài cũ) rồi tiếp tục.

## Việc chủ shop nên làm (Claude không làm thay được)

- Google Search Console: gửi `sitemap.xml`, dùng "Kiểm tra URL" → "Yêu cầu lập chỉ mục" cho trang trụ cột.
- Tạo/cập nhật Google Business Profile (Google Maps) cho xưởng 85 Bác Ái, Tân Phú, gắn link website.
- Đăng link trang trụ cột lên Facebook, Zalo OA, YouTube (mô tả video), Shopee shop.
- Xin khách quen (trường học, công ty) đánh giá trên Google Maps.

## Nhật ký

- 2026-10-24: Đổi sanpham.html (bản trùng, canonical tên miền cũ) thành trang chuyển hướng về Chi-tiet-san-pham.html.
- 2026-10-24: Viết lại trang trụ cột (~350 → ~1.460 chữ), thêm 6 câu hỏi thường gặp riêng
  về khung bằng khen A4 (kèm FAQ schema), thêm liên kết từ trang chủ, trang sản phẩm và bài A4.
