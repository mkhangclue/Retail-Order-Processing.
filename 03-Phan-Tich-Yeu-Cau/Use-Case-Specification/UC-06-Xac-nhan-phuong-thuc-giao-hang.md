# UC-06 – Đặc tả Use Case: Xác nhận phương thức giao hàng

## 1. Thông tin chung

| Thuộc tính | Nội dung |
|---|---|
| Mã Use Case | UC-06 |
| Tên Use Case | Xác nhận phương thức giao hàng |
| Tác nhân chính | Nhân viên bán hàng |
| Tác nhân phụ | Khách hàng |
| Mục tiêu | Xác nhận phương thức giao hàng phù hợp với yêu cầu của khách hàng. |
| Mức độ ưu tiên | Cao |
| Phạm vi | Quy trình xử lý đơn hàng bán lẻ |

## 2. Mô tả

Use Case mô tả quá trình nhân viên bán hàng trao đổi và xác nhận phương thức giao hàng với khách hàng, làm cơ sở cho việc lập hóa đơn và tổ chức giao hàng.

## 3. Điều kiện tiên quyết (Preconditions)

- Thông tin đơn hàng đã được kiểm tra.
- Tình trạng hàng hóa đã được xác định.
- Thông tin giao hàng đã được cập nhật thông qua UC-05.

## 4. Luồng sự kiện chính (Main Flow)

1. Nhân viên bán hàng trao đổi với khách hàng về phương thức giao hàng.
2. Nhân viên tiếp nhận lựa chọn của khách hàng.
3. Nhân viên xác nhận phương thức giao hàng.
4. Nhân viên ghi nhận phương thức giao hàng vào thông tin đơn hàng.
5. Quy trình chuyển sang bước lập hóa đơn (UC-07).

## 5. Luồng thay thế (Alternative Flow)

**Trường hợp khách hàng thay đổi phương thức giao hàng:**

1. Khách hàng đề nghị thay đổi phương thức giao hàng.
2. Nhân viên bán hàng kiểm tra khả năng đáp ứng phương thức mới.
3. Hai bên thống nhất phương thức giao hàng phù hợp.
4. Nhân viên cập nhật lại thông tin đơn hàng.

## 6. Điều kiện hậu (Postconditions)

- Phương thức giao hàng đã được xác nhận và ghi nhận trong đơn hàng.
- Đơn hàng sẵn sàng chuyển sang bước lập hóa đơn.

## 7. Quy tắc nghiệp vụ liên quan

- BR-05: Phương thức giao hàng cần được xác nhận trước khi hoàn thiện quá trình xử lý đơn hàng.

## 8. Điểm cần xác minh

- Doanh nghiệp hiện hỗ trợ những phương thức giao hàng nào?
- Khách hàng có được lựa chọn đơn vị vận chuyển không?
- Phương thức giao hàng có ảnh hưởng đến phí vận chuyển không?
- Ai có quyền quyết định phương thức giao hàng cuối cùng?
