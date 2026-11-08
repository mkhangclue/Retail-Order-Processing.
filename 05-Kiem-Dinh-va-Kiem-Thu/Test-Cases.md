# Test Cases – Đặc tả trường hợp kiểm thử

## 1. Mục đích

Tài liệu mô tả chi tiết các trường hợp kiểm thử được xây dựng từ Test Scenarios, nhằm đánh giá khả năng xử lý các tình huống nghiệp vụ trong giải pháp đề xuất.

## 2. Chi tiết Test Cases

### Nhóm 1 – Kiểm soát tồn kho

#### TC-01-01: Sản phẩm còn đủ số lượng

| Thuộc tính | Nội dung |
|---|---|
| Scenario ID | TS-01-01 |
| Requirement | SR-01 |
| Priority | High |
| Preconditions | Đơn hàng đã được tiếp nhận. |
| Test Data | Số lượng đặt: 5; số lượng tồn kho: 10. |
| Steps | 1. Tiếp nhận đơn hàng. 2. Kiểm tra tồn kho. 3. Ghi nhận kết quả kiểm tra. |
| Expected Result | Kết quả kiểm tra được ghi nhận và đơn hàng được chuyển sang bước tiếp theo. |

#### TC-01-02: Sản phẩm không đủ số lượng

| Thuộc tính | Nội dung |
|---|---|
| Scenario ID | TS-01-02 |
| Requirement | SR-01 |
| Priority | High |
| Preconditions | Đơn hàng đã được tiếp nhận. |
| Test Data | Số lượng đặt: 10; số lượng tồn kho: 4. |
| Steps | 1. Tiếp nhận đơn hàng. 2. Kiểm tra tồn kho. 3. Ghi nhận kết quả. |
| Expected Result | Hệ thống nhận diện không đủ hàng và chuyển sang luồng xử lý hết hàng. |

#### TC-01-03: Thông tin tồn kho chưa được xác minh

| Thuộc tính | Nội dung |
|---|---|
| Scenario ID | TS-01-03 |
| Requirement | SR-01 |
| Priority | High |
| Preconditions | Đơn hàng đã được tiếp nhận. |
| Test Data | Trạng thái tồn kho: Chưa xác minh. |
| Steps | 1. Kiểm tra thông tin tồn kho. 2. Xác định trạng thái dữ liệu. |
| Expected Result | Chưa xác nhận khả năng đáp ứng đơn hàng; yêu cầu kiểm tra lại. |

### Nhóm 2 – Chuẩn hóa thông tin giao hàng

#### TC-02-01: Thông tin giao hàng đầy đủ

| Thuộc tính | Nội dung |
|---|---|
| Scenario ID | TS-02-01 |
| Requirement | SR-02 |
| Priority | High |
| Preconditions | Khách hàng đã cung cấp thông tin giao hàng. |
| Test Data | Người nhận: Nguyễn Văn A; số điện thoại: 0900000000; địa chỉ: 123 Đường A, TP.HCM. |
| Steps | 1. Tiếp nhận thông tin. 2. Kiểm tra các trường bắt buộc. 3. Ghi nhận thông tin. |
| Expected Result | Thông tin đầy đủ được ghi nhận và chuyển sang bước tiếp theo. |

#### TC-02-02: Thiếu thông tin giao hàng

| Thuộc tính | Nội dung |
|---|---|
| Scenario ID | TS-02-02 |
| Requirement | SR-02 |
| Priority | High |
| Preconditions | Khách hàng đã cung cấp thông tin giao hàng. |
| Test Data | Người nhận: Nguyễn Văn A; số điện thoại: Để trống; địa chỉ: 123 Đường A, TP.HCM. |
| Steps | 1. Tiếp nhận thông tin. 2. Kiểm tra tính đầy đủ. |
| Expected Result | Nhận diện trường thông tin còn thiếu và yêu cầu khách hàng bổ sung. |

#### TC-02-03: Khách hàng cập nhật thông tin còn thiếu

| Thuộc tính | Nội dung |
|---|---|
| Scenario ID | TS-02-03 |
| Requirement | SR-02 |
| Priority | High |
| Preconditions | Thông tin giao hàng đang thiếu số điện thoại. |
| Test Data | Số điện thoại bổ sung: 0900000000. |
| Steps | 1. Khách hàng bổ sung thông tin. 2. Nhân viên kiểm tra lại. 3. Ghi nhận kết quả. |
| Expected Result | Thông tin được kiểm tra lại; nếu đầy đủ thì chuyển sang bước tiếp theo. |

### Nhóm 3 – Theo dõi thời hạn thanh toán

#### TC-03-01: Khách hàng xác nhận thanh toán trong 2 ngày

