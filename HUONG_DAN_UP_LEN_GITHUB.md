# HƯỚNG DẪN ĐƯA PHẦN MỀM LÊN GITHUB ĐỂ SỬ DỤNG PHIÊN BẢN WEB & ĐÁM MÂY (SUPABASE)

Tệp `index.html` trong thư mục này đã được tối ưu hóa toàn diện cho môi trường Web. Khi được tải lên GitHub và bật tính năng **GitHub Pages**, phần mềm sẽ tự động chạy ở **Chế độ Đám Mây (Supabase Cloud)**, giúp bạn và các thành viên khác có thể truy cập qua điện thoại, máy tính bảng hoặc máy tính ở bất kỳ đâu và dữ liệu được đồng bộ trực tuyến theo thời gian thực.

---

## BƯỚC 1: TẠO KHO LƯU TRỮ (REPOSITORY) TRÊN GITHUB

1. Truy cập [https://github.com](https://github.com) và đăng nhập tài khoản của bạn.
2. Bấm vào nút **"New"** (hoặc dấu cộng `+` ở góc trên bên phải -> chọn **New repository**).
3. Đặt tên kho lưu trữ tại ô **Repository name**: ví dụ `quan-ly-kho` hoặc `kho-hang`.
4. Để chế độ là **Public** (để dùng được tính năng GitHub Pages miễn phí).
5. Bấm nút xanh **"Create repository"** ở dưới cùng.

---

## BƯỚC 2: TẢI TỆP LÊN GITHUB

1. Tại trang kho lưu trữ vừa tạo, bấm vào liên kết **"uploading an existing file"** (hoặc nút **Add file** -> **Upload files**).
2. Kéo thả 2 tệp trong thư mục `Ban-Giao-Web-GitHub` vào trình duyệt:
   - **`index.html`** *(Bắt buộc phải giữ đúng tên `index.html` viết thường)*
   - **`favicon.svg`** *(Icon kho hàng hiển thị trên tab trình duyệt)*
3. Kéo xuống dưới và bấm nút xanh **"Commit changes"** để lưu tệp.

---

## BƯỚC 3: BẬT TÍNH NĂNG GITHUB PAGES (PHIÊN BẢN WEB)

1. Trong kho lưu trữ GitHub của bạn, bấm vào tab **Settings** (biểu tượng bánh răng ở thanh menu ngang trên cùng).
2. Ở cột menu bên trái, tìm và bấm vào mục **Pages** (mục GitHub Pages).
3. Tại phần **Build and deployment**:
   - Ở mục **Source**: Chọn **Deploy from a branch**.
   - Ở mục **Branch**: Chọn nhánh **`main`** (hoặc `master`), thư mục chọn **`/ (root)`**.
   - Bấm nút **"Save"**.
4. Chờ khoảng 1 - 2 phút, sau đó tải lại trang Settings -> Pages:
   - Bạn sẽ nhìn thấy đường dẫn trang web xuất hiện ở khung trên cùng, dạng:
     `https://<ten-tai-khoan>.github.io/<ten-kho>/`
     *(Ví dụ: `https://nguyenvana.github.io/quan-ly-kho/`)*

---

## BƯỚC 4: SỬ DỤNG VÀ CHIA SẺ

- Bây giờ bạn có thể mở đường dẫn trên bằng bất kỳ trình duyệt nào:
  - Máy tính để bàn, Laptop (Chrome, Edge, Cốc Cốc, Firefox...)
  - Điện thoại thông minh (iPhone Safari, Android Chrome...)
  - Máy tính bảng / iPad
- Khi truy cập qua đường dẫn này:
  - Hệ thống tự động kích hoạt **Đám mây (Supabase)**.
  - Toàn bộ danh mục hàng hóa, tồn kho, phiếu nhập, phiếu xuất, nhập trả, thẻ kho và nhật ký đều được lưu trên Cloud.
  - Mọi thao tác lập phiếu ở máy tính A sẽ lập tức cập nhật cho người xem ở máy tính B hoặc điện thoại.

---

## LƯU Ý VỀ TÍNH NĂNG PHÁT HÀNG CHO XE (NẾU DÙNG CLOUD):
- Cơ sở dữ liệu Supabase hiện tại đã có sẵn các bảng tồn kho và chứng từ: `products`, `phieu_nhap`, `phieu_xuat`, `hang_nhap_tra`, `inventory_transactions`, `voucher_audit_logs`.
- Nếu bạn muốn đưa cả 3 tính năng mới (Phát hàng theo xe, Danh mục xe, Nhân viên kho) lên đồng bộ Cloud:
  - Đăng nhập [https://supabase.com](https://supabase.com) -> Mở dự án kho của bạn.
  - Chọn mục **SQL Editor** ở thanh bên trái.
  - Mở tệp `supabase_setup_phat_hang.sql` trong thư mục này, sao chép toàn bộ nội dung và dán vào SQL Editor rồi bấm **Run**.
  - *(Nếu chưa chạy script này, phần mềm vẫn hoạt động bình thường và tự động lưu các lượt phát xe trên bộ nhớ thiết bị mà không bao giờ bị báo lỗi).*
