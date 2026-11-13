# 002 — Ngân hàng câu hỏi & Trộn đề Tin học 3–5

Ứng dụng web xây dựng **ngân hàng câu hỏi trắc nghiệm Tin học lớp 3–5** (sách Kết nối tri thức với cuộc sống) theo từng bài học và **trộn đề ngẫu nhiên** thành nhiều mã đề cho các lớp — dùng cho luyện tập giữa kỳ (không chấm điểm) và ra đề kiểm tra cuối kỳ I / cuối năm (chấm điểm, theo ma trận) tại Trường Tiểu học Huỳnh Ngọc Huệ.

**Mở ứng dụng:** mở tệp `index.html` trong thư mục này bằng trình duyệt, hoặc qua GitHub Pages của repo (mục `002-ngan-hang-cau-hoi/`).

## Chức năng

- **Tổng quan:** thống kê kho câu hỏi (tổng số câu, đã duyệt / chờ duyệt, theo khối), lối tắt vào các chức năng chính.
- **Ngân hàng câu hỏi:** lọc theo khối, bài học, mức độ (Nhận biết / Kết nối / Vận dụng), trạng thái duyệt và tìm kiếm; mỗi câu có đáp án, lời giải thích, yêu cầu cần đạt và nguồn soạn; duyệt câu, đánh dấu cần sửa, thêm / sửa / xóa câu hỏi.
- **Trộn đề:** hai hình thức — luyện tập giữa kỳ (không chấm điểm, hiện đáp án + giải thích) và đề kiểm tra (chỉ dùng câu **đã duyệt**, theo tỉ lệ mức độ 50/30/20, thang điểm 10). Phạm vi theo đợt (giữa HKI đến tuần 10, cuối HKI đến tuần 18, giữa HKII đến tuần 27, cuối năm đến tuần 35) hoặc tự chọn bài. Mỗi lớp một mã đề riêng, thứ tự câu và thứ tự đáp án được xáo trộn ngẫu nhiên, đáp án tính lại đúng theo vị trí sau trộn.
- **Bộ đề đã tạo:** lưu trữ các mã đề đã sinh, mở xem lại, in lại.
- **In hồ sơ đề:** bản học sinh (đề bài, không đáp án, đầu đề theo thể thức văn bản trường) và bản giáo viên (đáp án từng mã đề, ma trận đề, bảng đối chiếu câu ↔ bài học ↔ yêu cầu cần đạt ↔ mức độ) để tổ trưởng và ban giám hiệu kiểm tra.
- **Cài đặt & dữ liệu:** khóa mã PIN, nạp / xuất gói ngân hàng câu hỏi dạng JSON, sao lưu / khôi phục qua USB, đồng bộ tự động qua Apps Script (mã mẫu dán-là-chạy kèm trong ứng dụng).

## Nguyên tắc chất lượng

- **AI soạn — thầy duyệt:** câu hỏi do AI soạn bám SGK/SGV/KHDH đều vào kho với trạng thái *Chờ duyệt*; chỉ câu đã được giáo viên duyệt mới được vào đề kiểm tra chấm điểm.
- **Nguồn chuẩn:** Chương trình GDPT 2018 môn Tin học (TT32) → SGK/SGV Tin học Kết nối tri thức → Kế hoạch dạy học của giáo viên; đánh giá theo TT27 và TT89/2026.
- **Offline trước hết:** chạy hoàn toàn không cần mạng tại phòng Tin; dữ liệu lưu trên thiết bị; đồng bộ Drive chỉ thực hiện khi có mạng.

## Kỹ thuật

Một tệp HTML duy nhất, không phụ thuộc thư viện ngoài, mở được trên mọi trình duyệt hiện đại, kể cả khi không có mạng.

## Nhật ký cập nhật

- **13/11/2026 — v1.2:** câu hỏi Muse phát hành lên kho trực tuyến được coi là **đã duyệt sẵn** — giáo viên không cần bấm duyệt từng câu, chỉ đánh dấu "Cần sửa" khi phát hiện câu chưa đúng; quy tắc hợp nhất mới cho trạng thái duyệt và mức độ từ kho trực tuyến chảy xuống các câu chưa sửa tay trên máy, không bao giờ ghi đè câu đã duyệt / đã sửa tay / đang cần sửa. Tổng quan có dòng trạng thái ngân hàng trực tuyến luôn hiển thị. Ngân hàng đồng thời lên **272 câu** (222 câu sẵn có đã được Muse phân loại mức độ theo TT27 + 50 câu Muse soạn mới), tất cả ở trạng thái đã duyệt.
- **13/11/2026 — v1.1:** ứng dụng **tự tải toàn bộ ngân hàng câu hỏi** từ tệp `ngan-hang-cau-hoi.json` trên chính repo này mỗi lần mở (khi có mạng) và hợp nhất thông minh vào kho trên thiết bị — không cần nạp tệp thủ công nữa; câu đã duyệt / đã sửa tay không bao giờ bị ghi đè; không có mạng (phòng Tin) thì dùng bản đã lưu trên máy. Thêm nút "Cập nhật ngân hàng trực tuyến" trong Cài đặt và dòng hướng dẫn thân thiện ở các bài chưa có câu hỏi.
- **13/11/2026 — v1.0:** phát hành bản đầu tiên lên tule-muse: giao diện phong cách "phòng lab số / bảng mạch điện tử" hoàn toàn mới, bộ icon SVG công nghệ riêng; đủ 5 màn hình; kho nạp sẵn 21 câu mẫu Lớp 3 Bài 1 (6 câu từ ngân hàng sẵn có của thầy + 15 câu Muse soạn có mức độ, yêu cầu cần đạt, lời giải thích — đều ở trạng thái chờ duyệt); trộn mã đề ngẫu nhiên đã kiểm thử 300 lần trộn không lỗi đáp án; kèm gói nạp mở rộng 237 câu hỏi.
