# 004 — Kho học liệu số

Nền tảng **kho học liệu số đa môn cho giáo viên tiểu học** tại Trường Tiểu học Huỳnh Ngọc Huệ: chọn **Môn → Lớp → Chủ đề → Bài** là có ngay ngân hàng câu hỏi bám sách giáo khoa Kết nối tri thức để dạy ngay trong tiết, kèm trò chơi theo bài cho học sinh. Một ứng dụng chung nạp được các gói môn học; dữ liệu được biên soạn và bổ sung dần theo từng khối.

**Mở ứng dụng:** mở tệp `index.html` trong thư mục này bằng trình duyệt, hoặc qua GitHub Pages của repo (mục `004-kho-hoc-lieu-so/`).

## Dữ liệu hiện có (bản phát hành 16/11/2026)

Tổng kho: **1.006 bài — 10.858 câu hỏi** ở đủ 7 môn:

| Môn | Khối có dữ liệu | Số câu |
|-----|------------------|--------|
| Toán | Lớp 1, 2, 3, 4, 5 | 3.077 |
| Tiếng Việt | Lớp 1, 2, 3, 4, 5 | 2.356 |
| Tiếng Anh | Lớp 3, 4, 5 | 2.352 |
| Tin học | Lớp 3, 4, 5 | 1.125 |
| Công nghệ | Lớp 3, 4, 5 | 467 |
| Khoa học | Lớp 4, 5 | 708 |
| Lịch sử & Địa lí | Lớp 4, 5 | 773 |

Mỗi câu hỏi có mức độ theo Thông tư 27 (Nhận biết / Kết nối / Vận dụng), lời giải thích hoặc đáp án mẫu (câu tự luận ngắn), yêu cầu cần đạt của bài và nguồn trang sách giáo khoa. Kho đã đầy đủ cho mọi môn ở đúng các khối lớp môn đó được dạy theo chương trình (Khoa học và Lịch sử & Địa lí chỉ học ở Lớp 4–5 nên ứng dụng chỉ hiện hai lớp này cho hai môn đó).

## Chức năng

- **17/11/2026 — v1.3.4:** đợt hoàn thiện khối 4: Toán thêm 18 câu cho Bài 28 và Bài 30 (Chủ đề 6, trước đây chưa có câu), bổ sung 23 lời giải thích còn thiếu (Toán 9, Tiếng Anh 14) — hai gói đạt 100% câu có giải thích; tổng kho 7 môn / 1.017 bài / 10.957 câu.
- **17/11/2026 — v1.3.3:** cập nhật toàn bộ dữ liệu khối 4 theo Kế hoạch môn học (CV 2345): thêm 81 câu ở các mục Ôn tập/Kiểm tra, căn lại tuần cho 1.092 câu, không đổi nội dung/đáp án/mức độ; tổng kho 7 môn / 1.015 bài / 10.939 câu.
- **Hồ sơ bài học:** xem toàn bộ câu hỏi của một bài kèm yêu cầu cần đạt; in hồ sơ bài dạng xem trước A4 trong trang.
- **Trình chiếu:** chiếu câu hỏi lên màn hình/máy chiếu để cả lớp cùng làm, có đồng hồ đếm ngược tùy chọn cho từng câu.
- **Luyện tập nhanh:** rút câu ngẫu nhiên theo bài/mức độ để ôn tập.
- **Sảnh trò chơi thống nhất:** chọn phạm vi (bài/chủ đề) → chọn trò chơi → chọn chế độ (Cả lớp / Đối kháng / Tiếp sức) → Bắt đầu; khi chơi theo tổ luôn có thanh điểm các tổ ở đầu màn hình, hộp câu hỏi lớn hiện đáp án kèm lời giải thích sau mỗi câu.
- **Đua điểm tổ:** trò chơi thi đua giữa các tổ trong lớp, tính điểm theo mức độ câu hỏi.
- **Mở ô bí mật:** trò chơi mở ô chọn câu hỏi, có ô ngôi sao may mắn cộng điểm.
- **Ai là triệu phú:** 12 câu khó dần theo mức độ, thang điểm, mốc an toàn, trợ giúp 50:50 và đổi câu.
- **Bingo tri thức:** mỗi tổ một thẻ 4×4 ô đáp án, chiếu câu lần lượt, tổ hoàn thành một hàng trước thắng.
- **Ô Ăn Quan tri thức:** trò chơi dân gian Ô Ăn Quan kết hợp câu hỏi — trả lời đúng mới được rải quân, ăn quan tính điểm, chơi 2–4 tổ.
- **Dạy tuần này:** Tổng quan tự tính tuần học theo lịch năm học và liệt kê các bài đúng tuần của từng môn/lớp, chạm là mở thẳng bài.
- **Tìm kiếm toàn kho:** tìm câu hỏi theo nội dung và tên bài trên cả 7 môn; mỗi câu có nút đánh dấu "Cần sửa" (loại khỏi luyện tập/trò chơi, xem lại trong Quản trị kho).
- **Quản trị kho:** nạp/cập nhật thêm gói môn từ tệp; gói mới có phiên bản cao hơn sẽ tự thay gói cũ đang lưu trên máy.
- **Ảnh bìa môn:** ứng dụng tự hiện ảnh bìa nếu có thư mục `covers/` đặt cạnh tệp `index.html` (tên tệp theo mã môn, ví dụ `covers/toan.jpg`); không có thì giữ thiết kế màu/icon mặc định.

