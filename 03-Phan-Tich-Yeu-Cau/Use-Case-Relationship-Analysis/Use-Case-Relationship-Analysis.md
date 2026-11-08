# Phân tích mối quan hệ giữa các Use Case

## 1. Mục tiêu

Tài liệu phân tích mối quan hệ giữa 18 Use Case trong quy trình xử lý đơn hàng bán lẻ nhằm:

- Xác định sự phụ thuộc giữa các chức năng.
- Phát hiện các Use Case có nội dung trùng lặp hoặc chồng chéo.
- Xác định các quan hệ phù hợp như `include` và `extend`.
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

| Use Case nguồn | Use Case liên quan | Mối quan hệ | Giải thích |
|---|---|---|---|
| UC-01 | UC-02 | Luồng tiếp nối | Sau khi tiếp nhận đơn hàng, thông tin được kiểm tra. |
| UC-02 | UC-03 | Luồng tiếp nối | Chỉ kiểm tra hàng hóa sau khi thông tin đơn hàng đã được kiểm tra. |
| UC-03 | UC-04 | Luồng điều kiện | UC-04 được thực hiện khi phát hiện hàng hóa không đủ số lượng. |
| UC-04 | UC-03 | Luồng lặp | Nếu khách hàng chọn sản phẩm thay thế, cần kiểm tra lại tình trạng hàng hóa. |
| UC-03 | UC-05 | Luồng tiếp nối | Khi hàng hóa đáp ứng yêu cầu, tiếp tục thu thập thông tin giao hàng. |
| UC-05 | UC-06 | Luồng tiếp nối | Sau khi thông tin giao hàng được xác nhận, tiếp tục xác nhận phương thức giao hàng. |
| UC-06 | UC-07 | Luồng tiếp nối | Sau khi xác nhận phương thức giao hàng, tiến hành lập hóa đơn. |
| UC-07 | UC-08 | Luồng tiếp nối | Sau khi hoàn thiện hóa đơn, tiếp nhận xác nhận thanh toán. |

### 3.2. Nhóm thanh toán và giao hàng

| Use Case nguồn | Use Case liên quan | Mối quan hệ | Giải thích |
|---|---|---|---|
| UC-08 | UC-09 | Luồng tiếp nối | Sau khi xác nhận thanh toán, đơn hàng được chuyển sang khâu chuẩn bị hàng hóa. |
| UC-09 | UC-10 | Luồng tiếp nối | Hàng hóa được kiểm tra và đóng gói trước khi bàn giao. |
| UC-10 | UC-11 | Luồng tiếp nối | Sau khi tiếp nhận hàng, đơn vị vận chuyển cập nhật trạng thái giao hàng. |
| UC-11 | UC-12 | Luồng điều kiện | UC-12 được kích hoạt khi kết quả giao hàng thất bại. |
| UC-12 | UC-09 | Luồng lặp | Nếu cần giao lại, đơn hàng quay về khâu chuẩn bị hàng hóa. |

### 3.3. Nhóm quản lý khiếu nại

| Use Case nguồn | Use Case liên quan | Mối quan hệ | Giải thích |
|---|---|---|---|
| UC-13 | UC-14 | Luồng tiếp nối | Sau khi khách hàng gửi khiếu nại, bộ phận chăm sóc khách hàng tiếp nhận. |
| UC-14 | UC-15 | Luồng tiếp nối | Khiếu nại được tiếp nhận trước khi kiểm tra tính hợp lệ. |
| UC-15 | UC-16 | Luồng điều kiện | Khiếu nại hợp lệ thì chuyển sang xử lý hàng hóa liên quan. |
| UC-16 | UC-17 | Luồng tiếp nối | Sau khi xử lý hàng hóa, tiến hành chuẩn bị hàng thay thế nếu cần. |
| UC-17 | UC-18 | Luồng tiếp nối | Sau khi hàng thay thế được gửi đi, cập nhật kết quả xử lý khiếu nại. |
| UC-15 | UC-18 | Luồng điều kiện | Nếu khiếu nại không hợp lệ, cần ghi nhận và thông báo kết quả cho khách hàng. |

