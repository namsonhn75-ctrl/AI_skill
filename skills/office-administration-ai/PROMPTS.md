# Office Administration AI — PROMPTS

## 0. Khung Prompt 6 thành phần

~~~text
ROLE: Bạn là [vai trò].
TASK: Hãy [công việc].
CONTEXT: [mục đích/người nhận/phạm vi].
INPUT: [file/dữ liệu/nguồn].
OUTPUT: [bảng/văn bản/checklist].
CONSTRAINT: [độ dài/giọng văn/điều cấm].
~~~

## 1. Tài liệu → Tóm tắt + Bảng hành động

~~~text
Đọc tài liệu và tạo:
1. Tóm tắt nội dung chính.
2. Bảng: Công việc | Chủ trì | Phối hợp | Hạn | Sản phẩm.
3. Nội dung thiếu/mâu thuẫn/cần xác nhận.

Chỉ sử dụng thông tin trong tài liệu.
Không tự thêm người, deadline, số liệu, căn cứ hoặc kết luận.
Thiếu dữ liệu ghi [CẦN XÁC NHẬN].
Giữ nguyên mức độ chắc chắn của nguồn.
~~~

## 2. Ghi chú lãnh đạo → Bảng giao việc

~~~text
Trích xuất:
Việc | Chủ trì | Phối hợp | Hạn | Sản phẩm | Trạng thái.

Đánh dấu việc trùng, mô tả mơ hồ, thiếu người, thiếu deadline, thiếu sản phẩm.
Không tự gán người hoặc tạo deadline.
~~~

## 3. Bảng thông tin → Email triển khai

~~~text
Từ bảng thông tin đã xác nhận, soạn email cho [đối tượng].
Mục đích, việc, người, deadline và sản phẩm phải rõ nếu nguồn có.
Giọng văn: [yêu cầu].
Không thêm thông tin ngoài bảng đã xác nhận.
~~~

## 4. Chỉnh văn bản hành chính

~~~text
Chỉnh văn bản cho rõ ràng, mạch lạc, lịch sự.
Giữ nguyên tên người/đơn vị, số liệu, thời hạn, nội dung và mức độ chắc chắn.
Không thêm căn cứ, ngày tháng, địa điểm, người ký hoặc thông tin mới.
Phần thiếu ghi [CẦN BỔ SUNG].
~~~

## 5. JD / Mô tả công việc

~~~text
Từ dữ liệu nguồn, tạo:
1. Mục tiêu vị trí.
2. Nhiệm vụ chính.
3. Trách nhiệm.
4. Yêu cầu kinh nghiệm/kỹ năng/thái độ.
5. Người báo cáo.
6. Tiêu chí đánh giá nếu nguồn có.
7. Thông tin còn thiếu.

Không tự thêm tiêu chí chưa có trong nguồn.
~~~

## 6. Tin tuyển dụng

~~~text
Tạo tin tuyển dụng gồm:
Tiêu đề | Giới thiệu | Nhiệm vụ | Yêu cầu | Quyền lợi nếu có | Hồ sơ | Cách ứng tuyển.
Không tự thêm lương, quyền lợi, địa điểm hoặc tiêu chí.
Thiếu thông tin ghi [CẦN BỔ SUNG].
Không tự quyết định tuyển/loại ứng viên.
~~~

## 7. Chuẩn hóa danh sách công việc

~~~text
Chuẩn hóa:
Công việc chuẩn | Trùng/không trùng | P1/P2/P3 | Deadline | Phụ trách | Sản phẩm | Trạng thái | Thiếu thông tin.
Phát hiện việc trùng, việc quá lớn, mô tả mơ hồ và phụ thuộc.
Không tự tạo deadline hoặc gán người.
~~~

## 8. Kế hoạch tuần

~~~text
Từ danh sách việc đã chuẩn hóa, lập kế hoạch Thứ Hai–Thứ Sáu:
Ngày | Ưu tiên | Công việc | Deadline | Sản phẩm | Trạng thái.
Tách Chờ thông tin / Chờ phản hồi / Chờ phê duyệt.
Không tự tạo deadline. Giữ khoảng trống cho việc phát sinh.
~~~

## 9. Transcript → Phân loại

~~~text
Đọc transcript và CHƯA viết biên bản.
Phân loại: Ý kiến/trao đổi | Kết luận | Nhiệm vụ | Chưa chốt.
Bảng: Nội dung | Loại | Người liên quan | Deadline | Căn cứ | Ghi chú.
Không biến ý kiến thành kết luận. Không tự thêm người/hạn.
~~~

## 10. Phân loại → Biên bản

