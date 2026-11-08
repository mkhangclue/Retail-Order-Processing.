# UC-18 – Đặc tả Use Case: Cập nhật kết quả xử lý khiếu nại

## 1. Thông tin chung

| Thuộc tính | Nội dung |
|---|---|
| Mã Use Case | UC-18 |
| Tên Use Case | Cập nhật kết quả xử lý khiếu nại |
| Tác nhân chính | Nhân viên chăm sóc khách hàng |
| Tác nhân phụ | Khách hàng |
| Mục tiêu | Cập nhật và thông báo kết quả xử lý khiếu nại cho khách hàng. |
| Mức độ ưu tiên | Cao |
| Phạm vi | Quy trình xử lý đơn hàng bán lẻ |

## 2. Mô tả

Use Case mô tả quá trình nhân viên chăm sóc khách hàng tiếp nhận kết quả xử lý từ các bộ phận liên quan, cập nhật tình trạng khiếu nại và thông báo kết quả cho khách hàng.

## 3. Điều kiện tiên quyết (Preconditions)

- Khiếu nại đã được tiếp nhận và xác minh thông qua UC-14 và UC-15.
- Kết quả xử lý từ các bộ phận liên quan đã được cung cấp.
- Nếu có hàng thay thế, thông tin giao hàng được tiếp nhận từ UC-17.

## 4. Luồng sự kiện chính (Main Flow)

1. Nhân viên chăm sóc khách hàng tiếp nhận kết quả xử lý khiếu nại.
2. Nhân viên kiểm tra thông tin và kết quả từ các bộ phận liên quan.
3. Nhân viên cập nhật trạng thái xử lý khiếu nại.
4. Nhân viên thông báo kết quả cho khách hàng.
5. Nhân viên ghi nhận thông tin đã thông báo.
6. Quy trình xử lý khiếu nại kết thúc khi kết quả được ghi nhận và thông báo theo quy trình.

## 5. Luồng thay thế (Alternative Flow)

**Trường hợp chưa có kết quả xử lý cuối cùng:**

1. Nhân viên kiểm tra tình trạng xử lý từ bộ phận liên quan.
2. Nhân viên ghi nhận khiếu nại đang chờ xử lý.
3. Nhân viên tiếp tục theo dõi cho đến khi có kết quả.

**Trường hợp khách hàng chưa nhận được hàng thay thế:**

1. Nhân viên kiểm tra trạng thái giao hàng.
2. Nhân viên phối hợp với đơn vị vận chuyển để xác minh.
3. Nhân viên cập nhật thông tin mới nhất cho khách hàng.

## 6. Điều kiện hậu (Postconditions)

- Kết quả xử lý khiếu nại được cập nhật.
- Khách hàng được thông báo về kết quả xử lý.
- Thông tin khiếu nại được lưu lại để phục vụ việc theo dõi và tra cứu.

## 7. Quy tắc nghiệp vụ liên quan

- BR-09: Bộ phận chăm sóc khách hàng phối hợp xử lý các tình huống phát sinh trong quá trình giao hàng.
- BR-10: Khiếu nại cần được xác minh trước khi thực hiện hướng xử lý tiếp theo.

## 8. Điểm cần xác minh

- Những trạng thái nào được sử dụng để theo dõi khiếu nại?
- Ai xác nhận khiếu nại đã được xử lý hoàn tất?
- Khách hàng được thông báo qua những kênh nào?
- Có cần lưu lịch sử trao đổi và kết quả xử lý không?
- Trường hợp khách hàng không đồng ý với kết quả xử lý thì quy trình tiếp theo là gì?
