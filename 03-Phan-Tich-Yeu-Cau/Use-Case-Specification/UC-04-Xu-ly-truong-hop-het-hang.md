# UC-04 – Đặc tả Use Case: Xử lý trường hợp hết hàng

## 1. Thông tin chung

| Thuộc tính | Nội dung |
|---|---|
| Mã Use Case | UC-04 |
| Tên Use Case | Xử lý trường hợp hết hàng |
| Tác nhân chính | Nhân viên bán hàng |
| Tác nhân phụ | Khách hàng |
| Mục tiêu | Xử lý yêu cầu đặt hàng khi sản phẩm không còn đủ số lượng trong kho. |
| Mức độ ưu tiên | Cao |
| Phạm vi | Quy trình xử lý đơn hàng bán lẻ |

## 2. Mô tả

Use Case mô tả quá trình nhân viên bán hàng thông báo tình trạng hết hàng cho khách hàng và ghi nhận lựa chọn của khách hàng về việc hủy đơn hoặc thay thế bằng sản phẩm khác.

## 3. Điều kiện tiên quyết (Preconditions)

- Đơn hàng đã được tiếp nhận.
- Thông tin đơn hàng đã được kiểm tra.
- Kết quả kiểm tra tồn kho cho thấy sản phẩm không đủ số lượng hoặc đã hết hàng thông qua UC-03.

## 4. Luồng sự kiện chính (Main Flow)

1. Nhân viên bán hàng xác định sản phẩm không đáp ứng được số lượng yêu cầu.
2. Nhân viên thông báo tình trạng hàng hóa cho khách hàng.
3. Nhân viên đề nghị khách hàng lựa chọn phương án xử lý.
4. Khách hàng lựa chọn hủy đơn hàng hoặc thay thế bằng sản phẩm khác.
5. Nhân viên ghi nhận lựa chọn của khách hàng.

## 5. Luồng thay thế (Alternative Flow)

**Trường hợp 1: Khách hàng chọn hủy đơn hàng**

1. Nhân viên ghi nhận yêu cầu hủy đơn.
2. Đơn hàng được chuyển sang trạng thái hủy.
3. Quy trình xử lý đơn hàng kết thúc.

**Trường hợp 2: Khách hàng chọn sản phẩm thay thế**

1. Nhân viên ghi nhận sản phẩm thay thế.
2. Nhân viên thực hiện kiểm tra tình trạng tồn kho của sản phẩm mới thông qua UC-03.
3. Nếu sản phẩm mới còn đủ hàng, quy trình tiếp tục.
4. Nếu sản phẩm mới vẫn hết hàng, nhân viên tiếp tục trao đổi với khách hàng để lựa chọn phương án khác.

## 6. Điều kiện hậu (Postconditions)

- Lựa chọn xử lý của khách hàng đã được ghi nhận.
- Đơn hàng được hủy hoặc tiếp tục xử lý với sản phẩm thay thế.

## 7. Quy tắc nghiệp vụ liên quan

- BR-02: Cần kiểm tra tình trạng hàng hóa trước khi tiếp tục xử lý đơn hàng.
- BR-03: Khi sản phẩm hết hàng, khách hàng có thể lựa chọn hủy đơn hoặc thay thế bằng sản phẩm khác.

## 8. Điểm cần xác minh

- Nhân viên bán hàng có quyền đề xuất sản phẩm thay thế hay không?
- Có yêu cầu khách hàng xác nhận lại giá bán khi thay thế sản phẩm không?
- Khi khách hàng hủy đơn, quy trình hoàn tiền được thực hiện như thế nào nếu đã thanh toán?
- Có giới hạn số lần lựa chọn sản phẩm thay thế hay không?
