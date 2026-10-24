# SEO tự động - hàng đợi từ khoá (3 bài/tuần: thứ 2, 4, 6)

Website: https://khungtranhgiare.com (repo nghiemannam/khungtranhgiare, nhánh main).
Nhóm "khung bằng khen A4" đã chuyển vào hàng đợi này (file seo/ke-hoach-khung-bang-khen-a4.md ngừng dùng từ 24/10/2026).
Không viết trùng chủ đề với bài đã có trong bai-viet/.

## Quy tắc mỗi lần chạy

1. `git pull origin main`. Lấy chủ đề đầu tiên còn `[ ]` trong "Hàng đợi".
2. Viết 1 bài mới `bai-viet/<slug>.html`:
   - Mẫu giao diện: nhóm "Cho thuê" copy `bai-viet/thue-gia-do-poster-su-kien.html` (giữ hỏi đáp về thuê giá vẽ);
     nhóm khác copy `bai-viet/gia-ve-khung-go-150cm.html` (giữ hỏi đáp chung). Chỉ thay khối `<article class="nkt-bv">`, title, meta, canonical, og:*, JSON-LD Article + BreadcrumbList.
   - Từ khoá chính = tên bài, có trong title, H1, đoạn đầu (in đậm), 1 thẻ H2.
   - Title ≤ 60 ký tự. Meta description 140-160 ký tự. 1 H1, 3-5 H2 (có thể thêm H3). Thân bài 300-500 chữ.
   - Đúng 5 link trong thân bài, link đầy đủ `https://khungtranhgiare.com/...`:
     (1) trang chủ, anchor "Nam Khung Tranh"; (2) trang/bài chính của nhóm; (3) 1 sản phẩm liên quan trên `Chi-tiet-san-pham.html#<id>`;
     (4) danh mục trên `Chi-tiet-san-pham.html#<id-danh-muc>`; (5) 1 bài viết cùng nhóm đã có.
   - Khối "Bài viết liên quan" đúng 3 bài khác, không trùng link trong thân bài. 5-8 hashtag.
   - Ảnh: chỉ dùng ảnh có sẵn trong `hinh-webp/` hoặc `hinh-anh/`, alt mô tả đúng ảnh.
   - SỰ THẬT: chỉ lấy thông tin sản phẩm, giá, chính sách từ `Chi-tiet-san-pham.html`, `chinhsach.html`, các bài đã có.
     Không bịa giá, số liệu, đánh giá, chứng nhận. Dịch vụ thuê: giá vẽ gỗ thông mộc 1m3, 1m5, không cọc, vận chuyển 1-2 chiều tính phí riêng, giao lắp tận nơi, giá thuê báo theo đơn.
   - Xưng hô với khách: "bạn". Hotline/Zalo duy nhất: 0979.569.915.
3. Thêm thẻ bài vào đầu `<div class="nkt-bl-grid">` của `bai-viet-moi.html` + cập nhật JSON-LD ItemList. Thêm URL vào `sitemap.xml`.
4. Link ngược: sửa 1 bài cùng nhóm cũ nhất chưa trỏ tới bài mới - thay 1 mục trong "Bài viết liên quan" bằng bài mới (vẫn đúng 3 mục).
5. Kiểm tra: mọi JSON-LD parse được; mọi link nội bộ trỏ tới file và id có thật; trang mới hiển thị tốt ở 390px (Playwright).
6. Đánh dấu `[x]` + ngày, ghi 1 dòng "Nhật ký". Commit tiếng Việt, `git push origin HEAD:main`.
7. Cứ lần chạy thứ 6, 12, 18...: không viết bài mới mà rà toàn web (link hỏng, ảnh thiếu, title/description trùng) và sửa lỗi.

## Hàng đợi

### Nhóm Cho thuê giá vẽ (bài chính: bai-viet/cho-thue-gia-ve-tranh-tphcm.html, bai-viet/cho-thue-gia-ve-su-kien-trien-lam-tphcm.html)
- [ ] cho-thue-gia-ve-quan-1-binh-thanh | cho thuê giá vẽ quận 1, Bình Thạnh
- [ ] thue-gia-ve-khai-truong-cua-hang | thuê giá vẽ khai trương cửa hàng
- [ ] thue-gia-ve-le-tot-nghiep | thuê giá vẽ lễ tốt nghiệp, sự kiện trường học
- [ ] checklist-thue-gia-ve-su-kien | checklist chuẩn bị thuê giá vẽ sự kiện

