# Requirements Coverage Review

## 1. Mục đích

Đánh giá mức độ bao phủ của các yêu cầu chức năng so với quy trình BPMN gốc, nhằm xác định những hoạt động nghiệp vụ đã được thể hiện trong bộ yêu cầu và những nội dung vẫn cần làm rõ.

## 2. Bảng đánh giá mức độ bao phủ

| STT | Hoạt động trong BPMN | Requirement ID | Use Case | Mức độ bao phủ |
|---|---|---|---|---|
| 1 | Tiếp nhận đơn hàng | FR-01 | UC-01 | Đã bao phủ |
| 2 | Kiểm tra thông tin đơn hàng | FR-02 | UC-02 | Đã bao phủ |
| 3 | Kiểm tra tình trạng hàng hóa | FR-03 | UC-03 | Đã bao phủ |
| 4 | Xử lý trường hợp hết hàng | FR-04 | UC-04 | Đã bao phủ |
| 5 | Kiểm tra thông tin giao hàng | FR-05 | UC-05 | Đã bao phủ |
| 6 | Cập nhật thông tin giao hàng | FR-06 | UC-05 | Đã bao phủ |
| 7 | Lập và hoàn thiện hóa đơn | FR-07 | UC-07 | Đã bao phủ |
| 8 | Ghi nhận xác nhận thanh toán | FR-08 | UC-08 | Đã bao phủ |
| 9 | Xác nhận phương thức giao hàng | FR-13 | UC-06 | Đã bao phủ |
| 10 | Quản lý thông tin bảo hiểm hàng hóa | FR-14 | UC-07, UC-09 | Đã bao phủ sơ bộ |
| 11 | Kiểm tra và đóng gói hàng hóa | FR-15 | UC-09 | Đã bao phủ |
| 12 | Bàn giao hàng cho đơn vị vận chuyển | Chưa có FR riêng | UC-10 | Chưa có yêu cầu riêng |
| 13 | Cập nhật trạng thái giao hàng | FR-09 | UC-11 | Đã bao phủ |
| 14 | Xử lý giao hàng thất bại | FR-10 | UC-12 | Đã bao phủ |
| 15 | Tiếp nhận khiếu nại | FR-11 | UC-13, UC-14 | Đã bao phủ |
| 16 | Kiểm tra tính hợp lệ của khiếu nại | FR-11 | UC-15 | Đã bao phủ sơ bộ |
| 17 | Xử lý hàng hóa bị lỗi | FR-12 | UC-16 | Đã bao phủ sơ bộ |
| 18 | Chuẩn bị và gửi hàng thay thế | FR-12 | UC-17 | Đã bao phủ sơ bộ |
| 19 | Cập nhật kết quả xử lý khiếu nại | FR-12 | UC-18 | Đã bao phủ |

## 3. Các nội dung cần làm rõ

| ID | Nội dung | Lý do |
|---|---|---|
| OQ-01 | Cơ chế kiểm tra và cập nhật tồn kho | BPMN chưa mô tả rõ hệ thống hoặc bộ phận chịu trách nhiệm |
| OQ-02 | Cách xử lý khi khách hàng không xác nhận thanh toán trong 2 ngày | Chưa có nhánh xử lý quá hạn |
| OQ-03 | Số lần giao hàng lại tối đa | BPMN chưa quy định giới hạn |
| OQ-04 | Tiêu chí xác định khiếu nại hợp lệ | Chưa có tiêu chí đánh giá cụ thể |
| OQ-05 | Cách thức khách hàng gửi khiếu nại | Chưa xác định kênh tiếp nhận |
| OQ-06 | Quy trình và thông tin xác nhận bàn giao hàng | BPMN có hoạt động bàn giao nhưng chưa mô tả chi tiết cách xác nhận |

## 4. Kết luận

Bộ yêu cầu chức năng hiện tại đã bao quát phần lớn các hoạt động chính trong BPMN.

Tuy nhiên, hoạt động bàn giao hàng cho đơn vị vận chuyển chưa có yêu cầu chức năng riêng. Một số yêu cầu liên quan đến bảo hiểm và xử lý khiếu nại mới được bao phủ ở mức tổng quát, cần tiếp tục làm rõ.

Việc một hoạt động đã được liên kết với Requirement ID không đồng nghĩa với việc yêu cầu đã đủ chi tiết để triển khai hoặc kiểm thử.

**Trạng thái:** Preliminary Review – Đánh giá sơ bộ.
