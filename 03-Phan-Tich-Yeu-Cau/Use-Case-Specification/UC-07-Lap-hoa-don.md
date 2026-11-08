# UC-07 – Đặc tả Use Case: Lập hóa đơn

## 1. Thông tin chung

| Thuộc tính | Nội dung |
|---|---|
| Mã Use Case | UC-07 |
| Tên Use Case | Lập hóa đơn |
| Tác nhân chính | Nhân viên bán hàng |
| Tác nhân phụ | Khách hàng |
| Mục tiêu | Lập hóa đơn dựa trên thông tin đơn hàng và các điều kiện giao dịch đã được xác nhận. |
| Mức độ ưu tiên | Cao |
| Phạm vi | Quy trình xử lý đơn hàng bán lẻ |

## 2. Mô tả

Use Case mô tả quá trình nhân viên bán hàng lập hóa đơn cho đơn hàng, bao gồm thông tin sản phẩm, số lượng, giá trị đơn hàng, phí liên quan và thông tin bảo hiểm nếu có.

## 3. Điều kiện tiên quyết (Preconditions)

- Thông tin đơn hàng đã được kiểm tra.
- Tình trạng hàng hóa đã được xác định.
- Thông tin giao hàng và phương thức giao hàng đã được xác nhận.

## 4. Luồng sự kiện chính (Main Flow)

1. Nhân viên bán hàng tổng hợp thông tin đơn hàng.
2. Nhân viên xác định giá trị sản phẩm và các khoản phí liên quan.
3. Nhân viên kiểm tra nhu cầu bảo hiểm cho đơn hàng.
4. Nếu đơn hàng có bảo hiểm, nhân viên bổ sung phí và thông tin bảo hiểm vào hóa đơn.
5. Nếu đơn hàng không có bảo hiểm, tiếp tục lập hóa đơn theo thông tin thông thường.
6. Nhân viên hoàn thiện hóa đơn.
7. Nhân viên gửi thông tin thanh toán cho khách hàng.

## 5. Luồng thay thế (Alternative Flow)

**Trường hợp thông tin hóa đơn chưa chính xác hoặc chưa đầy đủ:**

1. Nhân viên xác định thông tin cần điều chỉnh.
2. Nhân viên kiểm tra lại thông tin đơn hàng.
3. Nhân viên cập nhật nội dung hóa đơn.
4. Nhân viên hoàn thiện lại hóa đơn trước khi gửi khách hàng.

## 6. Điều kiện hậu (Postconditions)

- Hóa đơn đã được lập và hoàn thiện.
- Thông tin thanh toán được gửi đến khách hàng.
- Đơn hàng chuyển sang giai đoạn chờ xác nhận thanh toán.

## 7. Quy tắc nghiệp vụ liên quan

- BR-06: Nếu đơn hàng có bảo hiểm, phí và thông tin bảo hiểm cần được bổ sung vào hóa đơn.

## 8. Điểm cần xác minh

- Hóa đơn được lập trên hệ thống nào?
- Những thông tin nào bắt buộc phải có trên hóa đơn?
- Ai có quyền điều chỉnh hoặc xác nhận hóa đơn?
- Phí bảo hiểm được tính theo quy tắc nào?
- Hóa đơn trong quy trình là hóa đơn bán hàng hay hóa đơn tài chính theo quy định?
