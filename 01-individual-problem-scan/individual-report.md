# 01 — Individual Problem Scan

> Điền theo Phase 1 + Phase 2 trong `01-worksheet.md`. Tự scan trước, dùng AI sau để phản biện. Không copy ví dụ Weekly Report.

## Thông tin cá nhân

- Họ và tên: Phạm Quang Đạt
- Mã học viên: 2A202602704
- Vai trò / bối cảnh: CTV dạy Python online tại công ty cổ phần giáo dục trực tuyến X
- Công việc hằng tuần (3-5 gạch đầu dòng để soi problem):
+ đọc các bài giảng có sẵn trên LMS,
+ soạn giáo án theo khung,
+ kiểm tra BTVN và quiz của học sinh,
+ tạo lịch các buổi học cho từng lớp bằng link Zoom
+ đánh giá học sinh trong vòng 8 giờ sau buổi học,
+ phản hồi với PH và quản lý lớp học về tình trạng từng học sinh
---

## Phase 1 — Scan 5+ problems (tối thiểu 5, khuyến khích 8-10)

**Cách điền:** mỗi dòng = việc gì + ai chịu + đo bằng gì. Cột `Dấu hiệu thật` bắt buộc có số: mất bao lâu (bấm giờ mấy lần), mấy lần/tuần, bao nhiêu người gặp, log/ticket/quote nào.

| # | Lăng kính (Lặp lại / Tốn thời gian / AI có thể tốt hơn / Pain từ người khác) | Problem quan sát được | Ai chịu ảnh hưởng? | Dấu hiệu thật (số + bằng chứng) |
|---|---|---|---|---|
1|Lặp lại |Tạo và đăng đúng link Zoom cho từng buổi của từng lớp phải lặp lại nhiều thao tác, dễ gắn nhầm lớp hoặc sai thời gian.|CTV giảng dạy; học sinh bị ảnh hưởng nếu link sai|1-2 buổi/khóa bị lỗi link|
2|Lặp lại|Sau mỗi buổi, CTV phải đối chiếu và ghi lại điểm danh hoặc tình trạng tham gia của từng học sinh.	|CTV và quản lý lớp	|15 phút/lớp|
3|Tốn thời gian|Khi đổi lịch đột xuất, cùng một thay đổi phải được cập nhật và xác nhận ở nhiều nơi.|CTV, quản lý lớp, học sinh và phụ huynh|15p - 20p/buổi|
4|Tốn thời gian|Để hoàn thành đánh giá trong 8 giờ, CTV phải gom bằng chứng của từng học sinh từ nhiều nguồn trước khi có thể đánh giá.|CTV giảng dạy|5-7 phút/học sinh|
5|AI có thể tốt hơn|Việc tổng hợp các lỗi Python phổ biến của cả lớp đang phụ thuộc vào việc CTV tự nhớ và tự nhóm các lỗi tương tự.|CTV và học sinh trong lớp|20 phút/lớp|
6|AI có thể tốt hơn	|Khi học sinh đặt câu hỏi, CTV mất thời gian tìm lại đúng bài giảng, ví dụ hoặc quy định liên quan trong LMS trước khi trả lời.|CTV và học sinh đang chờ hỗ trợ|25 phút/lớp|
7|Pain từ người khác|Phụ huynh và quản lý lớp khó nắm nhanh tình trạng học sinh vì thông tin nằm rải rác và cách phản hồi giữa các lớp không đồng nhất.|Phụ huynh, quản lý lớp và CTV|50% số học sinh/lớp; 30 phút/lần|

> Gợi ý tự soi: tuần trước mất nhiều thời gian nhất vào việc gì? Việc gì hay trì hoãn? Người khác hay hỏi lại câu gì? Workflow nào ai cũng biết là chậm?

