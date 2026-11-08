# Business Rules – Quy tắc nghiệp vụ

## 1. Mục đích

Tài liệu xác định các quy tắc nghiệp vụ chi phối quy trình xử lý đơn hàng bán lẻ, làm cơ sở cho việc phân tích yêu cầu và đề xuất quy trình TO-BE.

Các quy tắc được tổng hợp từ BPMN hiện tại. Những nội dung chưa được xác nhận sẽ được đánh dấu là cần làm rõ.

## 2. Danh sách quy tắc nghiệp vụ

### BR-01 – Kiểm tra thông tin đơn hàng

- Nội dung: Thông tin đơn hàng cần được kiểm tra trước khi tiếp tục xử lý.
- Căn cứ: Quy trình có bước kiểm tra thông tin hóa đơn và yêu cầu khách hàng cập nhật nếu thông tin chưa đầy đủ hoặc không chính xác.
- Trạng thái: Đã thể hiện trong BPMN.

### BR-02 – Kiểm tra tình trạng hàng hóa

- Nội dung: Tình trạng hàng hóa cần được kiểm tra trước khi xác nhận khả năng đáp ứng đơn hàng.
- Căn cứ: Subprocess có bước kiểm tra tình trạng hàng hóa trên hệ thống quản lý tồn kho.
- Trạng thái: Đã thể hiện trong BPMN.

### BR-03 – Xử lý khi hàng hóa không có sẵn

- Nội dung: Khi hàng hóa không có sẵn, khách hàng được lựa chọn hủy đơn hoặc chọn sản phẩm thay thế.
- Căn cứ: Subprocess kiểm tra thông tin đơn hàng.
- Trạng thái: Đã thể hiện trong BPMN.

### BR-04 – Kiểm tra thông tin giao hàng

- Nội dung: Thông tin giao hàng cần được kiểm tra. Nếu chưa đầy đủ, khách hàng phải bổ sung hoặc cập nhật.
- Căn cứ: Subprocess có bước kiểm tra thông tin và vòng lặp yêu cầu cập nhật.
- Trạng thái: Đã thể hiện trong BPMN.

### BR-05 – Xác nhận phương thức giao hàng

- Nội dung: Phương thức giao hàng cần được xác nhận trước khi hoàn tất xử lý đơn hàng.
- Căn cứ: Quy trình chính có bước nhân viên bán hàng xác nhận phương thức giao hàng.
- Trạng thái: Đã thể hiện trong BPMN.

### BR-06 – Xử lý bảo hiểm hàng hóa

- Nội dung: Nếu đơn hàng thuộc trường hợp có bảo hiểm, phí và thông tin bảo hiểm cần được bổ sung vào hóa đơn.
- Căn cứ: Quy trình chính có nhánh quyết định về bảo hiểm.
- Trạng thái: Đã thể hiện trong BPMN.

### BR-07 – Xác nhận thanh toán

- Nội dung: Khách hàng gửi xác nhận thanh toán trong thời hạn 2 ngày theo mô tả quy trình.
- Căn cứ: Quy trình chính.
- Trạng thái: Đã thể hiện trong BPMN; chưa rõ cách xử lý khi quá hạn.

### BR-08 – Kiểm tra và đóng gói hàng hóa

- Nội dung: Nhân viên kho kiểm tra thông tin đơn hàng trước khi đóng gói và bàn giao cho đơn vị vận chuyển.
- Căn cứ: Quy trình chính.
- Trạng thái: Đã thể hiện trong BPMN.

### BR-09 – Xử lý giao hàng thất bại

- Nội dung: Khi giao hàng thất bại, bộ phận chăm sóc khách hàng liên hệ khách hàng và phối hợp kiểm tra để quyết định hướng xử lý tiếp theo.
- Căn cứ: Quy trình chính.
- Trạng thái: Đã thể hiện trong BPMN; chưa rõ số lần giao lại tối đa.

### BR-10 – Xử lý khiếu nại

- Nội dung: Khi khách hàng khiếu nại về hàng hóa thiếu, hư hỏng hoặc giao sai, cần thu thập hình ảnh và kiểm tra bằng chứng trước khi quyết định xử lý.
- Căn cứ: Quy trình chính.
- Trạng thái: Đã thể hiện trong BPMN; chưa có tiêu chí đánh giá khiếu nại chi tiết.

## 3. Các quy tắc cần làm rõ

| ID | Nội dung cần xác minh |
|---|---|
| OQ-BR-01 | Những trường thông tin nào bắt buộc đối với đơn hàng? |
| OQ-BR-02 | Tiêu chí nào xác định thông tin giao hàng hợp lệ? |
| OQ-BR-03 | Ai chịu trách nhiệm xác nhận tình trạng tồn kho? |
| OQ-BR-04 | Điều gì xảy ra khi khách hàng không thanh toán trong 2 ngày? |
| OQ-BR-05 | Đơn hàng được phép giao lại tối đa bao nhiêu lần? |
| OQ-BR-06 | Những tiêu chí nào được sử dụng để xác định khiếu nại hợp lệ? |
| OQ-BR-07 | Ai có quyền quyết định phương án xử lý khiếu nại? |

## 4. Định hướng sử dụng

Các quy tắc BR-01 đến BR-10 được tổng hợp từ mô hình BPMN.

Các câu hỏi OQ-BR-01 đến OQ-BR-07 sẽ được sử dụng để bổ sung thông tin trong giai đoạn xác minh yêu cầu.

Sau khi xác minh, các quy tắc sẽ được cập nhật và sử dụng làm cơ sở xây dựng Business Requirements và quy trình TO-BE.
