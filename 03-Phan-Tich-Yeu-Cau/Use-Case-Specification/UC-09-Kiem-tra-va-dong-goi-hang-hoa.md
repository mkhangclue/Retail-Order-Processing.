# UC-09 – Đặc tả Use Case: Kiểm tra và đóng gói hàng hóa

## 1. Thông tin chung

| Thuộc tính | Nội dung |
|---|---|
| Mã Use Case | UC-09 |
| Tên Use Case | Kiểm tra và đóng gói hàng hóa |
| Tác nhân chính | Nhân viên kho |
| Tác nhân phụ | Quản lý kho (cần xác minh) |
| Mục tiêu | Đảm bảo hàng hóa được kiểm tra và đóng gói phù hợp trước khi bàn giao cho đơn vị vận chuyển. |
| Mức độ ưu tiên | Cao |
| Phạm vi | Quy trình xử lý đơn hàng bán lẻ |

## 2. Mô tả

Use Case mô tả quá trình nhân viên kho tiếp nhận thông tin đơn hàng, kiểm tra hàng hóa và thực hiện đóng gói theo yêu cầu. Đối với đơn hàng có bảo hiểm, hàng hóa cần được đóng gói theo chính sách bảo hiểm và dán nhãn cảnh báo nếu cần thiết.

## 3. Điều kiện tiên quyết (Preconditions)

- Đơn hàng đã hoàn thành các bước xử lý thông tin và hóa đơn.
- Thông tin thanh toán đã được ghi nhận theo quy trình.
- Nhân viên kho nhận được thông tin đơn hàng cần chuẩn bị.

## 4. Luồng sự kiện chính (Main Flow)

1. Nhân viên kho tiếp nhận thông tin đơn hàng.
2. Nhân viên kiểm tra thông tin đơn hàng trên hệ thống.
3. Nhân viên kiểm tra sản phẩm và số lượng cần đóng gói.
4. Nhân viên xác định đơn hàng có bảo hiểm hay không.
5. Nếu có bảo hiểm, nhân viên đóng gói theo chính sách bảo hiểm và dán nhãn cảnh báo nếu cần.
6. Nếu không có bảo hiểm, nhân viên thực hiện đóng gói theo quy cách thông thường.
7. Nhân viên kiểm tra lại thông tin kiện hàng trước khi bàn giao.

## 5. Luồng thay thế (Alternative Flow)

**Trường hợp hàng hóa không đúng với thông tin đơn hàng:**

1. Nhân viên kho phát hiện sai lệch về sản phẩm hoặc số lượng.
2. Nhân viên tạm dừng đóng gói.
3. Nhân viên kiểm tra lại thông tin đơn hàng và tình trạng hàng hóa.
4. Sai lệch được xử lý trước khi tiếp tục đóng gói.

**Trường hợp hàng hóa bị hư hỏng:**

1. Nhân viên phát hiện sản phẩm bị hư hỏng.
2. Nhân viên ghi nhận tình trạng hàng hóa.
3. Nhân viên báo cáo người phụ trách để xem xét hướng xử lý.

## 6. Điều kiện hậu (Postconditions)

- Hàng hóa đã được kiểm tra và đóng gói.
- Thông tin kiện hàng đã được kiểm tra trước khi bàn giao.
- Đơn hàng sẵn sàng chuyển sang bước bàn giao cho đơn vị vận chuyển.

## 7. Quy tắc nghiệp vụ liên quan

- BR-08: Nhân viên kho cần kiểm tra và đóng gói hàng hóa trước khi bàn giao cho đơn vị vận chuyển.
- Đơn hàng có bảo hiểm cần được đóng gói theo chính sách bảo hiểm tương ứng.

## 8. Điểm cần xác minh

- Ai chịu trách nhiệm xác nhận hàng hóa trước khi đóng gói?
- Có checklist kiểm tra sản phẩm và số lượng không?
- Quy cách đóng gói được quy định theo loại sản phẩm hay giá trị đơn hàng?
- Những trường hợp nào cần dán nhãn cảnh báo?
- Quy trình xử lý khi phát hiện hàng hóa hư hỏng trước khi giao hàng là gì?