| Thuộc tính | Nội dung |
|---|---|
| Scenario ID | TS-03-01 |
| Requirement | SR-03 |
| Priority | High |
| Preconditions | Đơn hàng đã được yêu cầu thanh toán. |
| Test Data | Thời điểm bắt đầu: 01/11/2026; thời điểm nhận xác nhận: 02/11/2026. |
| Steps | 1. Ghi nhận thời điểm bắt đầu tính hạn. 2. Nhận xác nhận thanh toán. 3. Kiểm tra thời hạn. |
| Expected Result | Xác nhận thanh toán được ghi nhận trong thời hạn 2 ngày. |

#### TC-03-02: Khách hàng không xác nhận trong 2 ngày

| Thuộc tính | Nội dung |
|---|---|
| Scenario ID | TS-03-02 |
| Requirement | SR-03 |
| Priority | High |
| Preconditions | Đơn hàng đang chờ xác nhận thanh toán. |
| Test Data | Thời điểm bắt đầu: 01/11/2026; thời điểm kiểm tra: 04/11/2026; chưa có xác nhận. |
| Steps | 1. Ghi nhận thời điểm bắt đầu. 2. Kiểm tra thời hạn. 3. Xác định chưa nhận được xác nhận. |
| Expected Result | Nhận diện đơn hàng quá hạn. Phương án xử lý tiếp theo: Pending Clarification. |

#### TC-03-03: Khách hàng xác nhận sau thời hạn

| Thuộc tính | Nội dung |
|---|---|
| Scenario ID | TS-03-03 |
| Requirement | SR-03 |
| Priority | Medium |
| Preconditions | Đơn hàng đã quá thời hạn xác nhận thanh toán. |
| Test Data | Thời điểm bắt đầu: 01/11/2026; thời điểm nhận xác nhận: 04/11/2026. |
| Steps | 1. Nhận xác nhận thanh toán. 2. Ghi nhận thời điểm nhận. 3. Đối chiếu thời hạn. |
| Expected Result | Ghi nhận xác nhận đến muộn; phương án xử lý đơn hàng: Pending Clarification. |

### Nhóm 4 – Kiểm soát giao hàng thất bại

#### TC-04-01: Giao hàng thành công

| Thuộc tính | Nội dung |
|---|---|
| Scenario ID | TS-04-01 |
| Requirement | SR-04 |
| Priority | High |
| Preconditions | Đơn hàng đã được bàn giao cho đơn vị vận chuyển. |
| Test Data | Trạng thái giao hàng: Thành công. |
| Steps | 1. Nhận kết quả giao hàng. 2. Ghi nhận trạng thái. 3. Kiểm tra kết quả. |
| Expected Result | Cập nhật trạng thái giao hàng thành công và hoàn tất đơn hàng. |

#### TC-04-02: Giao hàng thất bại lần đầu

| Thuộc tính | Nội dung |
|---|---|
| Scenario ID | TS-04-02 |
| Requirement | SR-04 |
| Priority | High |
| Preconditions | Đơn hàng đang trong quá trình vận chuyển. |
| Test Data | Số lần giao thất bại: 1. |
| Steps | 1. Nhận kết quả giao hàng thất bại. 2. Ghi nhận trạng thái. 3. Chuyển thông tin cho bộ phận CS. |
| Expected Result | Ghi nhận giao hàng thất bại và chuyển sang bước liên hệ khách hàng. |

#### TC-04-03: Giao hàng thất bại nhiều lần

| Thuộc tính | Nội dung |
|---|---|
| Scenario ID | TS-04-03 |
| Requirement | SR-04 |
| Priority | High |
| Preconditions | Đơn hàng đã từng giao thất bại và được giao lại. |
| Test Data | Số lần giao thất bại: 2. |
| Steps | 1. Nhận kết quả giao hàng. 2. Cập nhật số lần thất bại. 3. Kiểm tra giới hạn giao lại. |
| Expected Result | Số lần thất bại được ghi nhận và đối chiếu với giới hạn đã được phê duyệt. |

#### TC-04-04: Đơn hàng đạt giới hạn giao lại

| Thuộc tính | Nội dung |
|---|---|
| Scenario ID | TS-04-04 |
| Requirement | SR-04 |
| Priority | High |
| Preconditions | Đã xác định giới hạn số lần giao lại. |
| Test Data | Số lần giao lại hiện tại bằng giới hạn được phê duyệt. |
| Steps | 1. Ghi nhận kết quả giao thất bại. 2. Kiểm tra số lần giao lại. 3. Đối chiếu giới hạn. |
| Expected Result | Nhận diện đơn hàng đã đạt giới hạn và chuyển sang phương án xử lý tiếp theo theo chính sách. |

