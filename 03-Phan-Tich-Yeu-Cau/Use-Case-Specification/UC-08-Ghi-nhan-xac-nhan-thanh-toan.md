# UC-08 – Đặc tả Use Case: Ghi nhận xác nhận thanh toán

## 1. Thông tin chung

| Thuộc tính | Nội dung |
|---|---|
| Mã Use Case | UC-08 |
| Tên Use Case | Ghi nhận xác nhận thanh toán |
| Tác nhân chính | Nhân viên bán hàng |
| Tác nhân phụ | Khách hàng |
| Mục tiêu | Tiếp nhận và ghi nhận thông tin xác nhận thanh toán của khách hàng. |
| Mức độ ưu tiên | Cao |
| Phạm vi | Quy trình xử lý đơn hàng bán lẻ |

## 2. Mô tả

Use Case mô tả quá trình khách hàng thực hiện thanh toán và gửi xác nhận thanh toán cho doanh nghiệp. Nhân viên tiếp nhận thông tin và ghi nhận kết quả thanh toán để phục vụ các bước xử lý tiếp theo.

## 3. Điều kiện tiên quyết (Preconditions)

- Hóa đơn đã được lập và hoàn thiện thông qua UC-07.
- Thông tin thanh toán đã được gửi đến khách hàng.

## 4. Luồng sự kiện chính (Main Flow)

1. Khách hàng thực hiện thanh toán theo thông tin được cung cấp.
2. Khách hàng gửi xác nhận thanh toán cho doanh nghiệp.
3. Nhân viên bán hàng tiếp nhận thông tin xác nhận.
4. Nhân viên kiểm tra thông tin thanh toán.
5. Nhân viên ghi nhận kết quả thanh toán.
6. Đơn hàng được chuyển sang bước chuẩn bị hàng hóa.

## 5. Luồng thay thế (Alternative Flow)

**Trường hợp chưa nhận được xác nhận thanh toán:**

1. Nhân viên kiểm tra tình trạng xác nhận thanh toán.
2. Nhân viên liên hệ khách hàng để yêu cầu bổ sung xác nhận nếu cần.
3. Đơn hàng tiếp tục ở trạng thái chờ xác nhận thanh toán.

**Trường hợp thông tin xác nhận chưa hợp lệ:**

1. Nhân viên thông báo cho khách hàng.
2. Khách hàng cung cấp lại thông tin xác nhận.
3. Nhân viên kiểm tra lại thông tin.

## 6. Điều kiện hậu (Postconditions)

- Thông tin xác nhận thanh toán đã được tiếp nhận và ghi nhận.
- Nếu chưa có xác nhận hợp lệ, đơn hàng tiếp tục ở trạng thái chờ thanh toán hoặc chờ xác minh.

## 7. Quy tắc nghiệp vụ liên quan

- BR-07: Khách hàng gửi xác nhận thanh toán trong thời hạn 2 ngày theo quy trình được mô tả.

## 8. Điểm cần xác minh

- Doanh nghiệp hỗ trợ những phương thức thanh toán nào?
- Nhân viên kiểm tra thanh toán bằng chứng từ hay đối chiếu trực tiếp trên tài khoản?
- Ai chịu trách nhiệm xác nhận thanh toán cuối cùng?
- Nếu quá 2 ngày chưa có xác nhận thanh toán, đơn hàng được xử lý như thế nào?
- Có trường hợp cho phép chuẩn bị hàng trước khi xác nhận thanh toán không?
