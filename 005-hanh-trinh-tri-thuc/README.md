# 005 — Hành trình tri thức

Trò chơi bản đồ dài kỳ cho học sinh tiểu học: cả lớp (hoặc từng tổ) cùng đi một hành trình trên **Đảo tri thức**, trong đó mỗi **bài học là một chặng**, hết một **chủ đề là một Cổng ôn tập** phải vượt qua mới đi tiếp. Tiến trình được lưu theo lớp/tổ và chơi tích lũy xuyên nhiều tuần — khác với các ván lẻ trong 004.

🔗 **Dùng ngay:** https://lebaotu.github.io/tule-muse/005-hanh-trinh-tri-thuc/

## Dữ liệu

Dùng nguyên nền ngân hàng câu hỏi của **004 — Kho học liệu số**: 7 môn (Toán, Tiếng Việt, Tiếng Anh, Tin học, Công nghệ, Khoa học, Lịch sử & Địa lí), **1.006 bài, 10.858 câu hỏi** bám SGK Kết nối tri thức và chương trình TT32; mức độ theo TT27 (Nhận biết / Kết nối / Vận dụng). Khoa học và Lịch sử & Địa lí chỉ có Lớp 4–5.

## Cách chơi

- Tạo hành trình: đặt tên lớp → chọn Môn → chọn Lớp → chọn chế độ **Cả lớp** hoặc **Đối kháng tổ** (2–6 tổ, mỗi tổ một lá cờ màu riêng, đi luân phiên).
- Mỗi chặng rút câu hỏi từ đúng bài học đó (mặc định 6 câu, khó dần; có lời giải thích sau mỗi câu; đồng hồ đếm ngược tùy chọn). Đúng từ 2/3 số câu là qua chặng, nhận 1–3 sao theo tỉ lệ đúng; chơi lại để nâng sao.
- Có **chặng thử thách** (chỉ câu Kết nối/Vận dụng, sao nhân đôi), **ô may mắn** tặng điểm thưởng, và **Cổng chủ đề** (10 câu trộn toàn chủ đề, qua cổng mở chủ đề tiếp theo).
- **Khóa chặng theo tuần học** (lịch năm học 2026–2027, 35 tuần, trừ 2 tuần Tết) — bật mặc định, tắt được trong Cài đặt.

## Sổ hành trình

Theo từng hành trình/lớp: phần trăm hoàn thành, tổng sao, bảng tỉ lệ đúng từng bài; bài dưới 60% được đánh dấu **"Bài yếu"** để giáo viên ôn lại — căn cứ cho đánh giá thường xuyên. Có bản in.

## Kỹ thuật

- Một tệp HTML duy nhất, **chạy hoàn toàn offline** (phòng Tin chưa có Internet), dung lượng ~2,8 MB.
- Tiến trình lưu trên máy; **xuất/nhập tệp tiến trình (JSON)** để mang qua USB giữa các máy.
- Chuẩn thương hiệu tule-muse: màn hình mở đầu với logo Trường Tiểu học Huỳnh Ngọc Huệ, ảnh minh họa 3D phong cách chung của nhà, icon SVG.

## Nhật ký cập nhật

- **16/11/2026 — v1.0.1:** minh bạch điểm số — màn kết quả mỗi chặng tách rõ điểm câu đúng (×10), điểm thưởng sao (×5) và điểm ô may mắn (+30), kèm dòng công thức tính điểm dưới bản đồ và chi tiết điểm trong Sổ hành trình; sửa nhãn chủ đề trên bản đồ bị cắt mép ở hai phía (nhãn dài nay được kẹp trọn trong khung bản đồ).
- **16/11/2026 — v1.0:** phát hành bản đầu: bản đồ Đảo tri thức sinh tự động theo từng Môn + Lớp từ ngân hàng của 004; 2 chế độ Cả lớp / Đối kháng tổ; chặng, chặng thử thách, ô may mắn, Cổng chủ đề; sao và điểm hành trình; Sổ hành trình theo lớp; khóa chặng theo tuần; xuất/nhập tiến trình.