### Nhóm 5 – Chuẩn hóa xử lý khiếu nại

#### TC-05-01: Khiếu nại thiếu hàng

| Thuộc tính | Nội dung |
|---|---|
| Scenario ID | TS-05-01 |
| Requirement | SR-05 |
| Priority | High |
| Preconditions | Khách hàng đã nhận hàng. |
| Test Data | Loại khiếu nại: Thiếu sản phẩm trong đơn hàng. |
| Steps | 1. Khách hàng gửi khiếu nại. 2. Nhân viên tiếp nhận. 3. Yêu cầu hình ảnh hoặc bằng chứng. |
| Expected Result | Khiếu nại được ghi nhận và chuyển sang bước xác minh. |

#### TC-05-02: Khiếu nại hàng hóa hư hỏng

| Thuộc tính | Nội dung |
|---|---|
| Scenario ID | TS-05-02 |
| Requirement | SR-05 |
| Priority | High |
| Preconditions | Khách hàng đã nhận hàng. |
| Test Data | Loại khiếu nại: Sản phẩm bị hư hỏng; có hình ảnh minh chứng. |
| Steps | 1. Tiếp nhận khiếu nại. 2. Kiểm tra hình ảnh. 3. Đối chiếu thông tin đơn hàng. |
| Expected Result | Bằng chứng được ghi nhận để đánh giá tính hợp lệ. |

#### TC-05-03: Khiếu nại giao sai hàng

| Thuộc tính | Nội dung |
|---|---|
| Scenario ID | TS-05-03 |
| Requirement | SR-05 |
| Priority | High |
| Preconditions | Khách hàng đã nhận hàng. |
| Test Data | Sản phẩm đặt mua khác với sản phẩm nhận được. |
| Steps | 1. Tiếp nhận khiếu nại. 2. Kiểm tra thông tin đơn hàng. 3. Thu thập bằng chứng. |
| Expected Result | Khiếu nại được ghi nhận và chuyển sang bước xác minh. |

#### TC-05-04: Khiếu nại không hợp lệ

| Thuộc tính | Nội dung |
|---|---|
| Scenario ID | TS-05-04 |
| Requirement | SR-05 |
| Priority | High |
| Preconditions | Có khiếu nại và bằng chứng để đánh giá. |
| Test Data | Kết quả đối chiếu: Không đáp ứng tiêu chí hợp lệ đã được phê duyệt. |
| Steps | 1. Kiểm tra nội dung khiếu nại. 2. Đối chiếu bằng chứng. 3. Đánh giá tính hợp lệ. |
| Expected Result | Ghi nhận khiếu nại không hợp lệ và thông báo cho khách hàng. |

#### TC-05-05: Khiếu nại hợp lệ

| Thuộc tính | Nội dung |
|---|---|
| Scenario ID | TS-05-05 |
| Requirement | SR-05 |
| Priority | High |
| Preconditions | Có khiếu nại và bằng chứng để đánh giá. |
| Test Data | Kết quả đối chiếu: Đáp ứng tiêu chí hợp lệ đã được phê duyệt. |
| Steps | 1. Kiểm tra nội dung khiếu nại. 2. Đối chiếu bằng chứng. 3. Xác nhận tính hợp lệ. |
| Expected Result | Chuyển sang quy trình xử lý hàng hóa và phương án giải quyết phù hợp. |

## 3. Tổng hợp Test Cases

| Nhóm | Số lượng |
|---|---:|
| Kiểm soát tồn kho | 3 |
| Thông tin giao hàng | 3 |
| Thanh toán | 3 |
| Giao hàng thất bại | 4 |
| Khiếu nại | 5 |
| **Tổng cộng** | **18** |

## 4. Quy ước đánh giá

| Trạng thái | Ý nghĩa |
|---|---|
| Not Run | Chưa thực hiện |
| Pass | Kết quả phù hợp với Expected Result |
| Fail | Kết quả không phù hợp với Expected Result |
| Blocked | Không thể đánh giá do thiếu điều kiện hoặc quy tắc |
| Pending Clarification | Chờ Stakeholder xác nhận quy tắc nghiệp vụ |

## 5. Ghi chú

- Dữ liệu trong tài liệu là dữ liệu giả lập phục vụ kiểm thử.
- Các Test Cases chưa được thực thi trên hệ thống phần mềm thực tế.
- Những trường hợp phụ thuộc chính sách chưa xác nhận không được tự kết luận Pass hoặc Fail.
- Cần cập nhật kết quả thực hiện trong Test Execution Report khi có môi trường kiểm thử phù hợp.

**Trạng thái:** Test Cases – Draft.
