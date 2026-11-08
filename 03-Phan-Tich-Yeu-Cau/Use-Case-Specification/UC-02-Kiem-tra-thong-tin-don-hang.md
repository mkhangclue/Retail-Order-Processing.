# UC-02 – Đặc tả Use Case: Kiểm tra thông tin đơn hàng

## 1. Thông tin chung

| Thuộc tính | Nội dung |
|---|---|
| Mã Use Case | UC-02 |
| Tên Use Case | Kiểm tra thông tin đơn hàng |
| Tác nhân chính | Nhân viên bán hàng |
| Mục tiêu | Đảm bảo thông tin đơn hàng được cung cấp đầy đủ và chính xác trước khi xử lý tiếp. |
| Mức độ ưu tiên | Cao |
| Phạm vi | Quy trình xử lý đơn hàng bán lẻ |

## 2. Mô tả

Use Case mô tả quá trình nhân viên bán hàng kiểm tra thông tin do khách hàng cung cấp nhằm xác định thông tin đơn hàng đã đầy đủ và chính xác hay chưa.

## 3. Điều kiện tiên quyết (Preconditions)

- Yêu cầu đặt hàng đã được tiếp nhận thông qua UC-01.
- Thông tin đơn hàng ban đầu đã được ghi nhận.

## 4. Luồng sự kiện chính (Main Flow)

1. Nhân viên bán hàng mở thông tin đơn hàng đã tiếp nhận.
2. Nhân viên kiểm tra các thông tin liên quan đến đơn hàng.
3. Nhân viên xác định thông tin đã đầy đủ và chính xác.
4. Nhân viên chuyển sang bước kiểm tra tình trạng hàng hóa (UC-03).

## 5. Luồng thay thế (Alternative Flow)

**Trường hợp thông tin chưa đầy đủ hoặc chưa chính xác:**

1. Nhân viên bán hàng xác định thông tin cần bổ sung hoặc điều chỉnh.
2. Nhân viên liên hệ khách hàng để yêu cầu cập nhật.
3. Khách hàng cung cấp thông tin bổ sung.
4. Nhân viên kiểm tra lại thông tin.
5. Nếu thông tin đã đạt yêu cầu, tiếp tục UC-03.

## 6. Điều kiện hậu (Postconditions)

- Thông tin đơn hàng đã được kiểm tra.
- Nếu thông tin chưa đạt yêu cầu, đơn hàng được giữ lại để bổ sung trước khi tiếp tục xử lý.

## 7. Quy tắc nghiệp vụ liên quan

- BR-01: Thông tin đơn hàng cần được kiểm tra trước khi tiếp tục xử lý.

## 8. Điểm cần xác minh

- Những trường thông tin nào bắt buộc phải có?
- Tiêu chí nào được sử dụng để xác định thông tin hợp lệ?
- Có cơ chế cảnh báo khi thông tin bị thiếu hoặc sai hay không?
