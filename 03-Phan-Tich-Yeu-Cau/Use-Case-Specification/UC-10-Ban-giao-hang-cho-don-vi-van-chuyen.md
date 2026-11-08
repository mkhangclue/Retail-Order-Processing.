# UC-10 – Đặc tả Use Case: Bàn giao hàng cho đơn vị vận chuyển

## 1. Thông tin chung

| Thuộc tính | Nội dung |
|---|---|
| Mã Use Case | UC-10 |
| Tên Use Case | Bàn giao hàng cho đơn vị vận chuyển |
| Tác nhân chính | Nhân viên kho |
| Tác nhân phụ | Đơn vị vận chuyển |
| Mục tiêu | Bàn giao kiện hàng cùng thông tin giao hàng cho đơn vị vận chuyển để thực hiện giao hàng. |
| Mức độ ưu tiên | Cao |
| Phạm vi | Quy trình xử lý đơn hàng bán lẻ |

## 2. Mô tả

Use Case mô tả quá trình nhân viên kho bàn giao kiện hàng đã được kiểm tra và đóng gói cho đơn vị vận chuyển. Đơn vị vận chuyển tiếp nhận hàng, kiểm tra thông tin giao hàng và chuẩn bị các điều kiện cần thiết để thực hiện giao hàng.

## 3. Điều kiện tiên quyết (Preconditions)

- Hàng hóa đã được kiểm tra và đóng gói thông qua UC-09.
- Thông tin giao hàng đã được xác nhận.
- Kiện hàng sẵn sàng để bàn giao.

## 4. Luồng sự kiện chính (Main Flow)

1. Nhân viên kho chuẩn bị kiện hàng và thông tin giao hàng.
2. Nhân viên kho bàn giao kiện hàng cho đơn vị vận chuyển.
3. Đơn vị vận chuyển tiếp nhận kiện hàng.
4. Đơn vị vận chuyển kiểm tra thông tin giao hàng.
5. Đơn vị vận chuyển chuẩn bị tuyến đường, phương tiện và tài xế.
6. Đơn vị vận chuyển tiến hành giao hàng.
7. Quy trình chuyển sang bước cập nhật trạng thái giao hàng (UC-11).

## 5. Luồng thay thế (Alternative Flow)

**Trường hợp thông tin giao hàng không chính xác hoặc chưa đầy đủ:**

1. Đơn vị vận chuyển phát hiện thông tin giao hàng có vấn đề.
2. Đơn vị vận chuyển thông báo cho bên liên quan.
3. Thông tin giao hàng được kiểm tra và điều chỉnh trước khi tiếp tục giao hàng.

**Trường hợp đơn vị vận chuyển không thể tiếp nhận kiện hàng:**

1. Nhân viên kho ghi nhận tình trạng chưa bàn giao được hàng.
2. Nhân viên kho phối hợp với bên liên quan để sắp xếp bàn giao lại.

## 6. Điều kiện hậu (Postconditions)

- Kiện hàng đã được bàn giao cho đơn vị vận chuyển.
- Thông tin giao hàng đã được tiếp nhận.
- Đơn hàng chuyển sang giai đoạn vận chuyển.

## 7. Quy tắc nghiệp vụ liên quan

- BR-08: Hàng hóa cần được kiểm tra và đóng gói trước khi bàn giao cho đơn vị vận chuyển.

## 8. Điểm cần xác minh

- Đơn vị vận chuyển được lựa chọn theo tiêu chí nào?
- Việc bàn giao có cần xác nhận số lượng kiện hàng hoặc chứng từ không?
- Ai chịu trách nhiệm khi phát sinh sai lệch trong quá trình bàn giao?
- Thời điểm nào được xem là đơn hàng chính thức chuyển sang trạng thái đang vận chuyển?
- Có cơ chế ghi nhận việc bàn giao thành công hay không?
