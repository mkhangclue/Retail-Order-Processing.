# UC-12 – Đặc tả Use Case: Xử lý giao hàng thất bại

## 1. Thông tin chung

| Thuộc tính | Nội dung |
|---|---|
| Mã Use Case | UC-12 |
| Tên Use Case | Xử lý giao hàng thất bại |
| Tác nhân chính | Nhân viên chăm sóc khách hàng |
| Tác nhân phụ | Khách hàng, đơn vị vận chuyển |
| Mục tiêu | Xử lý các trường hợp giao hàng không thành công và xác định hướng xử lý tiếp theo cho đơn hàng. |
| Mức độ ưu tiên | Cao |
| Phạm vi | Quy trình xử lý đơn hàng bán lẻ |

## 2. Mô tả

Use Case mô tả quá trình nhân viên chăm sóc khách hàng tiếp nhận thông tin giao hàng thất bại, liên hệ khách hàng để xác minh tình hình và phối hợp với các bên liên quan nhằm xử lý đơn hàng.

## 3. Điều kiện tiên quyết (Preconditions)

- Đơn hàng đã được bàn giao cho đơn vị vận chuyển.
- Đơn vị vận chuyển đã cập nhật trạng thái giao hàng thất bại thông qua UC-11.
- Thông tin đơn hàng và khách hàng có sẵn để kiểm tra.

## 4. Luồng sự kiện chính (Main Flow)

1. Nhân viên chăm sóc khách hàng tiếp nhận thông tin giao hàng thất bại.
2. Nhân viên kiểm tra thông tin và tình trạng đơn hàng.
3. Nhân viên liên hệ khách hàng để xác minh nguyên nhân giao hàng thất bại.
4. Nhân viên ghi nhận phản hồi và nhu cầu nhận hàng của khách hàng.
5. Nhân viên phối hợp với các bên liên quan để xác định hướng xử lý.
6. Nếu tiếp tục giao hàng, đơn hàng được chuyển lại khâu chuẩn bị và bàn giao vận chuyển.
7. Nhân viên cập nhật kết quả xử lý.

## 5. Luồng thay thế (Alternative Flow)

**Trường hợp khách hàng đồng ý nhận lại hàng:**

1. Nhân viên ghi nhận yêu cầu giao hàng lại.
2. Nhân viên phối hợp với bộ phận liên quan để chuẩn bị đơn hàng.
3. Đơn hàng được chuyển sang quy trình chuẩn bị và giao hàng lại.

**Trường hợp chưa xác định được hướng xử lý:**

1. Nhân viên tiếp tục liên hệ khách hàng hoặc đơn vị vận chuyển để làm rõ tình hình.
2. Đơn hàng được giữ ở trạng thái chờ xử lý.
3. Sau khi có thông tin, nhân viên tiếp tục thực hiện các bước xử lý phù hợp.

## 6. Điều kiện hậu (Postconditions)

- Nguyên nhân hoặc tình trạng giao hàng thất bại được ghi nhận trong phạm vi thông tin thu thập được.
- Hướng xử lý tiếp theo của đơn hàng được xác định hoặc ghi nhận đang chờ xử lý.
- Nếu giao hàng lại, đơn hàng được chuyển sang khâu chuẩn bị và vận chuyển.

## 7. Quy tắc nghiệp vụ liên quan

- BR-09: Khi giao hàng thất bại, bộ phận chăm sóc khách hàng liên hệ khách hàng và phối hợp xử lý đơn hàng.

## 8. Điểm cần xác minh

- Những nguyên nhân giao hàng thất bại nào được ghi nhận?
- Ai có quyền quyết định giao hàng lại hoặc dừng xử lý đơn hàng?
- Đơn hàng được phép giao lại tối đa bao nhiêu lần?
- Chi phí phát sinh khi giao hàng lại do bên nào chịu trách nhiệm?
- Nếu không thể liên hệ khách hàng, đơn hàng được xử lý như thế nào?
