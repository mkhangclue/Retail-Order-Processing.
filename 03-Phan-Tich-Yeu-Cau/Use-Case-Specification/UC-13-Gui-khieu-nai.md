# UC-13 – Đặc tả Use Case: Gửi khiếu nại

## 1. Thông tin chung

| Thuộc tính | Nội dung |
|---|---|
| Mã Use Case | UC-13 |
| Tên Use Case | Gửi khiếu nại |
| Tác nhân chính | Khách hàng |
| Tác nhân phụ | Nhân viên chăm sóc khách hàng |
| Mục tiêu | Gửi thông tin khiếu nại về tình trạng hàng hóa sau khi nhận hàng. |
| Mức độ ưu tiên | Cao |
| Phạm vi | Quy trình xử lý đơn hàng bán lẻ |

## 2. Mô tả

Use Case mô tả quá trình khách hàng phản ánh các vấn đề phát sinh sau khi nhận hàng, bao gồm thiếu sản phẩm, sản phẩm bị hư hỏng hoặc giao sai sản phẩm. Thông tin khiếu nại được gửi đến bộ phận chăm sóc khách hàng để tiếp nhận và xử lý.

## 3. Điều kiện tiên quyết (Preconditions)

- Khách hàng đã nhận được hàng hoặc đã phát hiện vấn đề liên quan đến đơn hàng.
- Đơn hàng có thông tin để đối chiếu và xác minh.

## 4. Luồng sự kiện chính (Main Flow)

1. Khách hàng phát hiện vấn đề liên quan đến hàng hóa.
2. Khách hàng liên hệ doanh nghiệp để gửi khiếu nại.
3. Khách hàng cung cấp thông tin đơn hàng và mô tả vấn đề.
4. Khách hàng cung cấp hình ảnh hàng hóa hoặc bằng chứng liên quan khi được yêu cầu.
5. Nhân viên chăm sóc khách hàng tiếp nhận thông tin khiếu nại.
6. Khiếu nại được chuyển sang UC-14 – Tiếp nhận khiếu nại.

## 5. Luồng thay thế (Alternative Flow)

**Trường hợp khách hàng chưa cung cấp đủ thông tin:**

1. Nhân viên chăm sóc khách hàng yêu cầu khách hàng bổ sung thông tin.
2. Khách hàng cung cấp thông tin hoặc bằng chứng còn thiếu.
3. Nhân viên tiếp tục tiếp nhận khiếu nại.

**Trường hợp khách hàng không cung cấp được bằng chứng:**

1. Nhân viên ghi nhận tình trạng thiếu bằng chứng.
2. Khiếu nại được chuyển sang bước xem xét và xác minh theo quy trình.

## 6. Điều kiện hậu (Postconditions)

- Thông tin khiếu nại đã được gửi đến doanh nghiệp.
- Nội dung phản ánh và bằng chứng liên quan được ghi nhận nếu có.
- Khiếu nại sẵn sàng được tiếp nhận và kiểm tra.

## 7. Quy tắc nghiệp vụ liên quan

- BR-10: Khiếu nại liên quan đến hàng hóa bị thiếu, hư hỏng hoặc giao sai cần được kiểm tra bằng hình ảnh hoặc bằng chứng liên quan.

## 8. Điểm cần xác minh

- Khách hàng có thể gửi khiếu nại qua những kênh nào?
- Thông tin nào bắt buộc phải cung cấp khi gửi khiếu nại?
- Hình ảnh hoặc bằng chứng có bắt buộc trong mọi trường hợp không?
- Thời hạn tiếp nhận khiếu nại sau khi khách hàng nhận hàng là bao lâu?
- Có quy định riêng cho từng loại khiếu nại không?
