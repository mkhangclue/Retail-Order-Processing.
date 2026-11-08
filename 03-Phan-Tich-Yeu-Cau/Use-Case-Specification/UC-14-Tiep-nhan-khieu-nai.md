# UC-14 – Đặc tả Use Case: Tiếp nhận khiếu nại

## 1. Thông tin chung

| Thuộc tính | Nội dung |
|---|---|
| Mã Use Case | UC-14 |
| Tên Use Case | Tiếp nhận khiếu nại |
| Tác nhân chính | Nhân viên chăm sóc khách hàng |
| Tác nhân phụ | Khách hàng |
| Mục tiêu | Tiếp nhận và ghi nhận đầy đủ thông tin khiếu nại để chuyển sang bước xác minh. |
| Mức độ ưu tiên | Cao |
| Phạm vi | Quy trình xử lý đơn hàng bán lẻ |

## 2. Mô tả

Use Case mô tả quá trình nhân viên chăm sóc khách hàng tiếp nhận phản ánh từ khách hàng về các vấn đề liên quan đến hàng hóa, kiểm tra thông tin ban đầu và ghi nhận nội dung khiếu nại để phục vụ quá trình xác minh.

## 3. Điều kiện tiên quyết (Preconditions)

- Khách hàng đã gửi khiếu nại thông qua UC-13.
- Thông tin đơn hàng có thể được sử dụng để đối chiếu.

## 4. Luồng sự kiện chính (Main Flow)

1. Nhân viên chăm sóc khách hàng tiếp nhận khiếu nại.
2. Nhân viên kiểm tra thông tin đơn hàng.
3. Nhân viên ghi nhận nội dung khiếu nại và loại vấn đề được phản ánh.
4. Nhân viên tiếp nhận hình ảnh hoặc bằng chứng liên quan từ khách hàng.
5. Nhân viên kiểm tra mức độ đầy đủ của thông tin.
6. Khiếu nại được chuyển sang UC-15 – Kiểm tra tính hợp lệ của khiếu nại.

## 5. Luồng thay thế (Alternative Flow)

**Trường hợp thông tin khiếu nại chưa đầy đủ:**

1. Nhân viên xác định thông tin hoặc bằng chứng còn thiếu.
2. Nhân viên liên hệ khách hàng để yêu cầu bổ sung.
3. Khách hàng cung cấp thông tin còn thiếu.
4. Nhân viên cập nhật hồ sơ khiếu nại và tiếp tục xử lý.

**Trường hợp không tìm thấy thông tin đơn hàng:**

1. Nhân viên yêu cầu khách hàng cung cấp thêm thông tin để đối chiếu.
2. Nhân viên kiểm tra lại thông tin đơn hàng.
3. Nếu vẫn chưa xác định được đơn hàng, khiếu nại được ghi nhận ở trạng thái chờ xác minh.

## 6. Điều kiện hậu (Postconditions)

- Thông tin khiếu nại đã được tiếp nhận và ghi nhận.
- Thông tin đơn hàng và bằng chứng liên quan được tập hợp để xác minh.
- Khiếu nại sẵn sàng chuyển sang bước kiểm tra tính hợp lệ.

## 7. Quy tắc nghiệp vụ liên quan

- BR-10: Khiếu nại liên quan đến hàng hóa bị thiếu, hư hỏng hoặc giao sai cần được kiểm tra bằng hình ảnh hoặc bằng chứng liên quan.

## 8. Điểm cần xác minh

- Nhân viên sử dụng hệ thống nào để ghi nhận khiếu nại?
- Những trường thông tin nào bắt buộc phải lưu?
- Có mã khiếu nại riêng để theo dõi không?
- Ai chịu trách nhiệm tiếp nhận khiếu nại khi nhân viên chăm sóc khách hàng không có mặt?
- Thời gian xử lý khiếu nại được quy định như thế nào?
