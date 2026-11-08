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
| P-03 | Khách hàng được yêu cầu gửi xác nhận thanh toán trong vòng 2 ngày. | Chưa có nhánh xử lý khi hết thời hạn nhưng chưa nhận được xác nhận thanh toán. | Có cơ chế theo dõi thời hạn và xử lý trường hợp quá hạn. | Bổ sung theo dõi thời hạn thanh toán và quy tắc xử lý quá hạn sau khi được Stakeholder xác nhận. |
| P-04 | Khi giao hàng thất bại, bộ phận CS liên hệ khách hàng và phối hợp xử lý giao lại. | Chưa xác định số lần giao lại tối đa và điều kiện dừng. | Có quy tắc kiểm soát số lần giao lại và phương án xử lý tiếp theo. | Xây dựng giới hạn số lần giao lại và điều kiện chuyển sang phương án khác. |
| P-05 | Khiếu nại cần có hình ảnh để kiểm tra và đánh giá tính hợp lệ. | Chưa có tiêu chí đánh giá và danh sách bằng chứng cụ thể. | Khiếu nại được đánh giá theo tiêu chí thống nhất. | Xây dựng bộ tiêu chí xác minh và danh sách bằng chứng cần thiết. |

## 4. Phân loại giải pháp

| Nhóm giải pháp | Nội dung | Loại giải pháp |
|---|---|---|
| Kiểm soát tồn kho | Làm rõ trách nhiệm cập nhật và ghi nhận kết quả kiểm tra tồn kho. | Quy trình / Hệ thống |
| Chuẩn hóa thông tin giao hàng | Xây dựng danh sách trường thông tin bắt buộc và tiêu chí kiểm tra. | Quy trình / Hệ thống |
| Theo dõi thanh toán | Theo dõi thời hạn xác nhận thanh toán và xử lý quá hạn. | Quy trình / Hệ thống |
| Kiểm soát giao hàng thất bại | Quản lý số lần giao lại và điều kiện dừng. | Quy trình / Hệ thống |
| Chuẩn hóa khiếu nại | Xác định tiêu chí đánh giá và bằng chứng cần thiết. | Quy trình / Hệ thống |

## 5. Các nội dung cần xác nhận

| ID | Nội dung | Lý do cần xác nhận |
|---|---|---|
| GAP-01 | Bộ phận chịu trách nhiệm cập nhật tồn kho. | BPMN chưa thể hiện rõ trách nhiệm cập nhật. |
| GAP-02 | Danh sách thông tin giao hàng bắt buộc. | Chưa có danh sách trường dữ liệu cụ thể. |
| GAP-03 | Phương án xử lý khi thanh toán quá hạn. | Chưa có quy định trong quy trình hiện tại. |
| GAP-04 | Số lần giao hàng lại tối đa. | Chưa có giới hạn được xác định. |
| GAP-05 | Tiêu chí xác định khiếu nại hợp lệ. | Chưa có quy tắc đánh giá cụ thể. |

## 6. Kết luận

Qua phân tích, 5 vấn đề P-01 đến P-05 đều có khoảng cách giữa quy trình hiện tại và trạng thái mong muốn.

Các giải pháp được đề xuất nhằm bổ sung quy tắc nghiệp vụ, chuẩn hóa thông tin và tăng khả năng kiểm soát quy trình.

Các nội dung trong tài liệu là đề xuất sơ bộ, chưa được Stakeholder xác nhận và chưa được xem là yêu cầu triển khai chính thức.

**Trạng thái:** Preliminary Gap Analysis – Phân tích GAP sơ bộ.