**AI đã dùng ở Phase 1 (nếu có):**
- Prompt đã hỏi:
[Tôi là [ctv dạy lập trình online code Python] trong [công ty giáo dục trực tuyến X]. Công việc hằng tuần gồm: [đọc các bài giảng có sẵn trên LMS, soạn giáo án theo khung, kiểm tra BTVN và quiz của học sinh, tạo lịch các buổi học cho từng lớp bằng link Zoom, mỗi buổi có 1 link (có thể tạo đồng loạt nhiều buổi theo 1 khóa, nhưng cần đổi lại lịch khi có việc đột xuất cần đổi, đánh giá học sinh trong vòng 8 giờ sau buổi học, phản hồi với PH và quản lý lớp học về tình trạng từng học sinh] 
Tôi đã nghĩ ra các vấn đề sau:
1. [soạn giáo án]
2. [nhận xét học sinh]
3. [check tiến độ bài làm của học sinh sau buổi học]
Hãy gợi ý thêm problem theo 4 lăng kính: lặp lại, tốn thời gian, AI có thể tốt hơn, pain từ người khác. Với mỗi gợi ý, ghi actor, workflow sơ bộ và cách đo. Đừng đưa ý tưởng quá rộng kiểu "xây trợ lý AI toàn năng. Chú ý đọc theo khung của file 01-worksheet.md và tham khảo mẫu 02-deliverable-example.md]
- Ý dùng được: Đổi lịch đột xuất, gom dữ liệu đánh giá và tổng hợp lỗi Python.
- Ý bỏ vì không phải pain thật: Học sinh phải tìm lịch ở nhiều kênh, vì thực tế lớp chỉ sử dụng một kênh chung.

**Self-check Phase 1:**
- [x] Đủ 5+ dòng, mỗi dòng có actor + số đo cụ thể
- [x] Dùng ít nhất 3/4 lăng kính
- [x] Không có dòng chung chung kiểu "mất nhiều thời gian"

---

## Phase 2 — Top 3 Problem Cards

### 2.1. Chọn top 3

Giữ bài nào: actor cụ thể, workflow vẽ được 3-7 bước, bottleneck ở 1 bước, impact đo được. Loại bài quá rộng.

| Rank | Problem (copy từ bảng scan) | Vì sao chọn (2-3 ý) | Điều còn chưa chắc |
|---|---|---|---|
| 1 | Đổi lịch đột xuất trên nhiều hệ thống | Workflow và bottleneck rõ; mất khoảng 15-20 phút/lần; lịch hoặc link sai có thể ảnh hưởng đồng thời đến CTV, quản lý lớp, học sinh và phụ huynh. | Chưa đo tần suất đổi lịch và số lỗi thực tế; chưa chắc AI cần thiết hay checklist, mẫu thông báo và một nguồn lịch chuẩn đã đủ. |
| 2 | Gom dữ liệu để đánh giá trong 8 giờ | Lặp lại sau mỗi buổi học; mất khoảng 5-7 phút/học sinh; có deadline 8 giờ và ảnh hưởng trực tiếp đến độ đầy đủ, đúng hạn của đánh giá. | Chưa tách được thời gian gom dữ liệu khỏi thời gian nhận định; chưa xác nhận khả năng xuất và ghép dữ liệu an toàn giữa các nguồn. |
| 3 | Tổng hợp lỗi Python phổ biến của lớp | Mất khoảng 20 phút/lớp; cần hiểu ngữ cảnh để nhóm các lỗi có cùng nguyên nhân; kết quả giúp CTV chọn đúng nội dung ôn tập cho buổi sau. | Chưa kiểm chứng độ chính xác khi AI phân nhóm lỗi; taxonomy và bảng tally cố định có thể đã giải quyết phần lớn vấn đề mà không cần AI. |


### 2.2. Problem Cards chi tiết (lặp lại cho cả 3 cards)

---

#### Problem Card #1 — Đổi lịch học đột xuất trên nhiều hệ thống

```text
Problem 1 câu:
Khi một buổi học phải đổi lịch đột xuất, CTV mất khoảng 15-20 phút để sửa thông tin
trên nhiều nơi và thông báo lại cho các bên, nhưng vẫn có nguy cơ học sinh dùng lịch
hoặc link Zoom cũ.

Actor:
CTV dạy Python online chịu trách nhiệm cập nhật lịch; học sinh, phụ huynh và quản lý
lớp là những người nhận thông tin và bị ảnh hưởng nếu lịch không đồng bộ.

Thời điểm / bối cảnh:
Khi CTV hoặc lớp có việc đột xuất và phải đổi ngày/giờ của một buổi học đã được tạo
trước trên Zoom và thông báo trên các kênh của lớp.

Current workflow 3-7 bước:
1. CTV tiếp nhận hoặc đề xuất yêu cầu đổi lịch.
2. CTV trao đổi với quản lý lớp để chốt ngày và giờ học mới.
3. CTV mở Zoom để sửa lịch hoặc tạo lại buổi học và lấy link mới.
4. CTV cập nhật lịch/link trên LMS hoặc lịch quản lý lớp.
5. CTV soạn và gửi thông báo cho học sinh, phụ huynh và quản lý lớp.
6. CTV kiểm tra phản hồi, giải đáp người còn nhầm lịch hoặc chưa nhận được link mới.

Bottleneck:
Thông tin ngày, giờ và link mới phải được nhập lại rồi đối chiếu ở nhiều nơi. Chỉ cần
bỏ sót một kênh hoặc giữ lại link cũ là các bên có thể nhận thông tin không thống nhất.

Impact:
Mỗi lần đổi lịch mất khoảng 15-20 phút thao tác thủ công. Ngoài thời gian của CTV,
việc cập nhật thiếu hoặc sai còn làm học sinh phải hỏi lại, vào nhầm giờ hoặc bỏ lỡ
buổi học; quản lý lớp phải hỗ trợ xử lý lại.

Success metric:
- Giảm thời gian xử lý một lần đổi lịch từ 15-20 phút xuống tối đa 8 phút.
- 100% nơi cần cập nhật có cùng ngày, giờ và link Zoom trước khi gửi thông báo.
- Không phát sinh trường hợp học sinh dùng lịch/link cũ do CTV cập nhật thiếu.
- Giảm số câu hỏi xác nhận lại lịch sau mỗi lần thay đổi.

Non-AI alternative:
Dùng một nguồn lịch chuẩn duy nhất, mẫu thông báo cố định và checklist các nơi cần cập
nhật. Cách này có thể giải quyết phần lớn lỗi bỏ sót mà chưa cần AI.

AI hypothesis:
Sau khi CTV nhập lịch cũ, lịch mới và link Zoom, một workflow có thể tạo checklist,
so sánh các trường thông tin và soạn thông báo phù hợp cho từng nhóm người nhận. CTV
vẫn phải kiểm tra ngày, giờ, link và tự bấm gửi.

Quick gut:
[ ] No AI / process fix
[ ] Rule
[x] Workflow
[ ] Agent
[ ] Chưa biết
```

**Draft workflow Card #1** (ASCII / Mermaid / ảnh đính kèm):

```text
CURRENT STATE — 15-20 phút

[1 Chốt giờ mới: 3']
→ [2 Sửa lịch/link Zoom: 3']
→ [3 Cập nhật LMS/lịch lớp: 4']  <-- bottleneck
→ [4 Soạn và gửi thông báo: 4']
→ [5 Kiểm tra, trả lời xác nhận: 2-6']

FUTURE STATE — mục tiêu tối đa 8 phút

[1 Nhập lịch mới một lần: 2']
→ [2 Workflow tạo checklist + draft thông báo: 1']
→ [3 CTV cập nhật hoặc xác nhận các hệ thống: 3']
→ [4 CTV kiểm tra ngày, giờ, link rồi gửi: 2']  <-- human boundary

Fallback: nếu workflow tạo sai nội dung hoặc không cập nhật được một hệ thống, CTV
dùng checklist và mẫu thông báo để cập nhật thủ công. Không gửi thông báo nếu CTV chưa
đối chiếu ngày, giờ và link Zoom với nguồn lịch chuẩn.
```

#### Problem Card #2 — Gom dữ liệu để đánh giá học sinh trong 8 giờ

```text
Problem 1 câu:
Sau mỗi buổi học, CTV mất khoảng 5-7 phút cho từng học sinh để tìm và đối chiếu dữ
liệu từ nhiều nguồn trước khi đánh giá, làm tăng nguy cơ nộp đánh giá muộn hơn thời
hạn 8 giờ hoặc bỏ sót bằng chứng quan trọng.

Actor:
CTV dạy Python online chịu trách nhiệm đánh giá học sinh sau buổi học; học sinh, phụ
huynh và quản lý lớp sử dụng kết quả này để theo dõi tình hình học tập.

Thời điểm / bối cảnh:
Ngay sau mỗi buổi học, khi CTV phải hoàn thành đánh giá cho toàn bộ học sinh trong lớp
trong vòng 8 giờ kể từ khi buổi học kết thúc.

Current workflow 3-7 bước:
1. Mở danh sách học sinh của lớp cần đánh giá.
2. Kiểm tra dữ liệu điểm danh và mức độ tham gia trong buổi học.
3. Mở LMS để kiểm tra tình trạng BTVN và kết quả quiz của từng học sinh.
4. Đối chiếu các dữ liệu trên với ghi chú quan sát trong buổi học.
5. Xác định mức độ hoàn thành, điểm mạnh và vấn đề cần theo dõi.
6. Nhập đánh giá của từng học sinh lên hệ thống và kiểm tra trước khi lưu.

Bottleneck:
CTV phải chuyển qua nhiều nguồn rồi tự ghép đúng dữ liệu với từng học sinh. Việc tìm
và đối chiếu dữ liệu ở bước 2-4 chiếm phần lớn thời gian và dễ xảy ra thiếu hoặc nhầm
thông tin khi lớp có nhiều học sinh.

Impact:
Mỗi học sinh cần khoảng 5-7 phút; tổng thời gian của một lớp bằng 5-7 phút nhân với
số học sinh cần đánh giá. Khi có nhiều lớp hoặc lịch dạy sát nhau, CTV dễ sát hoặc quá
mốc 8 giờ; đánh giá thiếu dữ liệu cũng làm phụ huynh và quản lý phải hỏi lại.

Success metric:
- Giảm thời gian gom dữ liệu và hoàn thành đánh giá từ 5-7 phút xuống tối đa 3 phút
  cho mỗi học sinh.
- 100% đánh giá được hoàn thành trong vòng 8 giờ sau buổi học.
- Không có đánh giá bị gắn nhầm dữ liệu giữa các học sinh.
- Mỗi đánh giá có đủ dữ liệu hiện có về điểm danh, BTVN/quiz và quan sát trong buổi học;
  nguồn nào chưa có phải được đánh dấu rõ thay vì tự suy đoán.

Non-AI alternative:
Dùng một bảng tổng hợp cố định theo danh sách lớp, checklist các nguồn phải kiểm tra
và mẫu đánh giá có sẵn. CTV ghi chú theo từng học sinh ngay trong buổi học để giảm thời
gian tìm lại thông tin sau buổi.

AI hypothesis:
Một workflow có thể gom dữ liệu điểm danh, BTVN, quiz và ghi chú theo đúng mã học sinh;
AI chỉ hỗ trợ tóm tắt bằng chứng và cảnh báo dữ liệu thiếu hoặc mâu thuẫn. CTV phải mở
nguồn gốc để kiểm tra, quyết định nội dung đánh giá và tự bấm lưu.

Quick gut:
[ ] No AI / process fix
[ ] Rule
[x] Workflow
[ ] Agent
[ ] Chưa biết
```

**Draft workflow Card #2:**

```text
CURRENT STATE — 5-7 phút/học sinh

[1 Mở danh sách lớp: 0,5']
→ [2 Tìm điểm danh và mức độ tham gia: 1-2']
→ [3 Kiểm tra BTVN/quiz trên LMS: 1-2']
→ [4 Đối chiếu với ghi chú buổi học: 1']  <-- bottleneck nằm ở bước 2-4
→ [5 Viết, nhập và kiểm tra đánh giá: 1-1,5']

FUTURE STATE — mục tiêu tối đa 3 phút/học sinh

[1 Workflow gom dữ liệu theo học sinh: 0,5']
→ [2 AI tóm tắt bằng chứng + đánh dấu dữ liệu thiếu: 0,5']
→ [3 CTV kiểm tra nguồn và quyết định đánh giá: 1,5']  <-- human boundary
→ [4 CTV chỉnh sửa và lưu: 0,5']

Fallback: nếu thiếu dữ liệu, ghép sai học sinh hoặc nội dung tóm tắt không khớp nguồn,
CTV bỏ bản tóm tắt và kiểm tra thủ công theo checklist. Workflow không được tự suy đoán
dữ liệu, tự chấm học sinh hoặc tự gửi đánh giá.
```

---

#### Problem Card #3 — Tổng hợp các lỗi Python phổ biến của lớp

```text
Problem 1 câu:
Sau khi kiểm tra bài làm, CTV mất khoảng 20 phút mỗi lớp để nhớ lại, ghi chép và nhóm
các lỗi Python tương tự của học sinh, nên có thể bỏ sót lỗi phổ biến hoặc chọn nội dung
ôn tập chưa đúng trọng tâm.

Actor:
CTV dạy Python online chịu trách nhiệm tổng hợp lỗi và chuẩn bị nội dung ôn tập; học
sinh trong lớp hưởng lợi khi các lỗi chung được giải thích lại ở buổi tiếp theo.

Thời điểm / bối cảnh:
Sau khi CTV đã kiểm tra BTVN và quiz của một lớp, trước khi chuẩn bị giáo án hoặc phần
ôn tập cho buổi học tiếp theo.

Current workflow 3-7 bước:
1. CTV mở lại bài làm, kết quả quiz và ghi chú khi chấm của từng học sinh.
2. Ghi ra các lỗi đã gặp, ví dụ lỗi cú pháp, kiểu dữ liệu, vòng lặp hoặc cách dùng hàm.
3. So sánh các lỗi có biểu hiện khác nhau nhưng cùng nguyên nhân kiến thức.
4. Nhóm lỗi theo chủ đề và đếm số học sinh gặp từng nhóm lỗi.
5. Xác định lỗi cần ưu tiên dựa trên tần suất và mức độ ảnh hưởng.
6. Chọn ví dụ hoặc bài luyện tập để giải thích lại trong buổi tiếp theo.

Bottleneck:
Bước 2-4 phụ thuộc vào việc CTV tự đọc lại, nhớ và chuẩn hóa mô tả lỗi. Cùng một lỗi
kiến thức có thể xuất hiện dưới nhiều dạng code hoặc đáp án khác nhau, khiến việc nhóm
thủ công mất thời gian và không nhất quán.

Impact:
CTV mất khoảng 20 phút cho mỗi lớp ngoài thời gian chấm bài. Nếu tổng hợp thiếu, phần
ôn tập có thể không tập trung vào khó khăn chung; học sinh tiếp tục lặp lại cùng loại
lỗi ở bài hoặc buổi học sau.

Success metric:
- Giảm thời gian tổng hợp lỗi từ khoảng 20 phút xuống dưới 10 phút mỗi lớp.
- Ít nhất 90% gợi ý phân nhóm của AI được CTV xác nhận là đúng sau khi đối chiếu bài gốc.
- Không bỏ sót nhóm lỗi xuất hiện ở từ 2 học sinh trở lên trong dữ liệu đã cung cấp.
- Theo dõi mức giảm số học sinh lặp lại cùng nhóm lỗi ở bài tập hoặc buổi học sau.

Non-AI alternative:
Dùng taxonomy lỗi Python cố định và bảng tally theo lớp. Khi chấm, CTV chọn mã lỗi có
sẵn cho từng học sinh; cuối buổi dùng bảng đếm để xác định các lỗi phổ biến.

AI hypothesis:
AI có thể đọc phần code, đáp án sai và ghi chú đã được ẩn danh để đề xuất nhóm lỗi,
nguyên nhân kiến thức và số trường hợp tương ứng. CTV phải đối chiếu với bài gốc, sửa
nhóm sai và quyết định nội dung nào cần đưa vào buổi ôn tập.

Quick gut:
[ ] No AI / process fix
[ ] Rule
[x] Workflow
[ ] Agent
[ ] Chưa biết
```

**Draft workflow Card #3:**

```text
CURRENT STATE — khoảng 20 phút/lớp

[1 Mở lại bài và ghi chú: 4']
→ [2 Liệt kê lỗi của từng học sinh: 6']
→ [3 So sánh và nhóm lỗi cùng nguyên nhân: 6']  <-- bottleneck
→ [4 Đếm, ưu tiên và chọn nội dung ôn tập: 4']

FUTURE STATE — mục tiêu dưới 10 phút/lớp

[1 Xuất và ẩn danh code/đáp án sai: 2']
→ [2 AI đề xuất nhóm lỗi + tần suất: 1']
→ [3 CTV đối chiếu bài gốc và sửa phân nhóm: 4']  <-- human boundary
→ [4 CTV chọn nội dung ôn tập: 2']

Fallback: nếu AI ghép sai nguyên nhân, bỏ sót lỗi hoặc giải thích không chính xác, CTV
bỏ kết quả đó và tổng hợp bằng taxonomy cùng bảng tally. Không đưa dữ liệu định danh
của học sinh vào công cụ AI và không dùng kết quả AI để tự động chấm hoặc gửi đánh giá.
```

---

### 2.3. Card muốn pitch nhất (chuẩn bị 2 phút)

**Card tôi muốn pitch nhất:**

```text
Problem Card #2 — Gom dữ liệu để đánh giá học sinh trong 8 giờ.
```

**Vì sao (2-3 câu: workflow gì, số đo gì, impact gì):**

```text
Sau mỗi buổi học, CTV phải mở và đối chiếu điểm danh, BTVN, quiz cùng ghi chú để đánh
giá từng học sinh. Workflow này lặp lại với baseline khoảng 5-7 phút/học sinh và phải
hoàn thành trong 8 giờ; mục tiêu là giảm xuống tối đa 3 phút/học sinh mà vẫn đúng người, đủ bằng chứng và không để AI tự quyết định đánh giá.
```

**Câu hỏi tôi muốn nhóm challenge (1-2 câu hỏi đúng chỗ yếu):**

```text
1. Bottleneck thực sự nằm ở việc gom dữ liệu hay ở bước CTV nhận định và viết đánh giá?
2. Các nguồn dữ liệu hiện tại có thể xuất và ghép theo mã học sinh một cách an toàn,
   chính xác không, hay giải pháp trước mắt chỉ nên là checklist và bảng tổng hợp?
```

**AI phản biện Card (nếu có):**
- Điểm yếu AI chỉ ra: Baseline 5-7 phút/học sinh mới dựa trên quan sát cá nhân; chưa
  tách thời gian gom dữ liệu khỏi thời gian nhận định. Khả năng truy cập, xuất và ghép
  dữ liệu giữa Zoom/LMS/ghi chú cũng chưa được xác nhận. Mục tiêu 100% đúng hạn chưa
  phản ánh đầy đủ chất lượng của đánh giá.
- Tôi sửa gì: Thu hẹp AI vào bước gom và tóm tắt bằng chứng; bổ sung metric không ghép
  nhầm học sinh, đủ nguồn hiện có và bắt buộc CTV kiểm tra trước khi lưu. Khi pilot sẽ
  bấm giờ riêng từng bước trong 2-3 buổi và kiểm tra khả năng xuất dữ liệu trước khi
  quyết định tự động hóa.

### Self-check nộp phần 01
- [x] Có 5+ problems + top 3 Cards đủ field
- [x] Mỗi Card có workflow trước/sau + bottleneck + metric + fallback
- [x] Đã chọn 1 card pitch + câu hỏi challenge
