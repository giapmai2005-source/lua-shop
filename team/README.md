# Lụa. Team
App nội bộ demo độc lập tại team/index.html. Chọn tài khoản Quản lý, Ngọc Giáp hoặc Anh Tú. Không có đăng nhập bảo mật.

- Quản lý: báo cáo theo ngày tạo đơn, doanh thu thuần, nhân sự, quyền giảm giá 0–30%, chính sách xem chi tiêu, CRUD sản phẩm, nhập/kiểm kê tồn, đơn và khách, nhật ký, POS và ca.
- Nhân viên: POS, tra kho, đơn/ca của mình, khách của các đơn mình xử lý. Chỉ mở liên hệ từ đơn cụ thể sau khi nhập lý do; địa chỉ chỉ cho đơn giao hàng. Không có thông tin mật khẩu hoặc thẻ.
- Dữ liệu mẫu được lưu tại localStorage lua_team_v1, độc lập với cửa hàng và staff.html cũ. Không đồng bộ máy khác. Đổi tài khoản trên cùng trình duyệt dùng chung dữ liệu.
- Nhập hàng tăng tồn. Kiểm kê đặt lại tồn với lý do. Đơn mới giữ/trừ hàng. Hủy chỉ dành cho đơn chưa thu tiền; trả toàn đơn chỉ dành cho đơn đã thanh toán, hoàn tồn và thu hồi điểm đã cộng, không thực sự chuyển tiền. Đổi hàng dùng luồng trả đơn cũ rồi tạo đơn mới. Chưa có trả từng phần hoặc chính sách bảo hành.
- Báo cáo loại đơn chờ/hủy/trả; doanh thu thuần theo ngày tạo đơn, không phải sổ dòng tiền theo ngày hoàn tiền. Tiền dự kiến khi chốt ca được lưu cố định để đối chiếu.
- Khách, đơn và tồn ban đầu đều là dữ liệu minh họa. Điểm nền không bao gồm đơn mẫu. Đơn mới cộng floor(tổng/10000).
- In hoặc lưu PDF hóa đơn dùng hộp thoại in trình duyệt. Không gửi email/SMS.
- Để dùng thật cần backend, xác thực, kiểm tra quyền phía máy chủ, giao dịch tồn kho, audit không sửa được và dữ liệu an toàn. Không nhập dữ liệu thực vào demo công khai.
