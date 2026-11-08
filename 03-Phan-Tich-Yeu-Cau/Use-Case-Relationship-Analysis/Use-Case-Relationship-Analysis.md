# Phân tích mối quan hệ giữa các Use Case

## 1. Mục tiêu

Tài liệu phân tích mối quan hệ giữa 18 Use Case trong quy trình xử lý đơn hàng bán lẻ nhằm:

- Xác định sự phụ thuộc giữa các chức năng.
- Phát hiện các Use Case có nội dung trùng lặp hoặc chồng chéo.
- Xác định các quan hệ phù hợp như `include` và `extend`.
- Liên kết các Use Case với Functional Requirements.
- Làm cơ sở hoàn thiện Use Case Diagram và đặc tả yêu cầu.

## 2. Phân nhóm Use Case

| Nhóm nghiệp vụ | Mã Use Case | Tên Use Case |
|---|---|---|
| Quản lý đơn hàng | UC-01 | Tiếp nhận đơn hàng |
| Quản lý đơn hàng | UC-02 | Kiểm tra thông tin đơn hàng |
| Quản lý đơn hàng | UC-03 | Kiểm tra tình trạng hàng hóa |
| Quản lý đơn hàng | UC-04 | Xử lý trường hợp hết hàng |
| Quản lý đơn hàng | UC-05 | Cập nhật thông tin giao hàng |
| Quản lý đơn hàng | UC-06 | Xác nhận phương thức giao hàng |
| Quản lý đơn hàng | UC-07 | Lập hóa đơn |
| Thanh toán và giao hàng | UC-08 | Ghi nhận xác nhận thanh toán |
| Thanh toán và giao hàng | UC-09 | Kiểm tra và đóng gói hàng hóa |
| Thanh toán và giao hàng | UC-10 | Bàn giao hàng cho đơn vị vận chuyển |
| Thanh toán và giao hàng | UC-11 | Cập nhật trạng thái giao hàng |
| Thanh toán và giao hàng | UC-12 | Xử lý giao hàng thất bại |
| Quản lý khiếu nại | UC-13 | Gửi khiếu nại |
| Quản lý khiếu nại | UC-14 | Tiếp nhận khiếu nại |
| Quản lý khiếu nại | UC-15 | Kiểm tra tính hợp lệ của khiếu nại |
| Quản lý khiếu nại | UC-16 | Xử lý hàng hóa bị lỗi |
| Quản lý khiếu nại | UC-17 | Chuẩn bị và gửi hàng thay thế |
| Quản lý khiếu nại | UC-18 | Cập nhật kết quả xử lý khiếu nại |

## 3. Phân tích các mối quan hệ

### 3.1. Nhóm quản lý đơn hàng

| Use Case nguồn | Use Case liên quan | Mối quan hệ nghiệp vụ | Giải thích |
|---|---|---|---|
| UC-01 | UC-02 | Luồng tiếp nối | Sau khi tiếp nhận đơn hàng, thông tin được kiểm tra. |
| UC-02 | UC-03 | Luồng tiếp nối | Sau khi kiểm tra thông tin đơn hàng, tiến hành kiểm tra tình trạng hàng hóa. |
| UC-03 | UC-04 | Luồng điều kiện | UC-04 được thực hiện khi phát hiện hàng hóa không đủ số lượng. |
| UC-04 | UC-03 | Luồng lặp | Nếu khách hàng chọn sản phẩm thay thế, cần kiểm tra lại tình trạng hàng hóa. |
| UC-03 | UC-05 | Luồng tiếp nối có điều kiện | Khi hàng hóa đáp ứng yêu cầu, tiếp tục thu thập thông tin giao hàng. |
| UC-05 | UC-06 | Luồng tiếp nối | Sau khi thông tin giao hàng được kiểm tra, tiếp tục xác nhận phương thức giao hàng. |
| UC-06 | UC-07 | Luồng tiếp nối | Sau khi xác nhận phương thức giao hàng, tiến hành lập hóa đơn. |
| UC-07 | UC-08 | Luồng tiếp nối | Sau khi hoàn thiện hóa đơn, tiếp nhận xác nhận thanh toán. |

