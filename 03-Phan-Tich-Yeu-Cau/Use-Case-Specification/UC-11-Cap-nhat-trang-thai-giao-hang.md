# UC-11 – Đặc tả Use Case: Cập nhật trạng thái giao hàng

## 1. Thông tin chung

| Thuộc tính | Nội dung |
|---|---|
| Mã Use Case | UC-11 |
| Tên Use Case | Cập nhật trạng thái giao hàng |
| Tác nhân chính | Đơn vị vận chuyển |
| Tác nhân phụ | Nhân viên chăm sóc khách hàng |
| Mục tiêu | Cập nhật tiến trình giao hàng để doanh nghiệp theo dõi và xử lý đơn hàng kịp thời. |
| Mức độ ưu tiên | Cao |
| Phạm vi | Quy trình xử lý đơn hàng bán lẻ |

## 2. Mô tả

Use Case mô tả quá trình đơn vị vận chuyển cập nhật trạng thái đơn hàng trong quá trình giao hàng. Thông tin trạng thái được sử dụng để theo dõi tiến trình và xác định kết quả giao hàng.

## 3. Điều kiện tiên quyết (Preconditions)

- Kiện hàng đã được bàn giao cho đơn vị vận chuyển thông qua UC-10.
- Đơn vị vận chuyển đã tiếp nhận thông tin giao hàng.
- Quá trình vận chuyển đã bắt đầu.

## 4. Luồng sự kiện chính (Main Flow)

1. Đơn vị vận chuyển tiếp nhận đơn hàng cần giao.
2. Đơn vị vận chuyển cập nhật trạng thái đơn hàng trong quá trình vận chuyển.
3. Hệ thống hoặc bên phụ trách tiếp nhận thông tin trạng thái.
4. Khi giao hàng thành công, đơn vị vận chuyển cập nhật trạng thái "Đã giao thành công".
5. Kết quả giao hàng được chuyển đến bộ phận chăm sóc khách
