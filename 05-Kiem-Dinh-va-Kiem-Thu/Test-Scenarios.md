# Test Scenarios – Danh sách tình huống kiểm thử

## 1. Mục đích

Xác định các tình huống nghiệp vụ cần kiểm thử dựa trên 5 nhóm Solution Requirements đã xây dựng trong Phase 4.

## 2. Danh sách Test Scenarios

### TS-01 – Kiểm soát tồn kho (SR-01)

| Scenario ID | Tình huống | Kết quả mong đợi |
|---|---|---|
| TS-01-01 | Sản phẩm còn đủ số lượng trong kho. | Ghi nhận kết quả kiểm tra và cho phép tiếp tục xử lý đơn. |
| TS-01-02 | Sản phẩm không đủ số lượng trong kho. | Chuyển sang luồng xử lý hết hàng. |
| TS-01-03 | Thông tin tồn kho chưa được cập nhật hoặc chưa xác minh. | Chưa xác nhận khả năng đáp ứng đơn hàng; yêu cầu kiểm tra lại. |

### TS-02 – Chuẩn hóa thông tin giao hàng (SR-02)

| Scenario ID | Tình huống | Kết quả mong đợi |
|---|---|---|
| TS-02-01 | Khách hàng cung cấp đầy đủ thông tin giao hàng. | Thông tin được ghi nhận và chuyển sang bước tiếp theo. |
| TS-02-02 | Khách hàng thiếu địa chỉ hoặc số điện thoại. | Yêu cầu bổ sung thông tin còn thiếu. |
| TS-02-03 | Khách hàng cập nhật thông tin theo yêu cầu. | Thông tin được kiểm tra lại trước khi tiếp tục xử lý. |

### TS-03 – Theo dõi thời hạn thanh toán (SR-03)

| Scenario ID | Tình huống | Kết quả mong đợi |
|---|---|---|
| TS-03-01 | Khách hàng gửi xác nhận thanh toán trong 2 ngày. | Ghi nhận xác nhận thanh toán và tiếp tục quy trình. |
| TS-03-02 | Hết 2 ngày nhưng chưa nhận được xác nhận thanh toán. | Nhận diện đơn hàng quá hạn và chuyển sang trạng thái chờ xử lý theo chính sách. |
| TS-03-03 | Khách hàng gửi xác nhận sau thời hạn 2 ngày. | Ghi nhận thời điểm nhận xác nhận và chờ xử lý theo quy định được xác nhận. |

### TS-04 – Kiểm soát giao hàng thất bại (SR-04)

| Scenario ID | Tình huống | Kết quả mong đợi |
|---|---|---|
| TS-04-01 | Đơn hàng được giao thành công. | Cập nhật trạng thái giao hàng thành công và hoàn tất đơn. |
| TS-04-02 | Đơn hàng giao thất bại lần đầu. | Ghi nhận thất bại và chuyển sang bước liên hệ khách hàng. |
| TS-04-03 | Đơn hàng tiếp tục giao thất bại sau khi giao lại. | Ghi nhận số lần thất bại và kiểm tra giới hạn giao lại theo chính sách. |
| TS-04-04 | Đơn hàng đạt giới hạn số lần giao lại. | Chuyển sang phương án xử lý tiếp theo theo chính sách được xác nhận. |

### TS-05 – Chuẩn hóa xử lý khiếu nại (SR-05)

| Scenario ID | Tình huống | Kết quả mong đợi |
|---|---|---|
| TS-05-01 | Khách hàng khiếu nại hàng hóa bị thiếu. | Tiếp nhận khiếu nại và yêu cầu bằng chứng liên quan. |
| TS-05-02 | Khách hàng khiếu nại hàng hóa bị hư hỏng. | Tiếp nhận và kiểm tra hình ảnh, bằng chứng. |
| TS-05-03 | Khách hàng khiếu nại giao sai hàng. | Tiếp nhận và kiểm tra thông tin đơn hàng cùng bằng chứng. |
| TS-05-04 | Khiếu nại không đáp ứng tiêu chí hợp lệ. | Ghi nhận kết quả không hợp lệ và thông báo cho khách hàng. |
| TS-05-05 | Khiếu nại đáp ứng tiêu chí hợp lệ. | Chuyển sang quy trình xử lý hàng hóa và phương án giải quyết phù hợp. |

## 3. Tổng hợp số lượng

| Nhóm | Số tình huống |
|---|---:|
| TS-01 – Tồn kho | 3 |
| TS-02 – Thông tin giao hàng | 3 |
| TS-03 – Thanh toán | 3 |
| TS-04 – Giao hàng thất bại | 4 |
| TS-05 – Khiếu nại | 5 |
| **Tổng cộng** | **18** |

## 4. Ghi chú

- Các tình huống được xây dựng dựa trên BPMN AS-IS và Solution Requirements.
- Kết quả mong đợi là kết quả dự kiến theo giải pháp đề xuất, không phải kết quả từ hệ thống thực tế.
- Các tình huống liên quan đến thanh toán quá hạn, giới hạn giao lại và tiêu chí khiếu nại cần được xác nhận với Stakeholder trước khi chốt.
- Chưa thực hiện kiểm thử trên phần mềm thực tế.

**Trạng thái:** Test Scenarios – Draft.
