# Solution Requirements – Yêu cầu giải pháp

## 1. Mục đích

Tài liệu xác định các yêu cầu giải pháp nhằm giải quyết những vấn đề được ghi nhận trong quá trình phân tích GAP.

Các yêu cầu này là cơ sở để định hướng thiết kế và đánh giá giải pháp cải tiến quy trình xử lý đơn hàng bán lẻ.

## 2. Danh sách yêu cầu giải pháp

### SR-01 – Kiểm soát thông tin tồn kho

- Hệ thống cần hỗ trợ ghi nhận kết quả kiểm tra tình trạng hàng hóa.
- Thông tin tồn kho cần được cập nhật và kiểm tra trước khi xác nhận khả năng đáp ứng đơn hàng.
- Cần xác định rõ vai trò chịu trách nhiệm cập nhật thông tin tồn kho.

**Liên quan:** P-01, BR-02, FR-03.

### SR-02 – Chuẩn hóa thông tin giao hàng

- Hệ thống cần hỗ trợ lưu trữ thông tin người nhận, số điện thoại và địa chỉ giao hàng.
- Cần xác định các trường thông tin bắt buộc.
- Hệ thống cần hỗ trợ kiểm tra tính đầy đủ của thông tin trước khi chuyển sang bước tiếp theo.
- Trường hợp thông tin chưa đầy đủ, cần ghi nhận nội dung cần bổ sung.

**Liên quan:** P-02, BR-04, FR-05, FR-06.

### SR-03 – Theo dõi thời hạn thanh toán

- Hệ thống cần ghi nhận thời điểm bắt đầu tính thời hạn xác nhận thanh toán.
- Hệ thống cần hỗ trợ theo dõi thời hạn 2 ngày theo quy trình.
- Cần có cơ chế nhận diện đơn hàng chưa nhận được xác nhận thanh toán khi hết thời hạn.
- Phương án xử lý đơn hàng quá hạn cần được xác nhận với Stakeholder.

**Liên quan:** P-03, BR-07, FR-08.

### SR-04 – Kiểm soát giao hàng thất bại

- Hệ thống cần hỗ trợ ghi nhận trạng thái giao hàng thất bại.
- Cần theo dõi số lần giao hàng lại của đơn hàng.
- Cần xác định giới hạn số lần giao lại theo chính sách được phê duyệt.
- Khi đạt giới hạn, hệ thống cần hỗ trợ chuyển đơn hàng sang trạng thái chờ xử lý tiếp theo.

**Liên quan:** P-04, BR-09, FR-09, FR-10.

### SR-05 – Chuẩn hóa xử lý khiếu nại

- Hệ thống cần hỗ trợ ghi nhận loại khiếu nại: thiếu hàng, hàng hóa hư hỏng hoặc giao sai hàng.
- Hệ thống cần hỗ trợ lưu trữ hình ảnh và bằng chứng liên quan.
- Cần xây dựng tiêu chí xác định tính hợp lệ của khiếu nại.
- Kết quả kiểm tra và phương án xử lý cần được ghi nhận để theo dõi.

**Liên quan:** P-05, BR-10, FR-11, FR-12.

## 3. Ma trận truy vết yêu cầu giải pháp

| Solution Requirement | Problem | Business Rule | Functional Requirement | Use Case |
|---|---|---|---|---|
| SR-01 | P-01 | BR-02 | FR-03 | UC-03 |
| SR-02 | P-02 | BR-04 | FR-05, FR-06 | UC-05 |
| SR-03 | P-03 | BR-07 | FR-08 | UC-08 |
| SR-04 | P-04 | BR-09 | FR-09, FR-10 | UC-11, UC-12 |
| SR-05 | P-05 | BR-10 | FR-11, FR-12 | UC-13, UC-14, UC-15, UC-16, UC-17, UC-18 |

### Ghi chú về phạm vi truy vết

- Các SR trên tập trung vào 5 vấn đề P-01 đến P-05 đã xác định trong Phase 2.
- FR-01, FR-02, FR-04, FR-07, FR-13, FR-14, FR-15 và FR-16 vẫn thuộc phạm vi yêu cầu nghiệp vụ của dự án, nhưng không phải tất cả đều cần một SR riêng trong nhóm cải tiến này.
- Việc một FR chưa xuất hiện trong ma trận SR không có nghĩa là yêu cầu đó bị loại bỏ.
- Các liên kết hiện tại là kết quả phân tích sơ bộ, cần được xác nhận khi có ý kiến Stakeholder.
## 4. Các nội dung chưa được xác định

| ID | Nội dung | Trạng thái |
|---|---|---|
| OQ-SR-01 | Trách nhiệm cập nhật tồn kho thuộc bộ phận nào? | Chờ xác nhận |
| OQ-SR-02 | Những trường thông tin giao hàng nào là bắt buộc? | Chờ xác nhận |
| OQ-SR-03 | Đơn hàng được xử lý thế nào khi quá hạn thanh toán? | Chờ xác nhận |
| OQ-SR-04 | Số lần giao hàng lại tối đa là bao nhiêu? | Chờ xác nhận |
| OQ-SR-05 | Tiêu chí và bằng chứng nào được dùng để đánh giá khiếu nại? | Chờ xác nhận |

## 5. Kết luận

Năm Solution Requirements được xây dựng nhằm giải quyết năm nhóm vấn đề đã xác định trong quy trình AS-IS.

Các yêu cầu cần tiếp tục được xác minh về tính khả thi, trách nhiệm thực hiện và phạm vi chức năng trước khi chuyển sang thiết kế chi tiết.

**Trạng thái:** Proposed Solution Requirements – Yêu cầu giải pháp đề xuất.