### Nhóm Khung bằng khen A4 (bài chính: bai-viet/khung-bang-khen-a4.html, danh mục #khung-hinh-khung-anh)
- [ ] khung-giay-khen-a4-cho-hoc-sinh | khung giấy khen A4 cho học sinh
- [ ] kich-thuoc-khung-bang-khen-a4 | kích thước khung bằng khen A4
- [ ] khung-bang-khen-21x30 | khung bằng khen 21x30
- [ ] khung-bang-khen-so-luong-lon-truong-hoc | mua khung bằng khen số lượng lớn cho trường học
- [ ] khung-chung-nhan-a4-doanh-nghiep | khung chứng nhận A4 cho doanh nghiệp
- [ ] cach-long-giay-khen-vao-khung | cách lồng giấy khen vào khung
- [ ] khung-bang-khen-mica-hay-kinh | khung bằng khen mica hay kính
- [ ] khung-giay-khen-treo-tuong-dep | khung giấy khen treo tường đẹp
- [ ] khung-bang-khen-de-ban | khung bằng khen để bàn
- [ ] khung-bang-khen-tan-phu-tphcm | khung bằng khen Tân Phú TPHCM
- [ ] cach-treo-nhieu-khung-bang-khen | cách treo nhiều khung bằng khen lên tường
- [ ] khung-giay-phep-kinh-doanh-a4 | khung giấy phép kinh doanh A4
- [ ] khung-bang-khen-qua-tang-nhan-vien | quà tặng khung bằng khen tri ân nhân viên
- [ ] cach-bao-quan-giay-khen | cách bảo quản giấy khen không bị ố vàng
- [ ] khung-bang-khen-tot-nghiep | khung bằng khen tốt nghiệp

### Nhóm Khung hình - khung ảnh (danh mục #khung-hinh-khung-anh)
- [ ] cach-treo-khung-anh-len-tuong | cách treo khung ảnh lên tường
- [ ] khung-anh-treo-tuong-phong-khach | khung ảnh treo tường phòng khách
- [ ] kich-thuoc-khung-anh-pho-bien | kích thước khung ảnh phổ biến
- [ ] khung-anh-mica-de-ban-lam-qua | khung ảnh mica để bàn làm quà tặng
- [ ] cach-dong-khung-ao-bong-da | cách đóng khung áo bóng đá (danh mục #khung-ao-dau-danh-muc)

### Nhóm Giá vẽ tranh - bán (danh mục #gia-ve-tranh)
- [ ] gia-ve-tranh-loai-nao-tot | giá vẽ tranh loại nào tốt
- [ ] gia-ve-cho-nguoi-moi-hoc-ve | giá vẽ cho người mới học vẽ
- [ ] gia-ve-mini-de-ban-trang-tri | giá vẽ mini để bàn trang trí
- [ ] gia-ve-trung-bay-cua-hang | giá vẽ trưng bày cửa hàng

### Nhóm Phụ kiện, vật tư làm khung (danh mục #phu-kien-khung-tranh, #dung-cu-vat-tu)
- [ ] dung-cu-lam-khung-tranh-can-co | dụng cụ làm khung tranh cần có
- [ ] cach-chon-moc-treo-tranh | cách chọn móc treo tranh
- [ ] dinh-v7-va-v10-khac-nhau | đinh V7 và V10 khác nhau thế nào
- [ ] chan-chong-khung-anh-chon-so-may | chân chống khung ảnh chọn số mấy
- [ ] cach-ghep-goc-khung-tranh | cách ghép góc khung tranh

### Nhóm Tranh treo tường (danh mục #tranh-treo-tuong)
- [ ] y-nghia-tranh-phat-a-di-da | ý nghĩa tranh Phật A Di Đà
- [ ] vi-tri-treo-tranh-phat-trong-nha | vị trí treo tranh Phật trong nhà
- [ ] tranh-cong-giao-treo-phong-khach | tranh Công giáo treo phòng khách
- [ ] qua-tang-giang-sinh-tranh-chua | quà tặng Giáng Sinh: tranh Chúa, tranh Đức Mẹ

## Nhật ký
| Ngày | Bài | Ghi chú |
|---|---|---|
