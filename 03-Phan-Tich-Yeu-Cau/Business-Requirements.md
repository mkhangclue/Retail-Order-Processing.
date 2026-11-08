# Business Requirements – Yêu cầu nghiệp vụ

## 1. Mục đích

Tài liệu xác định các yêu cầu cần đáp ứng nhằm hỗ trợ quá trình xử lý đơn hàng bán lẻ, tập trung vào việc tiếp nhận thông tin, kiểm tra hàng hóa, xác nhận đơn hàng, giao hàng và xử lý các trường hợp ngoại lệ.

Các yêu cầu dưới đây là đề xuất phục vụ phân tích và cải tiến quy trình, chưa phải yêu cầu đã được doanh nghiệp xác nhận.

## 2. Functional Requirements (FR)

| ID | Tên yêu cầu | Mô tả | Mức độ ưu tiên |
|---|---|---|---|
| FR-01 | Tiếp nhận đơn hàng | Quy trình cần hỗ trợ ghi nhận thông tin đơn hàng từ khách hàng. | High |
| FR-02 | Kiểm tra thông tin đơn hàng | Cho phép kiểm tra tính đầy đủ và chính xác của thông tin đơn hàng. | High |
| FR-03 | Kiểm tra tồn kho | Hỗ trợ kiểm tra tình trạng hàng hóa trước khi xác nhận khả năng đáp ứng đơn hàng. | High |
| FR-04 | Xử lý hàng hóa không có sẵn | Hỗ trợ ghi nhận lựa chọn hủy đơn hoặc chọn sản phẩm thay thế. | Medium |
| FR-05 | Kiểm tra thông tin giao hàng | Hỗ trợ kiểm tra thông tin người nhận, địa chỉ và số điện thoại. | High |
| FR-06 | Cập nhật thông tin giao hàng | Cho phép cập nhật thông tin khi phát hiện dữ liệu chưa đầy đủ hoặc không chính xác. | High |
| FR-07 | Quản lý hóa đơn | Hỗ trợ lập và cập nhật thông tin hóa đơn theo đơn hàng. | High |
| FR-08 | Ghi nhận thanh toán | Hỗ trợ ghi nhận trạng thái xác nhận thanh toán. | High |
| FR-09 | Theo dõi trạng thái giao hàng | Hỗ trợ cập nhật và theo dõi trạng thái giao hàng. | High |
| FR-10 | Xử lý giao hàng thất bại | Hỗ trợ ghi nhận kết quả giao thất bại và hướng xử lý tiếp theo. | High |
| FR-11 | Tiếp nhận khiếu nại | Hỗ trợ ghi nhận loại khiếu nại và bằng chứng từ khách hàng. | Medium |
| FR-12 | Theo dõi kết quả xử lý khiếu nại | Hỗ trợ cập nhật kết quả xác minh và phương án giải quyết. | Medium |
| FR-13 | Xác nhận phương thức giao hàng | Hỗ trợ ghi nhận phương thức giao hàng được lựa chọn và xác nhận cho đơn hàng. | High |
| FR-14 | Quản lý thông tin bảo hiểm hàng hóa | Hỗ trợ ghi nhận lựa chọn bảo hiểm, thông tin bảo hiểm và khoản phí bảo hiểm (nếu có). | Medium |
| FR-15 | Kiểm tra và đóng gói hàng hóa | Hỗ trợ kiểm tra thông tin đơn hàng, tình trạng hàng hóa và thực hiện đóng gói theo yêu cầu trước khi bàn giao cho đơn vị vận chuyển. | High |
## 3. Non-functional Requirements (NFR)

| ID | Tên yêu cầu | Mô tả |
|---|---|---|
| NFR-01 | Tính chính xác | Thông tin đơn hàng cần được ghi nhận chính xác và nhất quán. |
| NFR-02 | Tính dễ sử dụng | Giao diện hoặc biểu mẫu cần dễ hiểu và thuận tiện cho nhân viên sử dụng. |
| NFR-03 | Tính bảo mật | Thông tin khách hàng cần được bảo vệ và chỉ người có quyền mới được truy cập. |
| NFR-04 | Tính sẵn sàng | Hệ thống cần sẵn sàng phục vụ hoạt động xử lý đơn hàng. |
| NFR-05 | Khả năng truy vết | Cần có khả năng theo dõi lịch sử cập nhật và trạng thái xử lý đơn hàng. |

## 4. Traceability – Liên kết với Business Rules

| Business Rule | Business Requirement |
|---|---|
| BR-01 | FR-01, FR-02 |
| BR-02 | FR-03 |
| BR-03 | FR-04 |
| BR-04 | FR-05, FR-06 |
| BR-05 | FR-07, FR-09 |
| BR-06 | FR-07 |
| BR-07 | FR-08 |
| BR-08 | FR-09 |
| BR-09 | FR-10 |
| BR-10 | FR-11, FR-12 |

## 5. Các nội dung cần xác minh

- Hệ thống hiện tại có hỗ trợ đầy đủ các chức năng trên hay không?
- Có cần xây dựng hệ thống mới hay chỉ cải tiến quy trình hiện tại?
- Những vai trò nào được phép cập nhật thông tin đơn hàng?
- Có yêu cầu cụ thể về thời gian phản hồi và thời gian xử lý không?
- Có quy định về quyền truy cập và lưu trữ thông tin khách hàng không?

## 6. Ghi chú

Danh sách FR và NFR là đề xuất ban đầu dựa trên quy trình BPMN và các vấn đề đã phân tích.

Các yêu cầu cần được xác minh với stakeholder trước khi chuyển thành đặc tả yêu cầu chính thức.