### 3.2. Nhóm thanh toán và giao hàng

| Use Case nguồn | Use Case liên quan | Mối quan hệ nghiệp vụ | Giải thích |
|---|---|---|---|
| UC-08 | UC-09 | Luồng tiếp nối | Sau khi ghi nhận xác nhận thanh toán, đơn hàng được chuyển sang khâu chuẩn bị hàng hóa. |
| UC-09 | UC-10 | Luồng tiếp nối | Hàng hóa được kiểm tra và đóng gói trước khi bàn giao. |
| UC-10 | UC-11 | Luồng tiếp nối | Sau khi đơn vị vận chuyển tiếp nhận hàng, quá trình giao hàng và cập nhật trạng thái được thực hiện. |
| UC-11 | UC-12 | Luồng điều kiện | UC-12 được thực hiện khi kết quả giao hàng thất bại. |
| UC-12 | UC-09 | Luồng lặp có điều kiện | Nếu cần giao lại, đơn hàng quay về khâu chuẩn bị hàng hóa. |

### 3.3. Nhóm quản lý khiếu nại

| Use Case nguồn | Use Case liên quan | Mối quan hệ nghiệp vụ | Giải thích |
|---|---|---|---|
| UC-13 | UC-14 | Luồng tiếp nối | Sau khi khách hàng gửi khiếu nại, bộ phận chăm sóc khách hàng tiếp nhận. |
| UC-14 | UC-15 | Luồng tiếp nối | Khiếu nại được tiếp nhận trước khi kiểm tra tính hợp lệ. |
| UC-15 | UC-16 | Luồng điều kiện | Khiếu nại hợp lệ và cần xử lý hàng hóa, tiến hành UC-16. |
| UC-16 | UC-17 | Luồng tiếp nối có điều kiện | Sau khi xử lý hàng hóa, chuẩn bị hàng thay thế nếu phương án giải quyết yêu cầu. |
| UC-17 | UC-18 | Luồng tiếp nối | Sau khi hàng thay thế được gửi đi, cập nhật kết quả xử lý khiếu nại. |
| UC-15 | UC-18 | Luồng điều kiện | Nếu khiếu nại không hợp lệ, ghi nhận và thông báo kết quả cho khách hàng. |

## 4. Đề xuất sử dụng quan hệ Include và Extend

Không phải mọi mối liên hệ giữa các Use Case đều cần thể hiện bằng `include` hoặc `extend`. Các quan hệ này chỉ nên sử dụng khi phù hợp với mục tiêu và hành vi của từng Use Case.

| Use Case mở rộng | Use Case cơ sở | Loại quan hệ | Điều kiện |
|---|---|---|---|
| UC-04 | UC-03 | `extend` | Hàng hóa không đủ số lượng |
| UC-12 | UC-11 | `extend` | Kết quả giao hàng thất bại |
| UC-16 | UC-15 | `extend` | Khiếu nại hợp lệ và cần xử lý hàng hóa |

Các quan hệ trên là đề xuất dựa trên luồng nghiệp vụ BPMN. Không sử dụng `include` chỉ vì một Use Case xảy ra sau một Use Case khác.

## 5. Liên kết Use Case với Functional Requirements

| Requirement ID | Nội dung yêu cầu | Use Case liên quan |
|---|---|---|
| FR-01 | Tiếp nhận đơn hàng | UC-01 |
| FR-02 | Kiểm tra thông tin đơn hàng | UC-02 |
| FR-03 | Kiểm tra tồn kho | UC-03 |
| FR-04 | Xử lý hàng hóa không có sẵn | UC-04 |
| FR-05 | Kiểm tra thông tin giao hàng | UC-05 |
| FR-06 | Cập nhật thông tin giao hàng | UC-05 |
| FR-07 | Quản lý hóa đơn | UC-07 |
| FR-08 | Ghi nhận thanh toán | UC-08 |
| FR-09 | Theo dõi trạng thái giao hàng | UC-11 |
| FR-10 | Xử lý giao hàng thất bại | UC-12 |
| FR-11 | Tiếp nhận khiếu nại | UC-13, UC-14, UC-15 |
| FR-12 | Theo dõi kết quả xử lý khiếu nại | UC-16, UC-17, UC-18 |
| FR-13 | Xác nhận phương thức giao hàng | UC-06 |
| FR-14 | Quản lý thông tin bảo hiểm hàng hóa | UC-07, UC-09 |
| FR-15 | Kiểm tra và đóng gói hàng hóa | UC-09 |
| FR-16 | Bàn giao hàng cho đơn vị vận chuyển | UC-10 |

