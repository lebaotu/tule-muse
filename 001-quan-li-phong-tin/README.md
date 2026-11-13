# 001 — Ứng dụng quản lí phòng Tin

Ứng dụng web quản lí phòng Tin học dành cho giáo viên phụ trách phòng máy ở trường tiểu học — xây dựng cho phòng Tin **40 máy** của Trường Tiểu học Huỳnh Ngọc Huệ.

**Mở ứng dụng:** mở tệp `index.html` trong thư mục này bằng trình duyệt, hoặc qua GitHub Pages của repo (mục `001-quan-li-phong-tin/`).

## Chức năng

- **Tổng quan:** tình hình phòng máy trong ngày, thao tác nhanh ghi sự cố / ghi tiết dạy / checklist.
- **Sơ đồ phòng:** bản đồ 40 máy trực quan, chạm vào từng máy để ghi sự cố; theo dõi trạng thái sửa chữa và chi phí.
- **Nhật ký tiết dạy:** ghi tiết dạy theo danh mục bài học trong kế hoạch dạy học Tin học lớp 3–5.
- **Kiểm kê thiết bị:** kiểm kê tài sản, in biên bản kiểm kê có chỗ ký.
- **Mượn – trả thiết bị:** phiếu mượn, cảnh báo quá hạn.
- **Checklist mở – đóng phòng:** danh mục việc đầu giờ / cuối giờ, lưu lịch sử theo ngày.
- **Trực nhật:** phân công và theo dõi trực nhật phòng Tin.
- **Báo cáo:** thống kê sự cố, chi phí sửa chữa theo tháng, xuất CSV.
- **Cài đặt & sao lưu:** xuất / khôi phục dữ liệu JSON, khóa mã PIN, đồng bộ.

## Nguyên tắc vận hành

- **Offline trước hết:** phòng Tin của trường chưa có Internet nên ứng dụng chạy hoàn toàn không cần mạng; dữ liệu lưu ngay trên thiết bị đang dùng.
- **Đồng bộ khi có mạng:** qua cầu nối Google Apps Script do chính giáo viên triển khai trên tài khoản Google của mình — dữ liệu đẩy lên Google Drive (thư mục *Sao lưu phòng Tin*), có bản sao an toàn trước mỗi lần ghi đè. Khi không có mạng, sao lưu thủ công bằng tệp JSON qua USB.
- **An toàn:** khóa mã PIN khi mở ứng dụng (mã PIN chỉ lưu dạng băm), tránh học sinh tò mò nghịch máy.

## Kỹ thuật

Một tệp HTML duy nhất, không phụ thuộc thư viện ngoài, mở được trên mọi trình duyệt hiện đại, kể cả khi không có mạng.

## Nhật ký cập nhật

- **12/11/2026 — v1:** phát hành bản đầu tiên lên tule-muse: đủ 9 màn hình, khóa PIN, đồng bộ tự động qua Apps Script (đã kiểm tra kết nối thành công), sửa hiển thị nút ở chế độ tối.
- **13/11/2026 — v1.1:** sửa lỗi khôi phục từ tệp trên iPad/iPhone — tệp sao lưu .json tải từ Drive về bị hệ thống làm mờ, không chọn được trong cửa sổ chọn tệp; nay ô chọn tệp không còn lọc loại tệp, ứng dụng tự kiểm tra nội dung sao lưu trước khi khôi phục.
- **13/11/2026 — v1.2:** vẽ lại sơ đồ phòng theo bố cục phòng Tin thật của trường: hàng mặt trước gồm Bàn giáo viên (GV) — Bảng/máy chiếu — Cửa vào có biểu tượng riêng; 5 dãy dọc × 8 máy đánh số từ phía bảng xuống (01–08, 09–16, 17–24, 25–32, 33–40), dãy 2–3 và 4–5 ghép cặp, 2 lối đi kẻ đứt có nhãn; bỏ bộ chọn số cột trên màn hình sơ đồ.
- **13/11/2026 — v1.3:** sửa lỗi khôi phục từ tệp đối với tệp đồng bộ tải từ Google Drive (phong-tin-moi-nhat.json và các bản trong thư mục Lich-su): ứng dụng nay bóc được lớp gói của tệp đồng bộ khi khôi phục, hiển thị đúng ngày giờ bản đồng bộ ở hộp xác nhận; bổ sung ghi chú giải thích cấu hình, mã PIN và mã khôi phục được lưu riêng theo từng thiết bị.
- **13/11/2026 — v1.4:** Nhật ký tiết dạy bám sát kế hoạch dạy học thật của trường: đổi tên mục "Nhật ký tiết" thành "Nhật ký tiết dạy"; nhúng sẵn lịch 35 tuần năm học 2026–2027, tên bài từng tuần của khối 3/4/5 theo KHDH và thời khóa biểu cố định 21 tiết/tuần theo Lịch báo giảng; form ghi tiết tự tính tuần theo ngày dạy và tự điền bài học, buổi, tiết số (vẫn sửa tay được); thêm thẻ "Lịch dạy hôm nay" ở màn hình Nhật ký tiết dạy và Tổng quan; danh sách lớp đổi sang 21 lớp thật (3/1–3/7, 4/1–4/8, 5/1–5/6), tự di trú nếu đang dùng danh sách mẫu cũ.
- **13/11/2026 — v1.4.1:** sửa lại buổi dạy trong thời khóa biểu theo đúng Lịch báo giảng (khối sáng tối đa 4 tiết, khối chiều tối đa 3 tiết): 5 lớp bị gán nhầm buổi trong v1.4 (4/4 thứ 2, 4/3 thứ 3, 3/4 thứ 4, 5/5 thứ 5, 4/7 thứ 6) đã chuyển từ buổi sáng sang buổi chiều tiết 1; sáng thứ 4 và thứ 5 không có tiết Tin.
