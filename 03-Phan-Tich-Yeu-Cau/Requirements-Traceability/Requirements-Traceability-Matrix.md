# Requirements Traceability Matrix (RTM)

## 1. Mục đích

Ma trận truy vết yêu cầu (RTM) được sử dụng để liên kết các yêu cầu chức năng, quy tắc nghiệp vụ và Use Case với quy trình BPMN gốc.

Mục đích:
- Đảm bảo các yêu cầu có nguồn gốc rõ ràng.
- Kiểm tra mức độ bao phủ của các Use Case.
- Hỗ trợ phát hiện yêu cầu chưa được mô hình hóa.
- Hạn chế việc bổ sung chức năng không có căn cứ.

## 2. Ma trận truy vết yêu cầu

| Requirement ID | Requirement | Business Rule | Use Case | Nguồn tham chiếu |
|---|---|---|---|---|
| FR-01 | Tiếp nhận đơn hàng | BR-01 | UC-01 | BPMN – Tiếp nhận đơn hàng |
| FR-02 | Kiểm tra thông tin đơn hàng | BR-01 | UC-02 | BPMN – Kiểm tra thông tin đơn hàng |
| FR-03 | Kiểm tra tồn kho | BR-02 | UC-03 | BPMN – Kiểm tra tình trạng hàng hóa |
| FR-04 | Xử lý hàng hóa không có sẵn | BR-03 | UC-04 | BPMN – Nhánh hết hàng |
| FR-05 | Kiểm tra thông tin giao hàng | BR-04 | UC-05 | BPMN – Kiểm tra thông tin giao hàng |
| FR-06 | Cập nhật thông tin giao hàng | BR-04 | UC-05 | BPMN – Yêu cầu cập nhật thông tin |
| FR-07 | Quản lý hóa đơn | BR-06 | UC-07 | BPMN – Lập và hoàn thiện hóa đơn |
| FR-08 | Ghi nhận thanh toán | BR-07 | UC-08 | BPMN – Xác nhận thanh toán |
| FR-09 | Theo dõi trạng thái giao hàng | BR-08 | UC-11 | BPMN – Cập nhật trạng thái giao hàng |
| FR-10 | Xử lý giao hàng thất bại | BR-09 | UC-12 | BPMN – Nhánh giao hàng thất bại |
| FR-11 | Tiếp nhận khiếu nại | BR-10 | UC-13, UC-14, UC-15 | BPMN – Tiếp nhận và kiểm tra khiếu nại |
| FR-12 | Theo dõi kết quả xử lý khiếu nại | BR-10 | UC-16, UC-17, UC-18 | BPMN – Xử lý và cập nhật kết quả khiếu nại |
| FR-13 | Xác nhận phương thức giao hàng | BR-05 | UC-06 | BPMN – Xác nhận phương thức giao hàng |
| FR-14 | Quản lý thông tin bảo hiểm hàng hóa | BR-06 | UC-07, UC-09 | BPMN – Xác nhận bảo hiểm và đóng gói theo chính sách |
| FR-15 | Kiểm tra và đóng gói hàng hóa | BR-08 | UC-09 | BPMN – Kiểm tra và đóng gói hàng hóa |

## 3. Ghi chú truy vết

- Các mã FR, BR và UC được sử dụng theo bộ tài liệu hiện tại của dự án.
- Một yêu cầu có thể liên kết với nhiều Use Case và ngược lại.
- FR-14 liên quan đến thông tin bảo hiểm, phí bảo hiểm và quy cách đóng gói theo chính sách.
- Các quan hệ truy vết phản ánh sự liên kết nghiệp vụ, không khẳng định tất cả chức năng đã được triển khai trên một hệ thống phần mềm.
- Một số chức năng và quan hệ giữa Actor với hệ thống vẫn cần được xác minh do BPMN chưa mô tả đầy đủ tương tác phần mềm.

## 4. Trạng thái

| Nội dung | Trạng thái |
|---|---|
| Liên kết FR với BR | Bản nháp |
| Liên kết FR với UC | Bản nháp |
| Đối chiếu với BPMN | Đã thực hiện sơ bộ |
| Xác nhận với Stakeholder | Chưa thực hiện |

**Lưu ý:** Đây là ma trận truy vết sơ bộ dựa trên BPMN và bộ yêu cầu đã xây dựng, chưa phải tài liệu yêu cầu đã được Stakeholder phê duyệt.
