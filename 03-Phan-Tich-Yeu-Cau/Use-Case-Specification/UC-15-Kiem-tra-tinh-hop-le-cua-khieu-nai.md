# UC-15 – Đặc tả Use Case: Kiểm tra tính hợp lệ của khiếu nại

## 1. Thông tin chung

| Thuộc tính | Nội dung |
|---|---|
| Mã Use Case | UC-15 |
| Tên Use Case | Kiểm tra tính hợp lệ của khiếu nại |
| Tác nhân chính | Nhân viên chăm sóc khách hàng |
| Tác nhân phụ | Khách hàng |
| Mục tiêu | Xác minh thông tin và bằng chứng để xác định khiếu nại có hợp lệ hay không. |
| Mức độ ưu tiên | Cao |
| Phạm vi | Quy trình xử lý đơn hàng bán lẻ |

## 2. Mô tả

Use Case mô tả quá trình nhân viên chăm sóc khách hàng kiểm tra nội dung khiếu nại, đối chiếu thông tin đơn hàng và xem xét hình ảnh hoặc bằng chứng do khách hàng cung cấp. Kết quả kiểm tra được sử dụng để xác định hướng xử lý tiếp theo.

## 3. Điều kiện tiên quyết (Preconditions)

- Khiếu nại đã được tiếp nhận thông qua UC-14.
- Thông tin đơn hàng và nội dung khiếu nại đã được ghi nhận.
- Hình ảnh hoặc bằng chứng liên quan đã được cung cấp hoặc đang chờ bổ sung.

## 4. Luồng sự kiện chính (Main Flow)

1. Nhân viên chăm sóc khách hàng mở thông tin khiếu nại.
2. Nhân viên kiểm tra nội dung phản ánh của khách hàng.
3. Nhân viên đối chiếu thông tin khiếu nại với dữ liệu đơn hàng.
4. Nhân viên kiểm tra hình ảnh hoặc bằng chứng liên quan.
5. Nhân viên đánh giá tính hợp lệ của khiếu nại.
6. Nếu khiếu nại hợp lệ, nhân viên chuyển sang bước xử lý hàng hóa bị lỗi thông qua UC-16.
7. Nếu khiếu nại không hợp lệ, nhân viên ghi nhận kết quả và thông báo cho khách hàng.

## 5. Luồng thay thế (Alternative Flow)

**Trường hợp chưa đủ bằng chứng để xác minh:**

1. Nhân viên xác định thông tin hoặc bằng chứng còn thiếu.
2. Nhân viên yêu cầu khách hàng bổ sung.
3. Khách hàng cung cấp thêm thông tin hoặc hình ảnh.
4. Nhân viên tiếp tục kiểm tra khiếu nại.

**Trường hợp khiếu nại không hợp lệ:**

1. Nhân viên ghi nhận lý do khiếu nại không hợp lệ.
2. Nhân viên thông báo kết quả cho khách hàng.
3. Quy trình xử lý khiếu nại kết thúc theo kết quả xác minh.

## 6. Điều kiện hậu (Postconditions)

- Kết quả xác minh khiếu nại đã được ghi nhận.
- Khiếu nại hợp lệ được chuyển sang bước xử lý tiếp theo.
- Khiếu nại không hợp lệ được ghi nhận kết quả và thông báo cho khách hàng.

## 7. Quy tắc nghiệp vụ liên quan

- BR-10: Khiếu nại liên quan đến hàng hóa bị thiếu, hư hỏng hoặc giao sai cần được kiểm tra bằng hình ảnh hoặc bằng chứng liên quan.

## 8. Điểm cần xác minh

- Tiêu chí cụ thể để xác định khiếu nại hợp lệ là gì?
- Ai có quyền đưa ra quyết định cuối cùng?
- Có cần bộ phận kho phối hợp xác minh không?
- Nếu bằng chứng không rõ ràng, khiếu nại được xử lý như thế nào?
- Có lưu lại lý do chấp nhận hoặc từ chối khiếu nại không?
