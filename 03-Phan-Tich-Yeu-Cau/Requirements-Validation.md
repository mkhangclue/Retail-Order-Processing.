# Requirements Validation

## 1. Mục đích

Tài liệu ghi nhận kết quả rà soát và kiểm định sơ bộ bộ yêu cầu của dự án phân tích và cải tiến quy trình xử lý đơn hàng bán lẻ.

Mục tiêu:
- Kiểm tra tính nhất quán giữa Business Requirements, Business Rules và Use Case.
- Đối chiếu yêu cầu với quy trình BPMN gốc.
- Phân biệt nội dung có căn cứ và nội dung cần xác minh.
- Chuẩn bị cơ sở cho giai đoạn thiết kế giải pháp.

## 2. Phạm vi kiểm định

| Thành phần | Số lượng | Trạng thái |
|---|---:|---|
| Functional Requirements | 16 | Đã xây dựng bản nháp |
| Non-functional Requirements | 5 | Đã xây dựng bản nháp |
| Business Rules | 10 | Đã xây dựng bản nháp |
| Use Cases | 18 | Đã xây dựng đặc tả |
| Use Case Diagram | 1 | Đã xây dựng |
| Requirements Traceability Matrix | 1 | Đã xây dựng bản nháp |

## 3. Kết quả kiểm định sơ bộ

| Tiêu chí | Kết quả | Ghi chú |
|---|---|---|
| Traceability | Đạt sơ bộ | Các yêu cầu đã được liên kết với Use Case và Business Rules |
| Completeness | Cần làm rõ | Một số hoạt động cần thêm thông tin chi tiết |
| Consistency | Cần rà soát | Cần bảo đảm mã FR, BR và UC nhất quán giữa các tài liệu |
| Clarity | Đạt sơ bộ | Một số yêu cầu vẫn đang ở mức tổng quát |
| Testability | Cần làm rõ | Chưa có tiêu chí nghiệm thu cụ thể |

## 4. Các nội dung cần xác minh với Stakeholder

| ID | Nội dung cần xác minh | Mức độ ưu tiên |
|---|---|---|
| OQ-01 | Cơ chế kiểm tra và cập nhật tồn kho | High |
| OQ-02 | Cách xử lý khi khách hàng không xác nhận thanh toán trong 2 ngày | High |
| OQ-03 | Số lần giao hàng lại tối đa | Medium |
| OQ-04 | Tiêu chí xác định khiếu nại hợp lệ | High |
| OQ-05 | Kênh tiếp nhận khiếu nại của khách hàng | Medium |
| OQ-06 | Cách thức xác nhận bàn giao hàng cho đơn vị vận chuyển | Medium |
| OQ-07 | Ranh giới giữa lập hóa đơn và hoàn thiện hóa đơn | Medium |
| OQ-08 | Quy tắc áp dụng bảo hiểm và tính phí bảo hiểm | Medium |

## 5. Giới hạn kiểm định

- Các yêu cầu được xây dựng dựa trên BPMN gốc và tài liệu phân tích hiện có.
- Nội dung phỏng vấn giả lập không được xem là xác nhận chính thức từ doanh nghiệp.
- Chưa có xác nhận trực tiếp từ Stakeholder về tính chính xác và mức độ ưu tiên của yêu cầu.
- Chưa có hệ thống thực tế để kiểm tra khả năng đáp ứng các yêu cầu phi chức năng.
- Các yêu cầu hiện tại là cơ sở phân tích, chưa phải đặc tả đã được phê duyệt.

## 6. Kết luận

Bộ tài liệu yêu cầu đã hình thành được cấu trúc ban đầu, bao gồm Business Rules, Business Requirements, Use Case Specifications và Requirements Traceability.

Các nội dung còn thiếu hoặc chưa rõ đã được ghi nhận để tiếp tục xác minh.

**Trạng thái:** Preliminary Validation – Kiểm định sơ bộ, chưa được Stakeholder phê duyệt.
