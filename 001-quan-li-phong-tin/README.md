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
