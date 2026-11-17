# 007 — Truyện Tri Thức: Biệt đội Ánh Sao

Game nhập vai kể chuyện theo chương trình Tin học lớp 3–5 (sách Kết nối tri thức): học sinh không "trả lời câu hỏi" mà sống trong một bộ truyện dài kỳ — Thư viện Ánh Sao bị Sương Mù Quên Lãng xâm chiếm, và chỉ tri thức thật mới xua được sương. Mỗi cụm bài là một mùa truyện, mỗi bài là một tập có rẽ nhánh bỏ phiếu, thử thách hóa thân vào hình ảnh (đáp án là vật thể trong tranh để chạm vào), trả lời chưa đúng thì rẽ sang cảnh biến cố với câu cứu viện — không ai bị loại, không ngõ cụt.

**Tác giả:** Lê Bảo Tú — Giáo viên Tin học, Trường Tiểu học Huỳnh Ngọc Huệ.
**Bản trực tuyến:** https://lebaotu.github.io/tule-muse/007-truyen-tri-thuc/

## Nội dung
- Đủ 3 khối lớp 3–4–5: **22 cụm truyện · 71 tập · 284 thử thách**, bám SGK/KHDH Tin học Kết nối tri thức và ngân hàng 1.131 câu hỏi đã duyệt của sản phẩm 002 (kèm 9 câu mới về tạo bài trình chiếu bám SGK Tin học 4, trang 30–33).
- Hai chế độ: Cả lớp phiêu lưu chung và Đối kháng tổ (mỗi tổ điều khiển một anh hùng). Khóa mở tập theo tuần học (tắt được trong Cài đặt), tính sao và vật phẩm theo tập, tiến trình lưu theo lớp, xuất kết quả phiên theo định dạng dùng chung để sản phẩm 008 tổng hợp.

## Kiến trúc
- Sản phẩm có mạng trước (theo hướng mới từ 007): tệp app chính nhẹ (~0,95 MB); 53 ảnh minh họa 3D nằm trong thư mục con `anh/` thành 13 tệp nạp lười theo cảnh — mở tập nào mới tải ảnh của tập đó.
- Bản offline cho phòng Tin: chép nguyên thư mục này (index.html + thư mục anh/) vào USB là chạy, không cần sửa gì.

## Nhật ký cập nhật
- **17/11/2026 — v1.0:** phát hành bản đầu tiên — đủ truyện Tin học 3–5 (22 cụm, 71 tập), sân khấu thử thách hóa thân vào hình ảnh với cảnh đổi trạng thái (cửa đá đóng → mở, cầu sương, kho sách khôi phục), đấu trùm cuối mỗi cụm, xuất/nhập tiến trình và xuất kết quả phiên cho 008.

- **17/11/2026 — v1.0.1:** thay logo trường bằng bản sạch (đã xoá vòng trắng thừa quanh huy hiệu và gỡ vòng trắng do CSS tạo quanh logo ở màn hình mở đầu); logo hiển thị 104×104 px trực tiếp trên nền.

- **17/11/2026 — v1.1:** mở THẾ GIỚI TOÁN đầu tiên — Vương quốc Số Học cho Lớp 3 học kỳ 1: 13 mùa truyện, 55 tập, 220 thử thách hoá thân vào sân khấu Toán (bậc thang số, cân thăng bằng, tháp khối hình, đồng hồ cát), Cụ Rùa Số Học dẫn đường, tập trùm phá khiên sương ở Cổng Số Học; nạp gói Toán lớp 3 trọn 77 bài/807 câu. Thế giới Tin học giữ nguyên.

- **17/11/2026 — v1.1.1:** vá bìa 13 mùa Toán lớp 3 — mỗi mùa một ảnh bìa riêng (thêm 8 ảnh mới: vườn bảng nhân, mảnh ghép bí ẩn, xưởng hình học, cỗ máy nhân chia, bài toán hai bước, phòng đo lường, nhiệt kế khổng lồ, đêm hội ôn tập; chunk ảnh 16–17, bản đồ ảnh 67 khóa); sửa bộ nạp ảnh không còn chốt chết lỗi tải chunk (nguyên nhân Mùa 5/9 trống bìa trên bản v1.1).

- **17/11/2026 — v1.2:** hoàn thiện TOÁN LỚP 3 TRỌN NĂM HỌC — nạp 14 mùa học kỳ 2 (cụm 14–27: 49 tập, 196 thử thách + 35 câu cứu viện), sảnh Toán lớp 3 đủ 27 mùa/104 tập/416 thử thách; 8 ảnh bìa mới (đồng hồ La Mã, quảng trường diện tích, sông chia số, thành phố trăm ngàn, tháp đồng hồ tiền, đoàn tàu số, trạm thống kê, cổng cuối năm) ở chunk ảnh 18–19, bản đồ ảnh 75 khóa. Gói câu hỏi Toán 3 dùng chung từ v1.1.

- **17/11/2026 — v1.2.1:** gia cố bộ nạp ảnh — gắn tem phiên bản (?v= theo PHIEN_BAN) vào mọi địa chỉ tệp ảnh (anh-map.js và các chunk anh-<n>.js) để trình duyệt không dùng bản đệm cũ sau mỗi lần phát hành; gỡ chốt chết lỗi của napAnhMap (nạp bản đồ lỗi một lần thì lần sau tự thử lại, như tệp chunk ở v1.1.1). Không thêm nội dung, không đổi dữ liệu.

- **17/11/2026 — v1.3:** mở TOÁN LỚP 4 học kỳ 1 — 12 mùa truyện, 49 tập theo kế hoạch cả năm 22 cụm/73 bài; 5 ảnh bìa mới (vườn biểu thức, tháp đo góc, lâu đài lớp triệu, xưởng đo đạc, thành phố đường thẳng) ở chunk ảnh 20, bản đồ ảnh 80 khóa; soạn bổ sung 18 câu cho 3 bài mỏng của kho (Bài 9 +7, Bài 32 +6, Bài 35 +5 — ghi rõ nguồn chờ thầy duyệt, chỉ dùng trong 007). Tổng app: 61 mùa.
