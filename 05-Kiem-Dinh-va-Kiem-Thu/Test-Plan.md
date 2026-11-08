# Test Plan – Kế hoạch kiểm thử

## 1. Mục đích

Tài liệu xác định phạm vi, phương pháp và cách thức kiểm thử các yêu cầu trong dự án phân tích và cải tiến quy trình xử lý đơn hàng bán lẻ.

Mục tiêu:
- Kiểm tra tính nhất quán của các yêu cầu nghiệp vụ.
- Đánh giá khả năng xử lý các tình huống nghiệp vụ.
- Xác định những trường hợp chưa được mô tả đầy đủ.
- Đối chiếu kết quả kiểm thử với yêu cầu đã xây dựng.

## 2. Phạm vi kiểm thử

Kiểm thử tập trung vào 5 nhóm giải pháp:

| ID | Nhóm kiểm thử | Nội dung |
|---|---|---|
| TC-G01 | Kiểm soát tồn kho | Kiểm tra trường hợp đủ hàng và hết hàng. |
| TC-G02 | Thông tin giao hàng | Kiểm tra thông tin đầy đủ và chưa đầy đủ. |
| TC-G03 | Thanh toán | Kiểm tra xác nhận thanh toán đúng hạn và quá hạn. |
| TC-G04 | Giao hàng thất bại | Kiểm tra tình huống giao hàng thất bại và giao lại. |
| TC-G05 | Khiếu nại | Kiểm tra tiếp nhận, xác minh và xử lý khiếu nại. |

## 3. Phương pháp kiểm thử

| Phương pháp | Mục đích |
|---|---|
| Requirements Review | Kiểm tra tính rõ ràng và nhất quán của yêu cầu. |
| Scenario-based Testing | Xây dựng tình huống để kiểm tra luồng nghiệp vụ. |
| Traceability Review | Kiểm tra liên kết giữa Problem, BR, FR, UC và SR. |
| Expected Result Evaluation | Đối chiếu kết quả mong đợi với quy tắc nghiệp vụ. |

## 4. Tiêu chí kiểm thử

Một tình huống được đánh giá là đạt khi:

- Có đầy đủ điều kiện đầu vào.
- Luồng xử lý phù hợp với yêu cầu đã xác định.
- Kết quả mong đợi được mô tả rõ ràng.
- Không có mâu thuẫn với Business Rules.
- Những nội dung chưa có quy định phải được ghi nhận là vấn đề cần xác minh, không tự suy diễn kết quả.

## 5. Môi trường và dữ liệu kiểm thử

- Môi trường: Mô phỏng nghiệp vụ trên tài liệu.
- Dữ liệu: Dữ liệu giả lập phục vụ xây dựng tình huống kiểm thử.
- Hệ thống thực tế: Chưa có.
- Công cụ: GitHub, Draw.io và tài liệu Markdown.

## 6. Kết quả đầu ra

| Tài liệu | Mục đích |
|---|---|
| Test-Scenarios.md | Danh sách các tình huống kiểm thử. |
| Test-Cases.md | Chi tiết điều kiện, bước thực hiện và kết quả mong đợi. |
| Test-Execution-Report.md | Ghi nhận kết quả đánh giá từng trường hợp. |
| Defect-Log.md | Ghi nhận vấn đề phát hiện trong quá trình kiểm thử. |

## 7. Giới hạn kiểm thử

- Chưa thực hiện kiểm thử trên phần mềm thực tế.
- Chưa có dữ liệu sản xuất hoặc dữ liệu khách hàng thực tế.
- Các kết quả kiểm thử chỉ phản ánh tính hợp lý của mô hình nghiệp vụ và tài liệu yêu cầu.
- Những quy tắc chưa được Stakeholder xác nhận sẽ được đánh dấu là Pending Clarification.

## 8. Kết luận

Kế hoạch kiểm thử được xây dựng nhằm đánh giá sơ bộ tính đầy đủ, nhất quán và khả năng đáp ứng của bộ yêu cầu nghiệp vụ.

Kết quả kiểm thử sẽ là cơ sở để rà soát và hoàn thiện tài liệu trước khi tổng kết dự án.

**Trạng thái:** Test Plan – Draft.
