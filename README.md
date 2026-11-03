# Quy trình xử lý đơn hàng bán lẻ

Mô hình hóa và mô tả quy trình xử lý đơn hàng bán lẻ bằng BPMN.
## 1. Giới thiệu

Project mô hình hóa quy trình nghiệp vụ của một nhà phân phối thiết bị, tập trung vào quy trình xử lý đơn hàng bán lẻ.
Quy trình bắt đầu từ khi khách hàng gửi yêu cầu đặt hàng và bao gồm các hoạt động tiếp nhận đơn hàng, xác nhận thông tin, xử lý hóa đơn, kiểm tra và đóng gói hàng hóa, vận chuyển, giao hàng và xử lý các trường hợp giao hàng thất bại hoặc phát sinh khiếu nại.
Mô hình được xây dựng bằng BPMN 2.0 nhằm trực quan hóa luồng nghiệp vụ, các bên tham gia và các điểm quyết định trong quy trình.
## 2. Mục tiêu

- Mô hình hóa quy trình xử lý đơn hàng bằng BPMN 2.0.
- Xác định các bên tham gia và vai trò trong quy trình.
- Biểu diễn luồng xử lý và các điểm quyết định của nghiệp vụ.
- Mô tả các trường hợp ngoại lệ như giao hàng thất bại và khiếu nại.
- Xây dựng tài liệu mô tả chi tiết để hỗ trợ việc đọc và phân tích mô hình BPMN.
## 3. Phạm vi quy trình
Quy trình bao gồm các giai đoạn chính:

1. Tiếp nhận và xác nhận yêu cầu đơn hàng.
2. Xử lý hóa đơn và thanh toán.
3. Kiểm tra và đóng gói hàng hóa.
4. Chuẩn bị và thực hiện giao hàng.
5. Cập nhật trạng thái đơn hàng.
6. Xử lý giao hàng thất bại và gửi lại hàng.
7. Xử lý khiếu nại về hàng hóa.
8. Kết thúc quy trình khi đơn hàng được giao thành công hoặc khiếu nại được xử lý hoàn tất.
## 4. Các bên tham gia

| Bên tham gia | Vai trò |
| --- | --- |
| Khách hàng | Gửi yêu cầu đặt hàng, xác nhận thông tin, thanh toán và phản hồi khi phát sinh vấn đề. |
| Công ty | Tiếp nhận và xử lý đơn hàng, hóa đơn và phối hợp các bộ phận liên quan. |
| Nhân viên bán hàng | Xác nhận phương thức giao hàng và trao đổi với khách hàng. |
| Nhân viên kho hàng | Kiểm tra đơn hàng và thực hiện đóng gói hàng hóa. |
| Đơn vị vận chuyển | Kiểm tra thông tin giao hàng và thực hiện vận chuyển. |
| Bộ phận chăm sóc khách hàng | Tiếp nhận và xử lý các trường hợp giao hàng thất bại hoặc khiếu nại. |
## 5. Sub-process: Xử lý đơn hàng
Sub-process xử lý đơn hàng mô tả các hoạt động xử lý đơn hàng sau khi đơn hàng được tiếp nhận.
Các bước chính bao gồm:

- Kiểm tra tình trạng còn hàng.
- Xử lý trường hợp sản phẩm không còn hàng.
- Tiếp nhận lựa chọn của khách hàng.
- Xử lý trường hợp khách hàng hủy đơn hoặc lựa chọn sản phẩm khác.
- Thu thập thông tin giao hàng.
- Kiểm tra và cập nhật thông tin giao hàng khi cần.
- Lập hóa đơn đơn hàng.
## 6. Công cụ sử dụng

- BPMN 2.0
- diagrams.net (draw.io)
- Microsoft Word
## 7. Cấu trúc repository

```text
quy-trinh-xu-ly-don-hang-ban-le/
│
├── BPMN/
│   ├── Quy trình xử lý đơn hàng bán lẻ.pdf
│   └── Quy trình xử lý đơn hàng - Sub-process.pdf
│
├── Documentation/
│   ├── Mô tả Quy trình Xử lý Đơn hàng Bán lẻ.docx
│   └── Mô tả Quy trình Xử lý Đơn hàng - Quy trình con.docx
│
└── README.md
```
## 8. Tài liệu
### BPMN

- [Quy trình xử lý đơn hàng bán lẻ](./BPMN/Quy%20trình%20xử%20lý%20đơn%20hàng%20bán%20lẻ.pdf)
- [Quy trình xử lý đơn hàng - Sub-process](./BPMN/Quy%20trình%20xử%20lý%20đơn%20hàng%20-%20Sub-process.pdf)
### Documentation
- [Mô tả Quy trình Xử lý Đơn hàng Bán lẻ](./Documentation/Mô%20tả%20Quy%20trình%20Xử%20lý%20Đơn%20hàng%20Bán%20lẻ.docx)
- [Mô tả Quy trình Xử lý Đơn hàng - Quy trình con](./Documentation/Mô%20tả%20Quy%20trình%20Xử%20lý%20Đơn%20hàng%20-%20Quy%20trình%20con.docx)
