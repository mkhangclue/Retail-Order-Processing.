# UC-03 – Đặc tả Use Case: Kiểm tra tình trạng hàng hóa

## 1. Thông tin chung

| Thuộc tính | Nội dung |
|---|---|
| Mã Use Case | UC-03 |
| Tên Use Case | Kiểm tra tình trạng hàng hóa |
| Tác nhân chính | Nhân viên bán hàng |
| Tác nhân phụ | Hệ thống quản lý tồn kho (cần xác minh) |
| Mục tiêu | Xác định sản phẩm khách hàng đặt có đủ số lượng tồn kho để đáp ứng đơn hàng hay không. |
| Mức độ ưu tiên | Cao |
| Phạm vi | Quy trình xử lý đơn hàng bán lẻ |

## 2. Mô tả

Use Case mô tả quá trình kiểm tra tình trạng tồn kho của sản phẩm trong đơn hàng nhằm xác định khả năng đáp ứng yêu cầu đặt hàng của khách hàng.

## 3. Điều kiện tiên quyết (Preconditions)

- Đơn hàng đã được tiếp nhận thông qua UC-01.
- Thông tin đơn hàng đã được kiểm tra thông qua UC-02.
- Có thông tin về sản phẩm và số lượng cần đặt.

## 4. Luồng sự kiện chính (Main Flow)

1. Nhân viên bán hàng xác định sản phẩm và số lượng khách hàng yêu cầu.
2. Nhân viên thực hiện kiểm tra tình trạng hàng hóa.
3. Hệ thống hoặc nguồn dữ liệu tồn kho cung cấp thông tin về số lượng hàng hiện có.
4. Nhân viên xác định sản phẩm có đủ số lượng đáp ứng đơn hàng.
5. Nếu hàng hóa còn đủ, nhân viên chuyển sang bước tiếp theo của quy trình.

## 5. Luồng thay thế (Alternative Flow)

**Trường hợp sản phẩm hết hàng hoặc không đủ số lượng:**

1. Nhân viên xác định sản phẩm không đáp ứng đủ số lượng yêu cầu.
2. Nhân viên thông báo tình trạng hàng hóa cho khách hàng.
3. Khách hàng lựa chọn hủy đơn hàng hoặc thay thế bằng sản phẩm khác.
4. Nếu khách hàng chọn sản phẩm thay thế, nhân viên thực hiện kiểm tra tình trạng hàng hóa lại.
5. Nếu khách hàng chọn hủy đơn, quy trình kết thúc với trạng thái đơn hàng đã hủy.

## 6. Điều kiện hậu (Postconditions)

- Tình trạng hàng hóa đã được xác định.
- Nếu đủ hàng, đơn hàng được chuyển sang bước xử lý tiếp theo.
- Nếu hết hàng, đơn hàng được xử lý theo lựa chọn của khách hàng.

## 7. Quy tắc nghiệp vụ liên quan

- BR-02: Cần kiểm tra tình trạng hàng hóa trước khi tiếp tục xử lý đơn hàng.
- BR-03: Khi sản phẩm hết hàng, khách hàng có thể lựa chọn hủy đơn hoặc thay thế bằng sản phẩm khác.

## 8. Điểm cần xác minh

- Nhân viên bán hàng kiểm tra tồn kho trên hệ thống nào?
- Dữ liệu tồn kho được cập nhật theo thời gian thực hay theo từng đợt?
- Ai chịu trách nhiệm cập nhật số lượng hàng tồn kho?
- Trường hợp chỉ còn một phần số lượng yêu cầu thì có cho phép đặt hàng một phần hay không?
