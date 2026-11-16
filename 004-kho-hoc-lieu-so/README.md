# 004 — Kho học liệu số

Nền tảng **kho học liệu số đa môn cho giáo viên tiểu học** tại Trường Tiểu học Huỳnh Ngọc Huệ: chọn **Môn → Lớp → Chủ đề → Bài** là có ngay ngân hàng câu hỏi bám sách giáo khoa Kết nối tri thức để dạy ngay trong tiết, kèm trò chơi theo bài cho học sinh. Một ứng dụng chung nạp được các gói môn học; dữ liệu được biên soạn và bổ sung dần theo từng khối.

**Mở ứng dụng:** mở tệp `index.html` trong thư mục này bằng trình duyệt, hoặc qua GitHub Pages của repo (mục `004-kho-hoc-lieu-so/`).

## Dữ liệu hiện có (bản phát hành 16/11/2026)

Tổng kho: **948 bài — 10.115 câu hỏi** ở đủ 7 môn:

| Môn | Khối có dữ liệu | Số câu |
|-----|------------------|--------|
| Toán | Lớp 1, 2, 3, 4, 5 | 3.077 |
| Tiếng Việt | Lớp 1, 2, 3, 4, 5 | 2.356 |
| Tiếng Anh | Lớp 3, 4, 5 | 2.352 |
| Tin học | Lớp 3, 4, 5 | 1.125 |
| Công nghệ | Lớp 3, 4, 5 | 467 |
| Khoa học | Lớp 4 | 350 |
| Lịch sử & Địa lí | Lớp 4 | 388 |

Mỗi câu hỏi có mức độ theo Thông tư 27 (Nhận biết / Kết nối / Vận dụng), lời giải thích hoặc đáp án mẫu (câu tự luận ngắn), yêu cầu cần đạt của bài và nguồn trang sách giáo khoa. Các môn/khối còn thiếu (Khoa học và Lịch sử & Địa lí Lớp 5…) sẽ được bổ sung trong các đợt cập nhật tiếp theo.

## Chức năng

- **Hồ sơ bài học:** xem toàn bộ câu hỏi của một bài kèm yêu cầu cần đạt; in hồ sơ bài dạng xem trước A4 trong trang.
- **Trình chiếu:** chiếu câu hỏi lên màn hình/máy chiếu để cả lớp cùng làm, có đồng hồ đếm ngược tùy chọn cho từng câu.
- **Luyện tập nhanh:** rút câu ngẫu nhiên theo bài/mức độ để ôn tập.
- **Đua điểm tổ:** trò chơi thi đua giữa các tổ trong lớp, tính điểm theo mức độ câu hỏi.
- **Mở ô bí mật:** trò chơi mở ô chọn câu hỏi, có ô ngôi sao may mắn cộng điểm.
- **Quản trị kho:** nạp/cập nhật thêm gói môn từ tệp; gói mới có phiên bản cao hơn sẽ tự thay gói cũ đang lưu trên máy.

## Nguyên tắc chuẩn

- **Bám sát văn bản:** nội dung câu hỏi bám chương trình GDPT 2018 (TT32), sách giáo khoa và sách giáo viên Kết nối tri thức; mức độ và cách dùng trong đánh giá theo TT27 và sửa đổi TT89; gắn khung năng lực số (TT02) và khung giáo dục AI (QĐ 2422) theo hướng dẫn 3456/5588.
- **Offline trước hết:** toàn bộ dữ liệu đi kèm trong ứng dụng, chạy được khi không có mạng tại phòng Tin; đồng bộ/sao lưu qua Drive và tệp USB theo cùng chuẩn các sản phẩm 001–003.
- **Mỗi môn một bản sắc:** mỗi môn có màu nhấn và bộ biểu tượng SVG riêng, giao diện phẳng, sinh động phù hợp trình chiếu trước học sinh tiểu học.

## Kỹ thuật

Một tệp HTML duy nhất, không phụ thuộc thư viện ngoài, mở được trên mọi trình duyệt hiện đại, kể cả khi không có mạng. Font thân bài Segoe UI; tên trường và tiêu đề sản phẩm theo chuẩn thương hiệu chung của nhà tule-muse.

## Nhật ký cập nhật

- **16/11/2026 — v1.0:** phát hành bản đầu tiên lên tule-muse: nền tảng kho học liệu số với 7 môn, 948 bài, 10.115 câu hỏi. Dữ liệu gồm ngân hàng Tin học 3–5 (1.125 câu, từ sản phẩm 002) và các gói Toán, Tiếng Việt, Tiếng Anh, Công nghệ, Khoa học, Lịch sử & Địa lí do giáo viên tổng hợp theo sách Kết nối tri thức cho Lớp 1–5. Đủ Trình chiếu, Luyện tập nhanh, Đua điểm tổ, Mở ô bí mật, đồng hồ đếm ngược và in hồ sơ bài học.
