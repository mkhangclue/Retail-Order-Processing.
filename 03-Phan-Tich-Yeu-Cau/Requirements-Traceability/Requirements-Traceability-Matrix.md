# Requirements Traceability Matrix (RTM)

## 1. Mục đích

Ma trận truy vết yêu cầu (RTM) được sử dụng để liên kết các yêu cầu nghiệp vụ, yêu cầu chức năng và Use Case với quy trình BPMN gốc.

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
| FR-03 | Kiểm tra tình trạng hàng hóa | BR-02 | UC-03 | BPMN – Kiểm tra tồn kho |
| FR-04 | Xử lý trường hợp hết hàng | BR-03 | UC-04 | BPMN – Nhánh hết hàng |
| FR-05 | Cập nhật thông tin giao hàng | BR-04 | UC-05 | BPMN – Yêu cầu và kiểm tra thông tin giao hàng |
| FR-06 | Xác nhận phương thức giao hàng | BR-05 | UC-06 | BPMN – Xác nhận phương thức giao hàng |
| FR-07 | Lập hóa đơn | BR-06 | UC-07 | BPMN – Lập và hoàn thiện hóa đơn |
| FR-08 | Ghi nhận xác nhận thanh toán | BR-07 | UC-08 | BPMN – Xác nhận thanh toán |
| FR-09 | Kiểm tra và đóng gói hàng hóa | BR-08 | UC-09 | BPMN – Kiểm tra và đóng gói |
| FR-10 | Bàn giao hàng cho đơn vị vận chuyển | BR-08 | UC-10 | BPMN – Bàn giao hàng |
| FR-11 | Cập nhật trạng thái giao hàng | BR-09 | UC-11 | BPMN – Cập nhật trạng thái giao hàng |
| FR-12 | Xử lý giao hàng thất bại và khiếu nại | BR-09, BR-10 | UC-12 đến UC-18 | BPMN – Nhánh giao thất bại và xử lý khiếu nại |

## 3. Ghi chú truy vết

- Các mã FR, BR và UC được sử dụng theo bộ tài liệu đã xây dựng trong dự án.
- Một yêu cầu có thể liên kết với nhiều Use Case.
- FR-12 hiện bao gồm nhiều hoạt động xử lý khác nhau. Có thể tách nhỏ trong lần rà soát yêu cầu tiếp theo nếu cần thiết.
- Một số chức năng và quan hệ giữa Actor với hệ thống vẫn cần được xác minh do BPMN chưa mô tả đầy đủ tương tác phần mềm.

## 4. Trạng thái

| Nội dung | Trạng thái |
|---|---|
| Liên kết FR với BR | Bản nháp |
| Liên kết FR với UC | Bản nháp |
| Đối chiếu với BPMN | Đã thực hiện sơ bộ |
| Xác nhận với Stakeholder | Chưa thực hiện |

**Lưu ý:** Đây là ma trận truy vết sơ bộ dựa trên BPMN và bộ yêu cầu đã xây dựng, chưa phải tài liệu yêu cầu đã được Stakeholder phê duyệt.
