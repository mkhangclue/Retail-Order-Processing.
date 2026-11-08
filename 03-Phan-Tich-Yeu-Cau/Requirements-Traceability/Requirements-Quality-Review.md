# Requirements Quality Review

## 1. Mục đích

Đánh giá chất lượng của các yêu cầu chức năng (Functional Requirements) dựa trên những tiêu chí:

- **Clarity:** Yêu cầu rõ ràng, dễ hiểu.
- **Completeness:** Yêu cầu có đủ thông tin cần thiết.
- **Consistency:** Không mâu thuẫn với các yêu cầu khác.
- **Testability:** Có thể kiểm tra hoặc xác minh.
- **Traceability:** Có thể truy xuất về nguồn nghiệp vụ.

## 2. Bảng đánh giá chất lượng yêu cầu

| Requirement ID | Nội dung | Đánh giá | Vấn đề cần lưu ý |
|---|---|---|---|
| FR-01 | Tiếp nhận đơn hàng | Đạt sơ bộ | Chưa xác định đầy đủ thông tin đầu vào |
| FR-02 | Kiểm tra thông tin đơn hàng | Cần làm rõ | Chưa xác định tiêu chí thông tin hợp lệ |
| FR-03 | Kiểm tra tồn kho | Đạt sơ bộ | Chưa rõ cơ chế cập nhật tồn kho |
| FR-04 | Xử lý hàng hóa không có sẵn | Đạt sơ bộ | Đã thể hiện hai lựa chọn hủy đơn hoặc chọn sản phẩm thay thế |
| FR-05 | Kiểm tra thông tin giao hàng | Đạt sơ bộ | Cần xác định các trường thông tin bắt buộc |
| FR-06 | Cập nhật thông tin giao hàng | Đạt sơ bộ | Chưa xác định quyền cập nhật và cách xác nhận thông tin |
| FR-07 | Quản lý hóa đơn | Cần làm rõ | Ranh giới giữa lập hóa đơn trong Subprocess và hoàn thiện hóa đơn trong quy trình chính chưa rõ |
| FR-08 | Ghi nhận thanh toán | Cần làm rõ | Chưa mô tả cách xử lý khi quá hạn 2 ngày |
| FR-09 | Theo dõi trạng thái giao hàng | Cần làm rõ | Chưa xác định rõ đơn vị trực tiếp cập nhật trạng thái trên hệ thống |
| FR-10 | Xử lý giao hàng thất bại | Đạt sơ bộ | Chưa có quy định về số lần giao lại và điều kiện dừng |
| FR-11 | Tiếp nhận khiếu nại | Đạt sơ bộ | Chưa xác định kênh tiếp nhận và thông tin bắt buộc |
| FR-12 | Theo dõi kết quả xử lý khiếu nại | Cần làm rõ | Đang bao gồm nhiều hoạt động: xác minh, xử lý hàng lỗi, gửi hàng thay thế và cập nhật kết quả |
| FR-13 | Xác nhận phương thức giao hàng | Đạt sơ bộ | Chưa xác định cách thức xác nhận |
| FR-14 | Quản lý thông tin bảo hiểm hàng hóa | Cần làm rõ | Chưa xác định đầy đủ thông tin bảo hiểm và cách tính phí |
| FR-15 | Kiểm tra và đóng gói hàng hóa | Đạt sơ bộ | Cần làm rõ tiêu chuẩn đóng gói và cách kiểm tra trước bàn giao |

## 3. Các vấn đề ưu tiên làm rõ

| Priority | Nội dung |
|---|---|
| High | Làm rõ FR-12 vì đang bao gồm nhiều hoạt động xử lý khiếu nại |
| High | Xác định tiêu chí kiểm tra thông tin đơn hàng và thông tin giao hàng |
| High | Làm rõ ranh giới giữa lập và hoàn thiện hóa đơn |
| Medium | Xác định cách ghi nhận và xử lý xác nhận thanh toán quá hạn |
| Medium | Làm rõ trách nhiệm cập nhật trạng thái giao hàng |
| Medium | Xác định thông tin và quy tắc áp dụng bảo hiểm |
| Medium | Làm rõ hoạt động bàn giao hàng cho đơn vị vận chuyển |

## 4. Kết luận

Bộ yêu cầu chức năng đã có cấu trúc tương đối đầy đủ và có thể truy xuất về các hoạt động chính trong BPMN.

Tuy nhiên, một số yêu cầu vẫn đang ở mức mô tả tổng quát, chưa đủ điều kiện để chuyển trực tiếp thành đặc tả chức năng chi tiết hoặc tiêu chí kiểm thử.

Các nội dung chưa rõ sẽ được ghi nhận trong Open Questions để tiếp tục xác minh với Stakeholder, thay vì tự đưa ra quy tắc nghiệp vụ.

**Trạng thái:** Preliminary Review – Đánh giá sơ bộ.
