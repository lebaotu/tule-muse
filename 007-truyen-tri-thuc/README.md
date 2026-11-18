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

- **17/11/2026 — v1.4:** khép TOÁN LỚP 4 TRỌN NĂM — thêm 10 mùa học kỳ 2 (cụm 13–22, Bài 38–73), tổng Toán 4 đủ 22 mùa/95 tập, tổng app 71 mùa; 6 ảnh bìa mới (lâu đài hai chữ số, vườn biểu đồ cột, vương quốc phân số, cân phân số, sông phân số, cỗ máy phân số) ở chunk ảnh 21, bản đồ ảnh 86 khóa; soạn bổ sung 26 câu cho các bài mỏng HK2 (Bài 47 +4, 43/44 +3, 55 +3, 54/49 +2... — nguồn ghi rõ chờ thầy duyệt, chỉ dùng trong 007); vá lỗi tiềm ẩn từ thời Toán 3: bước câu cứu viện có thể rút trúng câu tự luận không có phương án làm văng bước — bộ rút câu nay chỉ rút câu trắc nghiệm có phương án.

- **17/11/2026 — v1.5:** mở TOÁN LỚP 5 học kỳ 1 — 12 mùa, 47 tập theo kế hoạch cả năm 24 cụm/75 bài (Vùng Đất Cuối của Vương quốc Số Học, nơi đặt Cánh Cổng Đêm Chung Kết); 2 ảnh bìa mới (làng hỗn số, cổng số thập phân) ở chunk ảnh 22, bản đồ ảnh 88 khóa; soạn bổ sung 55 câu cho các bài mỏng HK1 (Bài 5/10/23/26/32 +5, Bài 8/25/27/33 +4, Bài 28 +4... — nguồn ghi rõ chờ thầy duyệt, chỉ dùng trong 007). Tổng app: 83 mùa.

- **18/11/2026 — v1.6:** khép TOÁN LỚP 5 TRỌN NĂM — thêm 12 mùa học kỳ 2 (cụm 13–24, Bài 36–75), tổng Toán 5 đủ 24 mùa/99 tập, tổng app 95 mùa/369 tập; 8 ảnh bìa mới (thung lũng tỉ số, cân tỉ số phần trăm, tháp máy tính cầm tay, hang khối thể tích, xưởng gấp hình khối, hồ thể tích, vườn biểu đồ quạt, đại sảnh tổng ôn) ở chunk ảnh 23, bản đồ ảnh 96 khóa; rà soát độc lập từng bài HK2 rồi soạn bổ sung 64 câu cho 34 bài mỏng (Bài 52 mỏng nhất chỉ 5 câu → +4; Bài 48/53/62/72 hết lặp câu) — nguồn ghi rõ chờ thầy duyệt, chỉ dùng trong 007.

- **18/11/2026 — v1.7:** mở TOÁN LỚP 1 học kỳ 1 — 8 mùa, 28 tập theo kế hoạch cả năm 18 cụm/41 bài (Vùng Đất Khởi Đầu của Vương quốc Số Học; truyện ngắn gọn, không câu mức khó, tình huống đếm đồ vật gần gũi trẻ nhỏ); 1 ảnh bìa mới (khu vườn số đếm) ở chunk ảnh 24, bản đồ ảnh 97 khóa; soạn bổ sung 24 câu cho các bài vừa khít (Bài 3/8/9/16/19 +2 mức 1, Bài 13 +3 mức 2...) — nguồn ghi rõ chờ thầy duyệt, chỉ dùng trong 007. Tổng app: 103 mùa.

- **18/11/2026 — v1.8:** TOÁN LỚP 1 TRỌN NĂM — nạp học kỳ 2 (cụm 9–18, 31 tập), Toán 1 đủ 18 mùa/59 tập; bổ sung 22 câu cho các bài vừa khít của HK2 (Bài 21 +2 mức 2, Bài 33 +2 mức 1...), gói Toán 1 trong app 391 câu. MỚI: cỡ chữ TO riêng cho lớp 1–2 trong màn chơi truyện (tăng 20 phần trăm: thoại 22,2px, câu hỏi 23,4px, nhãn đáp án 18px), lớp 3–5 giữ nguyên. Tổng app: 113 mùa.

