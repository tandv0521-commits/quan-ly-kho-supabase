# Hệ Thống Quản Lý Kho Thông Minh (Supabase Engine & Google Apps Script)

Dự án Web App Quản Lý Kho Hàng phát triển trên nền tảng **Google Apps Script** tích hợp cơ sở dữ liệu **Supabase Cloud Engine** cho tốc độ xử lý siêu tốc, chống trễ dữ liệu và kiểm soát biến động tồn kho chi tiết.

## 🚀 Tính Năng Chính
- **Supabase Cloud Engine**: Tối ưu hóa truy vấn một chiều, triệt tiêu độ trễ đồng bộ.
- **Auto-Pagination**: Vượt qua giới hạn 1.000 dòng của Supabase PostgREST.
- **Batching & Chunking**: Tối ưu chia mẻ ghi dữ liệu lớn (250 dòng/batch).
- **Quy Cách Bao Gói (Pack Qty)**: Đồng bộ tự động tỷ lệ đóng gói sang bảng tồn kho, biến động ngày và thẻ kho.
- **Giao Diện Hiện Đại**: Xây dựng với Tailwind CSS, Bootstrap Icons, SweetAlert2, JetBrains Mono font cho số liệu.
- **Xuất Nhập Excel**: Tích hợp ExcelJS & SheetJS (XLSX) xử lý trực tiếp trên trình duyệt.

## 📁 Cấu Trúc File
- `Code.gs` / `Mã.gs`: Mã nguồn backend Google Apps Script xử lý REST API Supabase và nghiệp vụ kho.
- `Index.html`: Toàn bộ giao diện Web App phía client (HTML, CSS, JavaScript).
- `appsscript.json`: File cấu hình dự án Google Apps Script manifest.

## 🛠️ Hướng Dẫn Cài Đặt Lên Google Sheets
1. Mở Google Trang tính > **Tiện ích mở rộng** > **Apps Script**.
2. Dán nội dung `Code.gs` vào file script.
3. Tạo file HTML đặt tên là `Index` và dán nội dung từ `Index.html`.
4. Bấm **Triển khai (Deploy)** > **Tùy chọn triển khai mới (New deployment)** > Chọn **Ứng dụng web (Web app)**.
5. Cấp quyền truy cập Google và nhận đường dẫn Web App để sử dụng.
