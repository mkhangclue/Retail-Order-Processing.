# UC-05 – Đặc tả Use Case: Cập nhật thông tin giao hàng

## 1. Thông tin chung

| Thuộc tính | Nội dung |
|---|---|
| Mã Use Case | UC-05 |
| Tên Use Case | Cập nhật thông tin giao hàng |
| Tác nhân chính | Nhân viên bán hàng |
| Tác nhân phụ | Khách hàng |
| Mục tiêu | Thu thập và hoàn thiện thông tin cần thiết để phục vụ việc giao hàng. |
| Mức độ ưu tiên | Cao |
| Phạm vi | Quy trình xử lý đơn hàng bán lẻ |

## 2. Mô tả

Use Case mô tả quá trình nhân viên bán hàng yêu cầu khách hàng cung cấp thông tin giao hàng, kiểm tra tính đầy đủ của thông tin và cập nhật thông tin vào đơn hàng.

## 3. Điều kiện tiên quyết (Preconditions)

- Đơn hàng đã được tiếp nhận.
- Sản phẩm đã được xác định có thể đáp ứng yêu cầu đặt hàng.
- Khách hàng đã lựa chọn tiếp tục mua hàng.

## 4. Luồng sự kiện chính (Main Flow)

1. Nhân viên bán hàng yêu cầu khách hàng cung cấp thông tin giao hàng.
2. Khách hàng cung cấp thông tin người nhận, địa chỉ và số điện thoại.
3. Nhân viên bán hàng tiếp nhận thông tin.
4. Nhân viên kiểm tra tính đầy đủ của thông tin.
5. Nhân viên cập nhật thông tin giao hàng vào đơn hàng.
6. Quy trình chuyển sang bước xác nhận phương thức giao hàng (UC-06).

## 5. Luồng thay thế (Alternative Flow)

**Trường hợp thông tin giao hàng chưa đầy đủ hoặc không chính xác:**

1. Nhân viên bán hàng xác định thông tin cần bổ sung hoặc điều chỉnh.
2. Nhân viên yêu cầu khách hàng cập nhật thông tin.
3. Khách hàng cung cấp lại thông tin.
4. Nhân viên kiểm tra lại thông tin.
5. Nếu thông tin đã đầy đủ, tiếp tục luồng chính.

## 6. Điều kiện hậu (Postconditions)

- Thông tin giao hàng đã được cập nhật vào đơn hàng.
- Nếu thông tin chưa đạt yêu cầu, đơn hàng chờ bổ sung trước khi tiếp tục xử lý.

## 7. Quy tắc nghiệp vụ liên quan

- BR-04: Thông tin giao hàng cần được kiểm tra và yêu cầu cập nhật nếu chưa đầy đủ.

## 8. Điểm cần xác minh

- Những trường thông tin giao hàng nào là bắt buộc?
- Có tiêu chí cụ thể để xác định địa chỉ và số điện thoại hợp lệ không?
- Khách hàng có thể thay đổi thông tin giao hàng sau khi xác nhận đơn hàng không?
- Nhân viên nào chịu trách nhiệm cập nhật thông tin khi có thay đổi?
