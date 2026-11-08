# Solution Design Summary

## 1. Tổng quan

Phase 4 tập trung xây dựng các đề xuất cải tiến cho quy trình xử lý đơn hàng bán lẻ dựa trên kết quả phân tích AS-IS và các vấn đề được xác định trong Phase 2.

Mục tiêu là chuyển những vấn đề nghiệp vụ thành các giải pháp và yêu cầu cụ thể, làm cơ sở cho việc đánh giá và kiểm thử ở giai đoạn tiếp theo.

## 2. Đầu vào thiết kế

| Tài liệu | Vai trò |
|---|---|
| BPMN AS-IS | Mô tả quy trình hiện tại |
| Business Findings | Tổng hợp các phát hiện nghiệp vụ |
| Open Questions | Ghi nhận những nội dung chưa rõ |
| Business Requirements | Xác định yêu cầu nghiệp vụ |
| Business Rules | Xác định các quy tắc nghiệp vụ |
| Use Case Specifications | Mô tả các hoạt động nghiệp vụ |

## 3. Kết quả thiết kế

| Thành phần | Kết quả |
|---|---|
| Improvement Proposal | Đề xuất cải tiến 5 vấn đề |
| Gap Analysis | Phân tích khoảng cách giữa hiện trạng và trạng thái mong muốn |
| Solution Requirements | Xây dựng 5 nhóm yêu cầu giải pháp |
| Requirements Traceability | Liên kết Problem, BR, FR, UC và SR |

## 4. Tổng hợp giải pháp

| Problem | Giải pháp đề xuất | Solution Requirement |
|---|---|---|
| P-01 – Kiểm soát tồn kho | Ghi nhận kết quả kiểm tra và làm rõ trách nhiệm cập nhật tồn kho | SR-01 |
| P-02 – Thông tin giao hàng | Chuẩn hóa trường thông tin và kiểm tra tính đầy đủ | SR-02 |
| P-03 – Thanh toán quá hạn | Theo dõi thời hạn xác nhận thanh toán và bổ sung phương án xử lý | SR-03 |
| P-04 – Giao hàng thất bại | Theo dõi số lần giao lại và xác định điều kiện dừng | SR-04 |
| P-05 – Xử lý khiếu nại | Chuẩn hóa tiêu chí đánh giá và bằng chứng | SR-05 |

## 5. Giới hạn thiết kế

- Giải pháp được xây dựng dựa trên BPMN AS-IS và kết quả phân tích nghiệp vụ hiện có.
- Chưa có xác nhận chính thức từ Stakeholder.
- Chưa xác định công nghệ, kiến trúc triển khai hoặc nền tảng hệ thống cụ thể.
- Chưa có số liệu thực tế để định lượng hiệu quả cải tiến.
- Chưa xây dựng BPMN TO-BE trong phạm vi hiện tại.

## 6. Kết luận

Phase 4 đã hình thành các đề xuất cải tiến và yêu cầu giải pháp tương ứng với năm vấn đề nghiệp vụ.

Các kết quả này sẽ được sử dụng làm đầu vào cho Phase 5 – Solution Validation & Testing.

**Trạng thái:** Preliminary Solution Design – Thiết kế giải pháp sơ bộ.
