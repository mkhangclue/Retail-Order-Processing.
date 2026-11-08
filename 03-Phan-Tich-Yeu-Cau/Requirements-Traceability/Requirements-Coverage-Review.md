# Requirements Coverage Review

## 1. Mục đích

Đánh giá mức độ bao phủ của các yêu cầu chức năng so với quy trình BPMN gốc, nhằm xác định những hoạt động hoặc nhánh nghiệp vụ chưa được thể hiện đầy đủ trong bộ yêu cầu.

## 2. Bảng đánh giá

| STT | Hoạt động trong BPMN | Requirement ID | Mức độ bao phủ | Ghi chú |
|---|---|---|---|---|
| 1 | Tiếp nhận đơn hàng | FR-01 | Đã bao phủ | UC-01 |
| 2 | Kiểm tra thông tin đơn hàng | FR-02 | Đã bao phủ | UC-02 |
| 3 | Kiểm tra tình trạng hàng hóa | FR-03 | Đã bao phủ | UC-03 |
| 4 | Xử lý trường hợp hết hàng | FR-04 | Đã bao phủ | UC-04 |
| 5 | Kiểm tra và cập nhật thông tin giao hàng | FR-05 | Đã bao phủ | UC-05 |
| 6 | Xác nhận phương thức giao hàng | FR-06 | Đã bao phủ | UC-06 |
| 7 | Lập và hoàn thiện hóa đơn | FR-07 | Đã bao phủ | UC-07 |
| 8 | Xác nhận thanh toán trong thời hạn 2 ngày | FR-08 | Đã bao phủ | UC-08 |
| 9 | Kiểm tra và đóng gói hàng hóa | FR-09 | Đã bao phủ | UC-09 |
| 10 | Bàn giao cho đơn vị vận chuyển | FR-10 | Đã bao phủ | UC-10 |
| 11 | Cập nhật trạng thái giao hàng | FR-11 | Đã bao phủ | UC-11 |
| 12 | Xử lý giao hàng thất bại | FR-12 | Đã bao phủ | UC-12 |
| 13 | Tiếp nhận và kiểm tra khiếu nại | FR-12 | Đã bao phủ | UC-13, UC-14, UC-15 |
| 14 | Xử lý hàng hóa bị lỗi | FR-12 | Đã bao phủ | UC-16 |
| 15 | Chuẩn bị và gửi hàng thay thế | FR-12 | Đã bao phủ | UC-17 |
| 16 | Cập nhật kết quả xử lý khiếu nại | FR-12 | Đã bao phủ | UC-18 |

## 3. Các nội dung cần làm rõ

| ID | Nội dung | Lý do |
|---|---|---|
| OQ-01 | Cơ chế kiểm tra và cập nhật tồn kho | BPMN chưa mô tả rõ hệ thống hoặc bộ phận chịu trách nhiệm |
| OQ-02 | Cách xử lý khi khách hàng không xác nhận thanh toán trong 2 ngày | Chưa có nhánh xử lý quá hạn |
| OQ-03 | Số lần giao hàng lại tối đa | BPMN chưa quy định giới hạn |
| OQ-04 | Tiêu chí xác định khiếu nại hợp lệ | Chưa có tiêu chí đánh giá cụ thể |
| OQ-05 | Cách thức khách hàng gửi khiếu nại | Chưa xác định kênh tiếp nhận |

## 4. Kết luận

Bộ yêu cầu chức năng FR-01 đến FR-12 đã bao quát sơ bộ các hoạt động chính được thể hiện trong BPMN.

Tuy nhiên, việc bao phủ hoạt động nghiệp vụ không đồng nghĩa với việc mọi chức năng phần mềm đã được xác định đầy đủ. Các nội dung cần làm rõ sẽ được giữ lại trong danh sách Open Questions để tránh tự đưa ra giả định.
