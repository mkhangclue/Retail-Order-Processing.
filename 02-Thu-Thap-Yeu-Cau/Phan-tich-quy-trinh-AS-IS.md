# PHÂN TÍCH QUY TRÌNH HIỆN TRẠNG (AS-IS ANALYSIS)

## 1. Mục đích

Phân tích quy trình xử lý đơn hàng bán lẻ hiện tại dựa trên các sơ đồ BPMN đã xây dựng, nhằm hiểu rõ trình tự hoạt động, các bên tham gia, dữ liệu đầu vào, đầu ra và các điểm cần được làm rõ.

## 2. Phạm vi phân tích

Phân tích bao gồm hai mô hình:

- Quy trình tổng thể: Quy trình xử lý đơn hàng bán lẻ.
- Quy trình con: Kiểm tra thông tin đơn hàng và tình trạng hàng hóa.

## 3. Phân rã quy trình hiện trạng

| STT | Giai đoạn | Hoạt động chính | Kết quả |
|---|---|---|---|
| 1 | Tiếp nhận đơn hàng | Tiếp nhận yêu cầu và tạo đơn hàng. | Đơn hàng đã nhận |
| 2 | Kiểm tra thông tin và hàng hóa | Kiểm tra thông tin đơn hàng và tình trạng tồn kho. | Kết quả kiểm tra |
| 3 | Xác nhận thông tin giao hàng | Thu thập và kiểm tra thông tin người nhận. | Thông tin giao hàng |
| 4 | Lập hóa đơn | Hoàn thiện thông tin và lập hóa đơn. | Hóa đơn |
| 5 | Thanh toán và chuẩn bị hàng | Yêu cầu thanh toán, kiểm tra và đóng gói hàng hóa. | Hàng đã đóng gói |
| 6 | Vận chuyển | Bàn giao đơn vị vận chuyển và cập nhật trạng thái. | Kết quả giao hàng |
| 7 | Xử lý ngoại lệ | Xử lý giao hàng thất bại và khiếu nại. | Kết quả xử lý |
| 8 | Kết thúc | Cập nhật trạng thái và thông báo kết quả. | Đơn hàng hoàn tất hoặc kết thúc theo nhánh xử lý |

## 4. Phân tích Input – Process – Output

| Giai đoạn | Input | Process | Output |
|---|---|---|---|
| Tiếp nhận đơn hàng | Yêu cầu đặt hàng | Ghi nhận và tạo đơn hàng | Đơn hàng đã nhận |
| Kiểm tra hàng hóa | Thông tin sản phẩm, dữ liệu tồn kho | Kiểm tra tình trạng hàng | Kết quả kiểm tra hàng |
| Xác nhận giao hàng | Thông tin người nhận | Kiểm tra và cập nhật thông tin | Thông tin giao hàng |
| Lập hóa đơn | Thông tin đơn hàng và giao hàng | Lập hóa đơn | Hóa đơn |
| Chuẩn bị hàng | Đơn hàng, thông tin đóng gói | Kiểm tra và đóng gói | Hàng đã đóng gói |
| Vận chuyển | Hàng hóa, thông tin giao hàng | Thực hiện giao hàng | Kết quả giao hàng |
| Xử lý ngoại lệ | Thông tin giao thất bại hoặc khiếu nại | Xác minh và xử lý | Kết quả xử lý ngoại lệ |

## 5. Các điểm cần làm rõ

| Mã | Nội dung | Mô tả |
|---|---|---|
| AS-01 | Ranh giới giữa quy trình tổng thể và subprocess | Cần xác định rõ vị trí gọi subprocess và hoạt động lập hóa đơn để tránh trùng lặp. |
| AS-02 | Quản lý dữ liệu tồn kho | Chưa làm rõ cách cập nhật và kiểm soát độ chính xác của dữ liệu tồn kho. |
| AS-03 | Xác nhận thông tin giao hàng | Chưa có tiêu chí cụ thể để xác định thông tin giao hàng hợp lệ. |
| AS-04 | Giao hàng thất bại | Chưa xác định số lần giao lại và điều kiện kết thúc việc giao lại. |
| AS-05 | Xử lý khiếu nại | Chưa mô tả tiêu chí đánh giá khiếu nại hợp lệ và thời gian xử lý. |

## 6. Nhận xét sơ bộ

Quy trình hiện trạng đã thể hiện các hoạt động chính từ tiếp nhận đơn hàng đến giao hàng và xử lý ngoại lệ.

Tuy nhiên, một số điều kiện nghiệp vụ, trách nhiệm phối hợp và tiêu chí xử lý chưa được mô tả chi tiết trong tài liệu hiện có.

Các điểm cần làm rõ sẽ được sử dụng làm cơ sở cho bước phân tích vấn đề, rủi ro và nguyên nhân.

## 7. Nguồn phân tích

- Sơ đồ BPMN quy trình xử lý đơn hàng bán lẻ.
- Sơ đồ BPMN subprocess kiểm tra thông tin đơn hàng và tình trạng hàng hóa.
- Tài liệu mô tả quy trình nghiệp vụ hiện có.

**Lưu ý:** Phân tích được thực hiện dựa trên mô hình quy trình và tài liệu. Các nhận xét chưa được xác minh bằng dữ liệu vận hành thực tế.
