# Gap Analysis – Phân tích khoảng cách

## 1. Mục đích

Tài liệu phân tích khoảng cách giữa quy trình xử lý đơn hàng bán lẻ hiện tại (AS-IS) và trạng thái mong muốn sau cải tiến (TO-BE).

Mục tiêu:
- Xác định những điểm còn thiếu hoặc chưa rõ trong quy trình hiện tại.
- Đối chiếu vấn đề nghiệp vụ với giải pháp đề xuất.
- Xác định yêu cầu cần bổ sung để thu hẹp khoảng cách.
- Làm cơ sở xây dựng Solution Requirements.

## 2. Phạm vi phân tích

Phân tích tập trung vào 5 vấn đề đã xác định trong Phase 2:

- P-01: Kiểm soát tình trạng tồn kho.
- P-02: Cập nhật thông tin giao hàng nhiều lần.
- P-03: Chưa có quy trình xử lý thanh toán quá hạn.
- P-04: Chưa xác định giới hạn số lần giao hàng lại.
- P-05: Chưa có tiêu chí cụ thể để xác định khiếu nại hợp lệ.

Nguồn phân tích:
- BPMN AS-IS – Quy trình xử lý đơn hàng bán lẻ.
- Business Findings.
- Open Questions.
- Phân tích vấn đề và nguyên nhân.
- Đề xuất cải tiến quy trình.

## 3. Bảng phân tích GAP

| Problem ID | Hiện trạng (AS-IS) | Khoảng cách (GAP) | Trạng thái mong muốn | Giải pháp đề xuất |
|---|---|---|---|---|
| P-01 | Có bước kiểm tra tình trạng hàng hóa nhưng cơ chế cập nhật và xác nhận tồn kho chưa rõ. | Chưa xác định rõ trách nhiệm cập nhật và cách bảo đảm số lượng tồn kho chính xác. | Có thông tin tồn kho được kiểm tra và ghi nhận rõ ràng trước khi tiếp tục xử lý đơn. | Quy định trách nhiệm cập nhật tồn kho và ghi nhận kết quả kiểm tra. |
| P-02 | Khi thông tin giao hàng chưa đầy đủ, quy trình yêu cầu khách hàng cập nhật và kiểm tra lại. | Chưa có danh sách thông tin bắt buộc và tiêu chí kiểm tra thống nhất. | Thông tin giao hàng được kiểm tra theo bộ tiêu chí thống nhất. | Chuẩn hóa các trường thông tin bắt buộc và kiểm tra tính đầy đủ trước khi chuyển bước. |
| P-03 | Khách hàng được yêu cầu gửi xác nhận thanh toán trong vòng 2 ngày. | Chưa có nhánh xử lý khi hết thời hạn nhưng chưa nhận được xác nhận thanh toán. | Có cơ chế theo dõi thời hạn và xử lý trường hợp quá