- **18/11/2026 — v1.9:** mở TOÁN LỚP 2 học kỳ 1 — 10 mùa, 45 tập (kế hoạch cả năm 23 cụm/75 bài); 4 ảnh bìa mới (cầu cộng qua mười, cầu trừ qua mười, đồi cộng có nhớ, đồi trừ có nhớ) ở chunk ảnh 25, bản đồ ảnh 101 khóa; bổ sung 19 câu cho các bài vừa khít của HK1 lớp 2 (Bài 32 +2 mức 1, Bài 5/6/14/33 +2 mức 2...) — tỉ lệ lượt chơi bị ép lặp câu giảm từ 3,2% xuống 0,28%; cỡ chữ to lớp 1–2 đã kiểm chứng chạy thật cho cả lớp 2. Tổng app: 123 mùa.

- **18/11/2026 — v1.10:** TOÁN LỚP 2 TRỌN NĂM — nạp học kỳ 2 (cụm 11–23, 53 tập), Toán 2 đủ 23 mùa/98 tập; VƯƠNG QUỐC SỐ HỌC KHÉP ĐỦ 5 LỚP (114 mùa Toán). 3 ảnh bìa mới (tháp số ba chữ số, chợ đo và tiền, thung lũng ngàn số) ở chunk ảnh 26, bản đồ ảnh 104 khóa; bổ sung 32 câu cho các bài mỏng HK2 lớp 2, gói Toán 2 trong app 645 câu; mô phỏng 39.200 lượt chơi toàn bộ Toán 2: 0 hụt, 0 lặp, 0 nới mức. Tổng app: 136 mùa.

- **18/11/2026 — v1.11:** mở THẾ GIỚI TIẾNG VIỆT — KHU VƯỜN NGÔN TỪ (Cô Ong Chăm Chữ dẫn truyện; 4 sân khấu Cây quả chữ, Cầu vần thơ, Dòng suối câu, Hòm thư bí mật) với TIẾNG VIỆT LỚP 3 học kỳ 1: 9 mùa, 43 tập; 9 ảnh bìa mới ở chunk ảnh 27, bản đồ ảnh 113 khóa; gói Tiếng Việt 3 trong app 795 câu (kèm 3 câu bổ sung). Tổng app: 145 mùa. LƯU Ý KỸ THUẬT: tệp app đã ~4,25 MB, gần trần đẩy 5 MB — đợt kế tiếp sẽ tách các gói câu hỏi thành tệp riêng cạnh app như đã làm với ảnh, để thư viện lớn tiếp mà không đụng trần.

- **18/11/2026 — v1.12 (bản bảo trì kiến trúc, nội dung không đổi):** TÁCH TOÀN BỘ GÓI DỮ LIỆU ra thư mục goi/ cạnh app — 9 tệp gói theo môn–lớp (goi-tin-3/4/5, goi-toan-1…5, goi-tieng-viet-3; tổng ~3,96 MB, 145 mùa/569 tập/5.281 câu), nạp lười theo lớp đang mở kèm tem phiên bản, lỗi nạp có nút thử lại. Vỏ app giảm từ 4,38 MB xuống ~0,52 MB. Đã đối chiếu băm SHA-256: dữ liệu tách ra khớp tuyệt đối với bản v1.11; mô phỏng 170.700 lượt chơi trên dữ liệu đã tách: 0 hụt, 0 lặp; chơi thử thật cả 3 thế giới đạt. Kiến trúc này cho phép thư viện lớn tiếp qua 4 thế giới còn lại mà không đụng trần tệp.

- **18/11/2026 — v1.13:** Tiếng Việt lớp 3 TRỌN NĂM trên kiến trúc tách gói — nạp thêm 9 mùa học kỳ 2 (cụm 10–18), Khu Vườn Ngôn Từ lớp 3 đủ 18 mùa/84 tập; thư viện 154 mùa/610 tập. 8 bìa mới (chunk anh-28; bản đồ ảnh 121 khóa; cụm 14 dùng lại bìa vuon-on-tap); 7 câu bổ sung mức 2 cho Bài 43/51/53 (đếm lại độc lập: hai bài mức 2 trống hẳn, một bài chỉ 1 câu) — gói Tiếng Việt 3 nay 802 câu. Mô phỏng 252.000 lượt trên gói mới: 0 hụt, 0 lặp, 0 phải nới mức; phần HK1 đối chiếu băm khớp tuyệt đối với bản đang sống.
