# Bản chạy trên trình duyệt

Mở `index.html` bằng Chrome hoặc Edge. File Excel được đọc cục bộ trong trình duyệt trên máy người dùng, không được tải lên máy chủ hay dịch vụ lưu trữ đám mây. Trang không gửi nội dung file Excel đi nơi khác. Thư viện SheetJS được nạp từ CDN khi mở trang, nhưng file Excel không được gửi tới CDN. Nếu cần chạy hoàn toàn không có mạng, tải `xlsx.full.min.js` về cạnh `index.html` rồi đổi thẻ script sang `src="xlsx.full.min.js"`.

Bản web giữ luồng chọn file/sheet, tự gợi ý loại HDCV/BIEU MAU, nhận diện tiêu đề và mã biểu mẫu, loại sheet HUY, kiểm tra lịch sử/ngày/lần ban hành, hợp nhất mã trùng, lọc danh mục/lỗi, xem chi tiết và xuất CSV/XLSX. Trình duyệt không thể kết nối trực tiếp SQL Server; dùng file xuất để nạp vào quy trình SQL hiện có.

