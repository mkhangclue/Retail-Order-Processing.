# UC-01 – Đặc tả Use Case: Tiếp nhận đơn hàng

## 1. Thông tin chung

| Thuộc tính | Nội dung |
|---|---|
| Mã Use Case | UC-01 |
| Tên Use Case | Tiếp nhận đơn hàng |
| Tác nhân chính | Nhân viên bán hàng |
| Mục tiêu | Tiếp nhận yêu cầu đặt hàng từ khách hàng và ghi nhận thông tin đơn hàng ban đầu. |
| Mức độ ưu tiên | Cao |
| Phạm vi | Quy trình xử lý đơn hàng bán lẻ |

## 2. Mô tả

Use Case mô tả quá trình nhân viên bán hàng tiếp nhận yêu cầu đặt hàng từ khách hàng, ghi nhận thông tin ban đầu và chuyển sang bước kiểm tra thông tin đơn hàng.

## 3. Điều kiện tiên quyết (Preconditions)

- Khách hàng có nhu cầu đặt mua sản phẩm.
- Nhân viên bán hàng sẵn sàng tiếp nhận yêu cầu đặt hàng.

## 4. Luồng sự kiện chính (Main Flow)

1. Khách hàng gửi yêu cầu đặt hàng.
2. Nhân viên bán hàng tiếp nhận yêu cầu.
3. Nhân viên bán hàng ghi nhận thông tin đơn hàng ban đầu.
4. Nhân viên bán hàng chuyển sang bước kiểm tra thông tin đơn hàng (UC-02).

## 5. Luồng thay thế (Alternative Flow)

- Nếu khách hàng chưa cung cấp đủ thông tin ban đầu, nhân viên bán hàng trao đổi để bổ sung thông tin trước khi tiếp tục.

## 6. Điều kiện hậu (Postconditions)

- Yêu cầu đặt hàng đã được tiếp nhận.
- Thông tin đơn hàng ban đầu được ghi nhận để phục vụ bước kiểm tra tiếp theo.

## 7. Quy tắc nghiệp vụ liên quan

- BR-01: Thông tin đơn hàng cần được kiểm tra trước khi tiếp tục xử lý.

## 8. Điểm cần xác minh

- Những kênh nào được sử dụng để tiếp nhận đơn hàng?
- Những thông tin nào cần ghi nhận ngay khi tiếp nhận đơn hàng?
- Nhân viên bán hàng ghi nhận đơn hàng trên hệ thống nào?
