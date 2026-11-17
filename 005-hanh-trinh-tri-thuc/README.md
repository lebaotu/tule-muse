# 005 — Hành trình tri thức

Trò chơi bản đồ dài kỳ cho học sinh tiểu học: cả lớp (hoặc từng tổ) cùng đi một hành trình trên **Đảo tri thức**, trong đó mỗi **bài học là một chặng**, hết một **chủ đề là một Cổng ôn tập** phải vượt qua mới đi tiếp. Tiến trình được lưu theo lớp/tổ và chơi tích lũy xuyên nhiều tuần — khác với các ván lẻ trong 004.

🔗 **Dùng ngay:** https://lebaotu.github.io/tule-muse/005-hanh-trinh-tri-thuc/

## Dữ liệu

Dùng nguyên nền ngân hàng câu hỏi của **004 — Kho học liệu số**: 7 môn (Toán, Tiếng Việt, Tiếng Anh, Tin học, Công nghệ, Khoa học, Lịch sử & Địa lí), **1.006 bài, 10.858 câu hỏi** bám SGK Kết nối tri thức và chương trình TT32; mức độ theo TT27 (Nhận biết / Kết nối / Vận dụng). Khoa học và Lịch sử & Địa lí chỉ có Lớp 4–5.

## Cách chơi

- Tạo hành trình: đặt tên lớp → chọn Môn → chọn Lớp → chọn chế độ **Cả lớp** hoặc **Đối kháng tổ** (2–6 tổ, mỗi tổ một lá cờ màu riêng, đi luân phiên).
- Mỗi chặng rút câu hỏi từ đúng bài học đó (mặc định 6 câu, khó dần; có lời giải thích sau mỗi câu; đồng hồ đếm ngược tùy chọn). Đúng từ 2/3 số câu là qua chặng, nhận 1–3 sao theo tỉ lệ đúng; chơi lại để nâng sao.
- Có **chặng thử thách** (chỉ câu Kết nối/Vận dụng, sao nhân đôi), **ô may mắn** tặng điểm thưởng, và **Cổng chủ đề** (10 câu trộn toàn chủ đề, qua cổng mở chủ đề tiếp theo).
- **17/11/2026 — v1.2.6:** cơ cấu LS&ĐL lớp 4 học kì II theo Kế hoạch môn học (CV 2345) như 004 v1.3.5: bản đồ đổi cấu trúc HKII, thêm chặng Bài 18, bỏ các chặng Tây Nguyên cũ; tổng kho 1.015 bài / 10.923 câu.
- **17/11/2026 — v1.2.5:** đợt hoàn thiện khối 4 như 004 v1.3.4: thêm 2 chặng Toán Bài 28 (tuần 14) và Bài 30 (tuần 14–15), bổ sung 23 lời giải thích; tổng kho 1.017 bài / 10.957 câu; tiến trình đã lưu giữ nguyên.
- **17/11/2026 — v1.2.4:** nạp dữ liệu khối 4 mới theo Kế hoạch môn học (CV 2345): thêm các chặng Ôn tập/Kiểm tra trên bản đồ, tuần của từng bài căn theo kế hoạch; tổng kho 1.015 bài / 10.939 câu; tiến trình đã lưu của người dùng được giữ nguyên.
- **Khóa chặng theo tuần học** (lịch năm học 2026–2027, 35 tuần, trừ 2 tuần Tết) — bật mặc định, tắt được trong Cài đặt.

## Sổ hành trình

Theo từng hành trình/lớp: phần trăm hoàn thành, tổng sao, bảng tỉ lệ đúng từng bài; bài dưới 60% được đánh dấu **"Bài yếu"** để giáo viên ôn lại — căn cứ cho đánh giá thường xuyên. Có bản in.

## Kỹ thuật

- Một tệp HTML duy nhất, **chạy hoàn toàn offline** (phòng Tin chưa có Internet), dung lượng ~2,8 MB.
- Tiến trình lưu trên máy; **xuất/nhập tệp tiến trình (JSON)** để mang qua USB giữa các máy.
- Chuẩn thương hiệu tule-muse: màn hình mở đầu với logo Trường Tiểu học Huỳnh Ngọc Huệ, ảnh minh họa 3D phong cách chung của nhà, icon SVG.