## 6. Các điểm cần rà soát

### 6.1. UC-03 và UC-04 có khả năng chồng chéo

UC-03 tập trung vào việc kiểm tra tình trạng hàng hóa và xác định kết quả tồn kho.

UC-04 mô tả việc xử lý khi hàng hóa không đủ số lượng, bao gồm lựa chọn hủy đơn hoặc chọn sản phẩm thay thế.

**Đề xuất:** Giữ hai Use Case riêng biệt. UC-04 là hành vi mở rộng của UC-03 khi phát hiện hàng hóa không đủ số lượng.

### 6.2. UC-13 và UC-14 có khả năng chồng chéo

UC-13 mô tả khách hàng gửi khiếu nại, UC-14 mô tả nhân viên tiếp nhận khiếu nại.

**Đề xuất:** Giữ hai Use Case trong mô hình nghiệp vụ. Tuy nhiên, nếu sơ đồ mô tả một hệ thống nội bộ và khách hàng không trực tiếp tương tác với hệ thống, UC-13 cần được xem xét là hoạt động bên ngoài phạm vi hệ thống.

### 6.3. UC-16 và UC-17 cần phân biệt rõ

UC-16 tập trung vào việc xử lý hàng hóa liên quan đến khiếu nại.

UC-17 tập trung vào việc chuẩn bị và gửi hàng thay thế.

**Đề xuất:** Giữ hai Use Case riêng biệt vì có mục tiêu nghiệp vụ khác nhau. Cần xác minh liệu mọi khiếu nại hợp lệ có yêu cầu trả hàng cũ và gửi hàng thay thế hay không.

### 6.4. UC-10 và UC-11 cần xác định ranh giới

UC-10 mô tả việc bàn giao hàng hóa cho đơn vị vận chuyển.

UC-11 mô tả việc cập nhật trạng thái trong quá trình vận chuyển.

**Đề xuất:** Giữ riêng hai Use Case vì bàn giao và theo dõi trạng thái là hai hoạt động khác nhau. Cần xác minh cách đơn vị vận chuyển trao đổi dữ liệu với hệ thống doanh nghiệp.

### 6.5. FR-12 đang bao gồm nhiều hoạt động

FR-12 hiện liên kết với UC-16, UC-17 và UC-18.

**Đề xuất:** Giữ FR-12 ở mức yêu cầu tổng quát trong giai đoạn hiện tại. Các hoạt động chi tiết được thể hiện trong từng Use Case Specification. Chỉ tách thành các FR riêng nếu phạm vi yêu cầu cần quản lý hoặc kiểm thử độc lập.

## 7. Kết luận

18 Use Case đã được phân nhóm thành ba mảng nghiệp vụ chính:

1. Quản lý đơn hàng.
2. Thanh toán và giao hàng.
3. Quản lý khiếu nại.

Bộ Use Case hiện tại đã được liên kết với 16 Functional Requirements. Các quan hệ `extend` được đề xuất dựa trên các nhánh điều kiện trong BPMN.

Một số nội dung vẫn cần được xác minh, đặc biệt là ranh giới hệ thống, cách tương tác của khách hàng và đơn vị vận chuyển, cũng như các điều kiện xử lý khiếu nại.

**Trạng thái:** Preliminary Analysis – Phân tích sơ bộ, chưa được Stakeholder xác nhận.
