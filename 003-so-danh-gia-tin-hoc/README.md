# 003 — Sổ đánh giá Tin học 3–5

Ứng dụng web **sổ đánh giá môn Tin học lớp 3–5** cho giáo viên bộ môn tại Trường Tiểu học Huỳnh Ngọc Huệ: quản lí 21 lớp (708 học sinh nạp sẵn), ghi nhận đánh giá thường xuyên trong tiết dạy, nhập điểm kiểm tra định kỳ, tổng hợp mức đánh giá theo quy định và xuất bảng tổng hợp nộp giáo viên chủ nhiệm / tổ chuyên môn / ban giám hiệu.

**Mở ứng dụng:** mở tệp `index.html` trong thư mục này bằng trình duyệt, hoặc qua GitHub Pages của repo (mục `003-so-danh-gia-tin-hoc/`).

## Chức năng

- **Tổng quan:** tiến độ ghi nhận theo kỳ hiện tại, các mốc năm học (giữa HKI tuần 10, cuối HKI tuần 18, giữa HKII tuần 27, cuối năm tuần 33), lớp dạy hôm nay theo thời khóa biểu nạp sẵn.
- **Lớp & học sinh:** danh sách 21 lớp với học sinh thật (chỉ họ tên + giới tính); tự nhập thêm từ tệp Excel/CSV, thêm/sửa/chuyển lớp, ghi diện hỗ trợ hòa nhập.
- **Ghi nhận thường xuyên:** ghi nhanh theo tiết/bài (tự gợi ý bài theo tuần PPCT kèm mã chỉ báo năng lực số trong kế hoạch dạy học), 5 nhóm quan sát — học tập, thực hành, nề nếp, tham gia phát biểu, hợp tác — mỗi ghi nhận là nhận xét, không dùng điểm số.
- **Điểm kiểm tra định kỳ:** thang điểm 10, số nguyên; nguồn điểm linh hoạt — nối từ sản phẩm 002 (kèm mã đề), nhập tay theo đề nguồn khác (ví dụ đề chung của Sở GDĐT cho khối 5), hoặc để trống; cảnh báo điểm bất thường so với đánh giá thường xuyên.
- **Tổng hợp & chốt sổ:** giữa kỳ tổng hợp bằng nhận xét quá trình kèm mức; cuối kỳ 3 mức Hoàn thành tốt / Hoàn thành / Chưa hoàn thành; cuối năm 4 mức theo Điều 9 TT27; gợi ý mức và nhận xét có lí do, giáo viên rà soát rồi chốt — chốt/mở khóa đều ghi vết đối soát phục vụ ký số Học bạ số; xuất Bảng tổng hợp (.xls) và CSV đối chiếu.
- **NLS & AI:** theo dõi biểu hiện theo 6 miền năng lực số (TT02) và 4 thành phần năng lực AI (QĐ 2422), tách bạch với hệ mã năng lực tin học của TT32.
- **Cài đặt & dữ liệu:** khóa mã PIN; mục **Thông tin** về tác giả kèm ảnh chân dung; sao lưu/khôi phục tệp qua USB; đồng bộ Drive qua Apps Script (mã mẫu dán-là-chạy kèm trong ứng dụng); **Chuyển năm học mới** — lưu trữ năm cũ chỉ-đọc, học sinh khối 3–4 tự lên khối 4–5, khối 5 khép sổ hoàn thành/chuyển cấp, khối 3 mới nhập từ Excel.

## Nguyên tắc chuẩn

- **Bám sát văn bản:** đánh giá theo Thông tư 27/2020/TT-BGDĐT và sửa đổi tại Thông tư 89/2026/TT-BGDĐT (Học bạ số, giáo viên bộ môn ký số xác nhận kết quả môn mình); chương trình môn Tin theo TT32/2018; khung năng lực số theo TT02/2025 và CV 3456; khung giáo dục AI theo QĐ 2422 và CV 5588.
- **Hai luồng tách bạch:** thường xuyên bằng nhận xét; định kỳ bằng điểm số kết hợp nhận xét. Giữa kỳ môn Tin không có bài kiểm tra — tổng hợp từ quá trình học tập.
- **AI chỉ là trợ lí:** gợi ý mức/nhận xét để giáo viên xem, sửa và chốt; không tự động ghi điểm hay mức chính thức.
- **Offline trước hết:** chạy hoàn toàn không cần mạng tại phòng Tin (kể cả nhập tệp Excel — thư viện đọc Excel đã nhúng sẵn trong tệp); dữ liệu lưu bền lâu ngay trên thiết bị; đồng bộ Drive chỉ thực hiện khi có mạng.
- **Độc lập, tự phục vụ:** sản phẩm số hoá riêng cho môn Tin học, không phụ thuộc hệ thống cơ sở dữ liệu ngành.

## Kỹ thuật

Một tệp HTML duy nhất, không phụ thuộc thư viện ngoài, mở được trên mọi trình duyệt hiện đại, kể cả khi không có mạng. Giao diện theo ngôn ngữ Windows 11 Fluent (phẳng, trung tính, một màu nhấn), tự thích ứng sáng/tối theo hệ thống; font Segoe UI như website nhà trường.

## Nhật ký cập nhật

- **13/11/2026 — v1.0:** phát hành bản đầu tiên lên tule-muse: đủ 7 màn hình theo bản thiết kế đã duyệt; nạp sẵn danh sách thật 708 học sinh của 21 lớp (chỉ họ tên + giới tính, từ tệp Excel giáo viên cung cấp) và thời khóa biểu 21 tiết/tuần; giao diện Fluent sau 3 vòng nghiệm thu (sửa lỗi gãy dòng tên trường trên điện thoại, lỗi lệch căn lề nút/nhãn, gỡ đóng dấu tác giả khỏi các màn hình bên trong và chuyển thông tin tác giả vào mục Thông tin trong Cài đặt); lưu trữ bền lâu trên thiết bị và nhập Excel offline đã gắn sẵn trong bản phát hành.