## 4. Đề xuất sử dụng quan hệ Include và Extend

Không phải mọi mối liên hệ giữa các Use Case đều cần thể hiện bằng `include` hoặc `extend`. Các quan hệ này chỉ nên sử dụng khi phù hợp với bản chất chức năng.

| Quan hệ đề xuất | Loại quan hệ | Lý do |
|---|---|---|
| UC-03 → UC-04 | Extend | Xử lý hết hàng chỉ xảy ra khi kiểm tra tồn kho phát hiện không đủ hàng. |
| UC-11 → UC-12 | Extend | Xử lý giao hàng thất bại chỉ xảy ra khi giao hàng không thành công. |
| UC-15 → UC-16 | Extend | Xử lý hàng hóa liên quan chỉ diễn ra khi khiếu nại hợp lệ và cần xử lý hàng. |

Các quan hệ trên là đề xuất ban đầu. Cần xem xét lại ranh giới hệ thống và mục tiêu từng Use Case trước khi đưa vào sơ đồ chính thức.

## 5. Các điểm cần rà soát

### 5.1. UC-03 và UC-04 có khả năng chồng chéo

UC-03 đã mô tả nhánh xử lý khi hết hàng, bao gồm việc khách hàng lựa chọn hủy đơn hoặc thay thế sản phẩm.

Trong khi đó, UC-04 tiếp tục mô tả chính hoạt động này.

**Đề xuất:** Giữ UC-04 như một hành vi mở rộng của UC-03 nếu muốn phân tách chức năng xử lý hết hàng. Cần bảo đảm UC-03 chỉ mô tả việc kiểm tra tồn kho và xác định kết quả, tránh lặp lại toàn bộ nội dung UC-04.

### 5.2. UC-13 và UC-14 có khả năng trùng lặp

UC-13 mô tả khách hàng gửi khiếu nại, UC-14 mô tả nhân viên tiếp nhận khiếu nại.

**Đề xuất:** Có thể giữ hai Use Case nếu hệ thống thực sự hỗ trợ chức năng khách hàng gửi khiếu nại. Nếu khách hàng chỉ liên hệ qua điện thoại hoặc kênh bên ngoài, UC-13 có thể là hoạt động bên ngoài phạm vi hệ thống.

### 5.3. UC-16 và UC-17 cần phân biệt rõ

UC-16 tập trung vào việc tiếp nhận và kiểm tra hàng hóa liên quan đến khiếu nại.

UC-17 tập trung vào việc chuẩn bị và gửi hàng thay thế.

**Đề xuất:** Giữ hai Use Case riêng biệt để thể hiện hai mục tiêu nghiệp vụ khác nhau. Tuy nhiên, cần xác minh liệu mọi khiếu nại hợp lệ đều cần trả hàng cũ và gửi hàng thay thế hay không.

### 5.4. UC-10 và UC-11 cần xác định ranh giới

UC-10 mô tả việc bàn giao hàng hóa cho đơn vị vận chuyển.

UC-11 mô tả việc cập nhật trạng thái trong quá trình vận chuyển.

**Đề xuất:** Giữ riêng hai Use Case vì bàn giao và theo dõi trạng thái là hai hoạt động khác nhau. Cần xác minh cách đơn vị vận chuyển trao đổi dữ liệu với hệ thống doanh nghiệp.

## 6. Kết luận

18 Use Case đã được phân nhóm thành ba mảng nghiệp vụ chính:

1. Quản lý đơn hàng.
2. Thanh toán và giao hàng.
3. Quản lý khiếu nại.

Các Use Case có luồng phụ thuộc và điều kiện chuyển tiếp tương đối rõ ràng. Tuy nhiên, một số chức năng cần được rà soát thêm để tránh chồng chéo và xác định đúng phạm vi hệ thống.
