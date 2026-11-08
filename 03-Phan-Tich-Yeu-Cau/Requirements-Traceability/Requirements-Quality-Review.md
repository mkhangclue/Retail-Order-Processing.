# Requirements Quality Review

## 1. Mục đích

Đánh giá chất lượng của các yêu cầu chức năng (Functional Requirements) dựa trên các tiêu chí:

- Clarity: Yêu cầu rõ ràng, dễ hiểu.
- Completeness: Yêu cầu có đủ thông tin cần thiết.
- Consistency: Không mâu thuẫn với các yêu cầu khác.
- Testability: Có thể kiểm tra hoặc xác minh.
- Traceability: Có thể truy xuất về nguồn nghiệp vụ.

## 2. Bảng đánh giá

| Requirement ID | Nội dung | Đánh giá | Vấn đề cần lưu ý |
|---|---|---|---|
| FR-01 | Tiếp nhận đơn hàng | Cần làm rõ | Chưa xác định đầy đủ thông tin đầu vào |
| FR-02 | Kiểm tra thông tin đơn hàng | Đạt sơ bộ | Cần xác định tiêu chí thông tin hợp lệ |
| FR-03 | Kiểm tra tình trạng hàng hóa | Đạt sơ bộ | Chưa rõ cơ chế cập nhật tồn kho |
| FR-04 | Xử lý trường hợp hết hàng | Đạt sơ bộ | Đã có hai lựa chọn hủy hoặc chọn sản phẩm thay thế |
| FR-05 | Cập nhật thông tin giao hàng | Cần làm rõ | Chưa xác định các trường thông tin bắt buộc |
| FR-06 | Xác nhận phương thức giao hàng | Đạt sơ bộ | Cần làm rõ cách xác nhận |
| FR-07 | Lập hóa đơn | Cần làm rõ | Ranh giới giữa lập hóa đơn trong Subprocess và hoàn thiện hóa đơn trong quy trình chính chưa rõ |
| FR-08 | Ghi nhận xác nhận thanh toán | Cần làm rõ | Chưa mô tả cách xử lý khi quá hạn 2 ngày |
| FR-09 | Kiểm tra và đóng gói hàng hóa | Đạt sơ bộ | Cần xác định chi tiết tiêu chuẩn đóng gói |
| FR-10 | Bàn giao hàng cho đơn vị vận chuyển | Đạt sơ bộ | Chưa mô tả chi tiết cách xác nhận bàn giao |
| FR-11 | Cập nhật trạng thái giao hàng | Cần làm rõ | Chưa xác định đơn vị trực tiếp cập nhật trên hệ thống |
| FR-12 | Xử lý giao hàng thất bại và khiếu nại | Cần tách nhỏ | Đang gộp nhiều hoạt động nghiệp vụ khác nhau |

## 3. Các vấn đề ưu tiên làm rõ

| Priority | Nội dung |
|---|---|
| High | Làm rõ FR-12 vì đang gộp nhiều chức năng |
| High | Làm rõ tiêu chí kiểm tra thông tin đơn hàng và giao hàng |
| Medium | Làm rõ cơ chế xác nhận thanh toán |
| Medium | Làm rõ trách nhiệm cập nhật trạng thái giao hàng |
| Medium | Làm rõ ranh giới lập và hoàn thiện hóa đơn |

## 4. Kết luận

Bộ yêu cầu hiện tại đã hình thành được cấu trúc ban đầu nhưng vẫn còn một số yêu cầu chưa đủ chi tiết để chuyển trực tiếp thành đặc tả chức năng hoàn chỉnh.

Các nội dung chưa rõ sẽ được ghi nhận để tiếp tục phân tích.

**Trạng thái:** Preliminary Review – Đánh giá sơ bộ.
