# UC-17 – Đặc tả Use Case: Chuẩn bị và gửi hàng thay thế

## 1. Thông tin chung

| Thuộc tính | Nội dung |
|---|---|
| Mã Use Case | UC-17 |
| Tên Use Case | Chuẩn bị và gửi hàng thay thế |
| Tác nhân chính | Nhân viên kho |
| Tác nhân phụ | Đơn vị vận chuyển, nhân viên chăm sóc khách hàng |
| Mục tiêu | Chuẩn bị và gửi hàng thay thế cho khách hàng theo kết quả xử lý khiếu nại hợp lệ. |
| Mức độ ưu tiên | Cao |
| Phạm vi | Quy trình xử lý đơn hàng bán lẻ |

## 2. Mô tả

Use Case mô tả quá trình nhân viên kho chuẩn bị hàng hóa thay thế sau khi khiếu nại được xác minh là hợp lệ. Hàng hóa được kiểm tra, đóng gói và bàn giao cho đơn vị vận chuyển để gửi đến khách hàng.

## 3. Điều kiện tiên quyết (Preconditions)

- Khiếu nại đã được xác minh là hợp lệ thông qua UC-15.
- Thông tin xử lý hàng hóa liên quan đã được ghi nhận thông qua UC-16.
- Có yêu cầu chuẩn bị hàng thay thế.
- Thông tin giao hàng của khách hàng đã được xác định.

## 4. Luồng sự kiện chính (Main Flow)

1. Nhân viên kho tiếp nhận yêu cầu chuẩn bị hàng thay thế.
2. Nhân viên kiểm tra thông tin sản phẩm và số lượng cần thay thế.
3. Nhân viên kiểm tra tình trạng hàng hóa trong kho.
4. Nhân viên chuẩn bị sản phẩm thay thế.
5. Nhân viên thực hiện đóng gói hàng hóa.
6. Nhân viên kiểm tra lại thông tin kiện hàng.
7. Nhân viên bàn giao hàng cho đơn vị vận chuyển.
8. Đơn vị vận chuyển tiếp nhận hàng và thực hiện giao hàng đến khách hàng.
9. Kết quả giao hàng được chuyển đến bộ phận chăm sóc khách hàng.

## 5. Luồng thay thế (Alternative Flow)

**Trường hợp không đủ hàng thay thế:**

1. Nhân viên kho phát hiện số lượng hàng hóa không đáp ứng yêu cầu.
2. Nhân viên ghi nhận tình trạng thiếu hàng.
3. Nhân viên thông báo cho bộ phận chăm sóc khách hàng.
4. Các bên phối hợp xác định hướng xử lý tiếp theo.

**Trường hợp thông tin giao hàng cần điều chỉnh:**

1. Nhân viên phát hiện thông tin giao hàng chưa phù hợp.
2. Nhân viên phối hợp với bộ phận chăm sóc khách hàng để xác minh.
3. Thông tin được điều chỉnh trước khi bàn giao hàng.

## 6. Điều kiện hậu (Postconditions)

- Hàng thay thế đã được chuẩn bị và bàn giao cho đơn vị vận chuyển.
- Thông tin giao hàng thay thế được ghi nhận.
- Kết quả giao hàng được chuyển đến bộ phận chăm sóc khách hàng để tiếp tục xử lý khiếu nại.

## 7. Quy tắc nghiệp vụ liên quan

- BR-08: Hàng hóa cần được kiểm tra và đóng gói trước khi bàn giao cho đơn vị vận chuyển.
- BR-10: Việc xử lý hàng hóa thay thế được thực hiện sau khi khiếu nại được xác minh hợp lệ.

## 8. Điểm cần xác minh

- Hàng thay thế có bắt buộc phải giống hoàn toàn sản phẩm ban đầu không?
- Ai chịu trách nhiệm phê duyệt việc xuất hàng thay thế?
- Nếu kho không còn hàng, doanh nghiệp xử lý như thế nào?
- Hàng thay thế có sử dụng mã đơn hàng mới hay tiếp tục sử dụng mã đơn hàng cũ?
- Chi phí vận chuyển hàng thay thế do bên nào chịu trách nhiệm?
- Có cần cập nhật lại thông tin bảo hiểm cho kiện hàng thay thế không?
