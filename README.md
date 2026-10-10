# Hệ Thống Quản Lý Kho Hàng Thông Minh (GitHub Pages & Supabase Cloud)

Dự án Web App Quản Lý Kho Hàng hoạt động trực tiếp 100% trên **GitHub Pages** (Single Page Application - SPA) kết nối cơ sở dữ liệu **Supabase Cloud Engine** cho tốc độ xử lý siêu tốc, chống trễ dữ liệu và kiểm soát biến động tồn kho chi tiết theo thời gian thực.

## 🚀 Tính Năng Nổi Bật
- **Hoạt động trực tiếp trên GitHub Pages**: Không cần cài đặt máy chủ phức tạp hay phụ thuộc thời gian chờ của Google Apps Script.
- **Supabase Cloud Engine**: Tối ưu hóa truy vấn trực tiếp từ trình duyệt web với tốc độ mili-giây.
- **Tự Động Kết Nối & Tải Siêu Tốc**: Hệ thống tự động kết nối bằng API Key bảo mật, không cần người dùng nhập cấu hình hay bấm nút thủ công.
- **Cơ Chế Bộ Nhớ Đệm (Cache-First)**: Mở trang là thấy ngay toàn bộ bảng tồn kho trong **0 mili-giây**, dữ liệu mới nhất tự động đồng bộ ngầm song song.
- **Xử Lý Song Song (Parallel Batching)**: Tải toàn bộ 1.454+ sản phẩm vượt giới hạn 1.000 dòng của Supabase trong chưa đầy 1 giây.
- **Quy Cách Bao Gói (Pack Qty)**: Đồng bộ tỷ lệ bao gói sang bảng tồn kho, biến động ngày và thẻ kho.
- **Giao Diện Hiện Đại**: Tailwind CSS, Bootstrap Icons, SweetAlert2, JetBrains Mono font cho số liệu.
- **Xuất Nhập Excel**: Xử lý trực tiếp file Excel trên trình duyệt qua SheetJS & ExcelJS.

## 📁 Cấu Trúc Mã Nguồn
- `index.html`: Toàn bộ mã nguồn giao diện và động cơ Supabase Engine xử lý nghiệp vụ kho.
- `Code.gs`: Bản dự phòng cho Google Apps Script (nếu cần triển khai trên Google Sheets).
- `appsscript.json`: File cấu hình Google Apps Script manifest.

## 🛠️ Hướng Dẫn Triển Khai Lại Lên GitHub Pages
1. Truy cập kho lưu trữ GitHub của bạn: `https://github.com/tandv0521-commits/quan-ly-kho-supabase`
2. Bấm vào file `index.html` > Bấm biểu tượng cây bút **Edit this file** (hoặc chọn **Add file** > **Upload files** rồi kéo file `index.html` vào).
3. Bấm **Commit changes**.
4. Truy cập Web App: [https://tandv0521-commits.github.io/quan-ly-kho-supabase/](https://tandv0521-commits.github.io/quan-ly-kho-supabase/)
5. Nhấn **Ctrl + F5** để trình duyệt cập nhật phiên bản mới nhất:
   - Nút kết nối đã được lược bỏ hoàn toàn.
   - Ứng dụng tự động kết nối và tải toàn bộ dữ liệu kho tức thì!
