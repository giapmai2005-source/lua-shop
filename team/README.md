# Lụa. Team — Supabase
Đăng nhập tại ../account/, mở team/ bằng tài khoản được cấp vai trò manager hoặc staff. Quản lý cấp vai trò nhân viên cho email đã đăng ký/xác minh tại Nhân viên & quyền. Không có mật khẩu mẫu hoặc chọn vai trò tùy ý.

Sản phẩm, tồn, khách, đơn, ca và nhật ký nằm trong Supabase; trình duyệt không còn là nguồn dữ liệu kinh doanh. Bấm Đồng bộ hoặc quay lại tab để tải lại. Phiên đăng nhập Supabase dùng chung các trang cùng tên miền.

Database chỉ cho API đã kiểm tra người dùng truy cập dữ liệu riêng. Máy chủ tính giá, kiểm tra giảm giá, khóa dòng trạng thái khi ghi đơn để tránh bán quá tồn; kiểm tra revision với thao tác nội bộ để từ chối dữ liệu cũ.

Website khách: đăng nhập, chọn sản phẩm, mở checkout.html để đặt giao hàng COD. Đơn pending giữ hàng. Quản lý mở ca rồi ghi nhận đã thu tiền, hoặc hủy đơn. Trả toàn bộ đơn hoàn tồn và điểm; hệ thống không chuyển khoản hoàn tiền. Chưa có thanh toán qua cổng ngân hàng, hóa đơn thuế, gửi SMS/email hóa đơn hoặc trả từng phần.

Dữ liệu mẫu cũ trong localStorage không tự nhập lên cloud. Danh mục khởi tạo là sản phẩm minh họa. Cửa hàng và Team cần mạng. ZIP offline phiên bản cũ chỉ dùng demo riêng.

Các tệp cloud/schema.sql và cloud/function.sql là tài liệu triển khai nguồn, không tự chạy lại trên dự án đang có dữ liệu. Schema thực tế theo migration history Supabase. Auth bootstrap được giữ riêng, không chứa trong mã web.