## Nhật ký cập nhật

- **17/11/2026 — v1.2.3:** nạp vá dữ liệu ngân hàng Tin học v5.1 — sửa đáp án câu Vận dụng Lớp 5 Bài 6 (M-20261113-VD-HKI-16) từ C sang D; hai câu trùng GROK-0338 (Lớp 4 Bài 6) và GROK-0613 (Lớp 5 Bài 6) gắn cờ "Cần sửa" nên bị loại khỏi các chặng và Cổng chủ đề; sửa chính tả "cầu vòng" thành "cầu vồng" (SEED-208); bổ sung lời giải thích cho 66 câu của 3 bài tuần 11 (Lớp 3 Bài 5, Lớp 4 Bài 6, Lớp 5 Bài 6). Tiến trình đã lưu của các lớp giữ nguyên.
- **16/11/2026 — v1.2.2:** sửa đúng gốc rễ lỗi hiển thị Cổng: nút Cổng mang lớp "cong" trong khi định dạng của các bản trước viết cho lớp "gate" nên đĩa cổng khóa chưa từng nhận nền vàng. Nay định dạng khớp đúng lớp "cong", đĩa cổng khóa phủ vàng đậm rõ hẳn (gắn cả nền vàng trực tiếp khi vẽ nút), đồng thời sửa cùng lỗi tên lớp cho ô may mắn.
- **16/11/2026 — v1.2.1:** vá hiển thị Cổng chủ đề trên bản đồ — trước đây cổng đang khóa bị lớp làm mờ/xám của trạng thái khóa phủ lên nên chỉ còn vòng tròn trắng mờ; nay cổng hiện khung vàng đúng thiết kế ở mọi trạng thái (vàng trầm + huy hiệu ổ khóa khi chưa mở, phát sáng mạnh khi đến lượt, vàng tươi khi đã qua).
- **16/11/2026 — v1.2:** gộp gói âm thanh và đợt tuốt giao diện chuẩn game. Âm thanh: nhạc nền không lời êm nhẹ lặp vòng (tổng hợp bằng WebAudio ngay trong ứng dụng, không thêm tệp nhạc, vẫn chạy offline), tiếng khi chọn chặng/chọn đáp án, giai điệu mừng khi đúng, tiếng trầm nhẹ khi sai, fanfare qua chặng và qua Cổng, chuông hết giờ, tiếng leng keng ô may mắn; nút loa tắt/mở nhanh trên mọi màn hình và mục Âm thanh trong Cài đặt (bật/tắt nhạc nền, bật/tắt hiệu ứng, chỉnh âm lượng). Giao diện: màn mở đầu thành bìa game (ảnh xuất phát khung vàng, sao bay, tiêu đề font Baloo 2 nổi khối, nút bắt đầu phát sáng); Cổng chủ đề khung vàng phát sáng, ô may mắn lấp lánh, chặng hiện tại nhấp nháy hào quang; màn chơi thành sân khấu game show (đáp án đúng nảy sáng xanh, sai rung nhẹ, đồng hồ nhấp nháy đỏ khi sắp hết giờ); màn kết quả sao bay từng ngôi, qua Cổng có cúp vàng và pháo giấy dày.
- **16/11/2026 — v1.0.1:** minh bạch điểm số — màn kết quả mỗi chặng tách rõ điểm câu đúng (×10), điểm thưởng sao (×5) và điểm ô may mắn (+30), kèm dòng công thức tính điểm dưới bản đồ và chi tiết điểm trong Sổ hành trình; sửa nhãn chủ đề trên bản đồ bị cắt mép ở hai phía (nhãn dài nay được kẹp trọn trong khung bản đồ).
- **16/11/2026 — v1.0:** phát hành bản đầu: bản đồ Đảo tri thức sinh tự động theo từng Môn + Lớp từ ngân hàng của 004; 2 chế độ Cả lớp / Đối kháng tổ; chặng, chặng thử thách, ô may mắn, Cổng chủ đề; sao và điểm hành trình; Sổ hành trình theo lớp; khóa chặng theo tuần; xuất/nhập tiến trình.