## Nguyên tắc chuẩn

- **Bám sát văn bản:** nội dung câu hỏi bám chương trình GDPT 2018 (TT32), sách giáo khoa và sách giáo viên Kết nối tri thức; mức độ và cách dùng trong đánh giá theo TT27 và sửa đổi TT89; gắn khung năng lực số (TT02) và khung giáo dục AI (QĐ 2422) theo hướng dẫn 3456/5588.
- **Offline trước hết:** toàn bộ dữ liệu đi kèm trong ứng dụng, chạy được khi không có mạng tại phòng Tin; đồng bộ/sao lưu qua Drive và tệp USB theo cùng chuẩn các sản phẩm 001–003.
- **Mỗi môn một bản sắc:** mỗi môn có màu nhấn và bộ biểu tượng SVG riêng, giao diện phẳng, sinh động phù hợp trình chiếu trước học sinh tiểu học.

## Kỹ thuật

Một tệp HTML duy nhất, không phụ thuộc thư viện ngoài, mở được trên mọi trình duyệt hiện đại, kể cả khi không có mạng. Font thân bài Segoe UI; tên trường và tiêu đề sản phẩm theo chuẩn thương hiệu chung của nhà tule-muse.

## Nhật ký cập nhật

- **17/11/2026 — v1.3.2:** nạp vá dữ liệu ngân hàng Tin học v5.1 — sửa đáp án câu Vận dụng Lớp 5 Bài 6 (M-20261113-VD-HKI-16) từ C sang D; hai câu trùng GROK-0338 (Lớp 4 Bài 6) và GROK-0613 (Lớp 5 Bài 6) gắn cờ "Cần sửa" nên bị loại khỏi Trình chiếu, Luyện tập và trò chơi nhưng vẫn tra cứu được trong Hồ sơ bài; sửa chính tả "cầu vòng" thành "cầu vồng" (SEED-208); bổ sung lời giải thích cho 66 câu của 3 bài tuần 11 (Lớp 3 Bài 5, Lớp 4 Bài 6, Lớp 5 Bài 6) — cả 3 bài nay đủ 69/69 câu có giải thích. Đồng thời nén lại ảnh bìa và logo để tệp giữ dưới 4,5 MB.
- **16/11/2026 — v1.3.1:** thêm ảnh bìa hoạt cảnh học sinh cho 3 trò chơi còn lại (Đua điểm tổ, Mở ô bí mật, Bingo tri thức) — nhúng trong ứng dụng và hiện làm banner ở màn thiết lập của từng trò, đồng bộ với Ai là triệu phú; cả 4 trò chơi nay đều có bìa.

- **16/11/2026 — v1.3 (đợt hình ảnh):** nhúng thẳng 7 ảnh bìa môn (WebP) vào trong ứng dụng — hiện ở thẻ môn và đầu trang môn trên mọi bản (Pages, offline); trò "Ai là triệu phú" có hoạt cảnh học sinh trong trường quay làm nền + pháo giấy khi đạt mốc cao; gỡ bỏ trò "Ô Ăn Quan tri thức" (sảnh còn 4 trò). Dữ liệu giữ nguyên 1.006 bài / 10.858 câu.

- **16/11/2026 — v1.2.1:** sửa lỗi mục "Dạy tuần này" thiếu Lớp 3 môn Tin học: ghi đúng khoảng tuần cho cả 49 bài Tin học theo PPCT/KHDH của trường (trước đây chỉ ghi tuần bắt đầu nên bài nhiều tuần bị mất khỏi danh sách ở các tuần sau); bài tự chọn không thuộc kế hoạch dạy được ghi nhãn "Tự chọn".

- **16/11/2026 — v1.2 (bản hoàn thiện):** thêm mục Dạy tuần này; sảnh trò chơi thống nhất với 3 chế độ chơi; ba trò chơi mới — Ai là triệu phú, Bingo tri thức, Ô Ăn Quan tri thức; hộp câu hỏi hiện đáp án + lời giải thích sau mỗi câu; tìm kiếm toàn kho và đánh dấu "Cần sửa"; cơ chế ảnh bìa môn qua thư mục covers/ (7 ảnh bìa hoạt hình 3D đi kèm gói ZIP offline). Dữ liệu giữ nguyên 1.006 bài / 10.858 câu.

- **16/11/2026 — v1.1:** bổ sung Khoa học Lớp 5 (358 câu) và Lịch sử & Địa lí Lớp 5 (385 câu) — tổng kho 1.006 bài / 10.858 câu, đầy đủ mọi môn theo đúng khối lớp được dạy; sửa ma trận môn–lớp: Khoa học và Lịch sử & Địa lí chỉ hiện Lớp 4–5, bỏ hẳn Lớp 3 (lớp 3 không học hai môn này).

- **16/11/2026 — v1.0:** phát hành bản đầu tiên lên tule-muse: nền tảng kho học liệu số với 7 môn, 948 bài, 10.115 câu hỏi. Dữ liệu gồm ngân hàng Tin học 3–5 (1.125 câu, từ sản phẩm 002) và các gói Toán, Tiếng Việt, Tiếng Anh, Công nghệ, Khoa học, Lịch sử & Địa lí do giáo viên tổng hợp theo sách Kết nối tri thức cho Lớp 1–5. Đủ Trình chiếu, Luyện tập nhanh, Đua điểm tổ, Mở ô bí mật, đồng hồ đếm ngược và in hồ sơ bài học.