~~~text
Dựa trên bảng phân loại đã xác nhận, soạn biên bản gồm:
Thời gian – địa điểm – thành phần; mục tiêu; trao đổi chính; kết luận;
nhiệm vụ; nội dung chưa chốt.
Không biến đề xuất thành kết luận.
~~~

## 11. Biên bản → Bảng hành động

~~~text
Lập:
STT | Công việc | Chủ trì | Phối hợp | Hạn | Sản phẩm | Trạng thái.
Không thêm người hoặc deadline chưa có. Thiếu ghi [CẦN XÁC NHẬN].
~~~

## 12. Nhiều báo cáo → Bảng chuẩn hóa

~~~text
Chuẩn hóa:
Đơn vị | Việc chính | Trạng thái | Kết quả | Vướng mắc | Deadline | Việc tiếp theo.
Sau đó lập riêng: nội dung trùng, khác số liệu, khác trạng thái, khác deadline,
thông tin chỉ có ở một nguồn.
Không tự chọn nguồn đúng khi chưa có căn cứ.
~~~

## 13. Bảng chuẩn hóa → Báo cáo tổng hợp

~~~text
Viết báo cáo 1–2 trang:
1. Tình hình chung
2. Kết quả đã đạt
3. Công việc đang triển khai
4. Vướng mắc/rủi ro
5. Nội dung cần xác nhận
6. Nhiệm vụ kỳ tiếp theo

Mỗi nhận xét quan trọng phải truy được về nguồn.
Không suy đoán nguyên nhân.
~~~

## 14. Excel → Theo dõi tiến độ

~~~text
Ngày báo cáo: [DD/MM/YYYY].
Phân loại: Hoàn thành | Đang thực hiện | Quá hạn | Sắp đến hạn |
Đang chờ | Chưa đủ dữ liệu | Bất thường.

Quá hạn = deadline trước ngày báo cáo và chưa hoàn thành.
Sắp đến hạn = theo khoảng thời gian được chỉ định.
Không tự tạo deadline, sửa trạng thái hoặc %.
Nếu trạng thái và % mâu thuẫn, đánh dấu bất thường.
~~~

## 15. Executive Brief

~~~text
Viết tóm tắt:
1. Tình hình chung
2. Kết quả đáng chú ý
3. Vấn đề/rủi ro
4. Nguyên nhân có căn cứ
5. Nội dung cần quyết định
6. Hành động: Việc | Đơn vị | Hạn

Không suy đoán nguyên nhân. Nếu thiếu dữ liệu, ghi
"Chưa đủ căn cứ xác định nguyên nhân".
Không biến đề xuất thành quyết định.
~~~

## 16. Phân tích bảng dữ liệu

~~~text
Mô tả ý nghĩa từng cột và đơn vị đo trước.
Xác định 3 điểm đáng chú ý, nêu số liệu làm căn cứ, đánh dấu bất thường,
không suy đoán nguyên nhân và đề xuất 3 câu hỏi kiểm tra thêm.
Tách rõ: Sự kiện | Suy luận có căn cứ | Câu hỏi kiểm tra.
~~~

## 17. Prompt phản biện

~~~text
Kiểm tra câu trả lời vừa tạo:
1. Giả định đã sử dụng.
2. Thông tin chưa có căn cứ.
3. Dữ liệu còn thiếu.
4. Kết luận cần người chuyên môn xác nhận.
5. Nguy cơ nhầm người/hạn/trạng thái/số liệu.
Sau đó viết lại thận trọng hơn.
~~~

## 18. Chỉ dùng dữ liệu nguồn

~~~text
Chỉ sử dụng dữ liệu trong các file/nguồn tôi cung cấp.
Không web search; không dùng kiến thức ngoài để lấp chỗ trống;
không tự sửa số liệu; không tự chọn nguồn trong các nguồn mâu thuẫn;
không tự tạo người, deadline, căn cứ, trạng thái hoặc kết luận.
Thiếu hoặc mâu thuẫn thì ghi [CẦN XÁC NHẬN].
~~~

## 19. Xử lý mâu thuẫn

~~~text
Lập bảng:
Nội dung | Nguồn A | Nguồn B | Loại mâu thuẫn | Tác động | Cần xác nhận từ ai.
Không tự chọn nguồn đúng, không lấy trung bình, không sửa dữ liệu nguồn.
~~~

## 20. Chuỗi prompt cho công việc lớn

~~~text
BƯỚC 1: Trích xuất.
BƯỚC 2: Chuẩn hóa.
BƯỚC 3: Kiểm tra thiếu.
BƯỚC 4: Phát hiện mâu thuẫn.
BƯỚC 5: Xác nhận.
BƯỚC 6: Tạo đầu ra nghiệp vụ.
BƯỚC 7: Kiểm chứng.
BƯỚC 8: Báo cáo quản trị/hành động.
~~~
