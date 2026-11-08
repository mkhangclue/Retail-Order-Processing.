# UC-16 – Đặc tả Use Case: Xử lý hàng hóa bị lỗi

## 1. Thông tin chung

| Thuộc tính | Nội dung |
|---|---|
| Mã Use Case | UC-16 |
| Tên Use Case | Xử lý hàng hóa bị lỗi |
| Tác nhân chính | Nhân viên kho |
| Tác nhân phụ | Nhân viên chăm sóc khách hàng |
| Mục tiêu | Tiếp nhận và xử lý hàng hóa liên quan đến khiếu nại đã được xác minh là hợp lệ. |
| Mức độ ưu tiên | Cao |
| Phạm vi | Quy trình xử lý đơn hàng bán lẻ |

## 2. Mô tả

Use Case mô tả quá trình nhân viên kho tiếp nhận hàng hóa bị lỗi hoặc hàng hóa được trả về theo kết quả xử lý khiếu nại. Tình trạng hàng hóa được kiểm tra và ghi nhận để phục vụ việc chuẩn bị hàng thay thế nếu cần.

## 3. Điều kiện tiên quyết (Preconditions)

- Khiếu nại đã được xác minh là hợp lệ thông qua UC-15.
- Thông tin hàng hóa và nội dung khiếu nại đã được ghi nhận.
- Có yêu cầu xử lý hàng hóa liên quan đến khiếu nại.

## 4. Luồng sự kiện chính (Main Flow)

1. Nhân viên kho tiếp nhận thông tin xử lý khiếu nại.
2. Nhân viên kho tiếp nhận hàng hóa được trả về theo quy trình.
3. Nhân viên kiểm tra tình trạng hàng hóa.
4. Nhân viên đối chiếu hàng hóa với thông tin khiếu nại.
5. Nhân viên ghi nhận kết quả kiểm tra.
6. Hàng hóa được chuyển sang bước chuẩn bị và gửi hàng thay thế thông qua UC-17.

## 5. Luồng thay thế (Alternative Flow)

**Trường hợp chưa nhận được hàng hóa trả về:**

1. Nhân viên kho ghi nhận tình trạng chưa tiếp nhận được hàng.
2. Nhân viên phối hợp với bộ phận chăm sóc khách hàng để kiểm tra thông tin.
3. Việc xử lý tiếp tục sau khi có thông tin phù hợp.

**Trường hợp hàng hóa thực tế không khớp với nội dung khiếu nại:**

1. Nhân viên kho ghi nhận sự khác biệt.
2. Nhân viên thông báo kết quả kiểm tra cho bộ phận chăm sóc khách hàng.
3. Các bên xem xét hướng xử lý tiếp theo.

## 6. Điều kiện hậu (Postconditions)

- Tình trạng hàng hóa liên quan đến khiếu nại được kiểm tra và ghi nhận.
- Thông tin hàng hóa được chuyển đến bước xử lý tiếp theo.
- Nếu cần gửi hàng thay thế, quy trình chuyển sang UC-17.

## 7. Quy tắc nghiệp vụ liên quan

- BR-10: Khiếu nại cần được xác minh bằng thông tin và bằng chứng liên quan trước khi xử lý.

## 8. Điểm cần xác minh

- Những trường hợp nào bắt buộc khách hàng phải trả lại hàng hóa?
- Ai chịu trách nhiệm tiếp nhận và vận chuyển hàng hóa trả về?
- Có quy trình kiểm tra chất lượng hàng hóa sau khi nhận lại không?
- Hàng hóa bị lỗi được lưu kho, sửa chữa hay loại bỏ như thế nào?
- Có trường hợp được gửi hàng thay thế mà không cần thu hồi hàng cũ không?
