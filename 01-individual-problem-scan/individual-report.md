# 01 — Individual Problem Scan

> Điền theo Phase 1 + Phase 2 trong `01-worksheet.md`. Tự scan trước, dùng AI sau để phản biện.

## Thông tin cá nhân

- **Họ và tên:** Nguyễn Thành Duy
- **Mã học viên:** 2A202602804
- **Vai trò / bối cảnh:** Sinh viên năm cuối Học viện Công nghệ Bưu chính Viễn thông
- **Công việc hằng tuần:**
  1. Học tập và làm đồ án
  2. Làm các task ở công ty đang thực tập

---

## Phase 1 — Scan 5+ problems (Tối thiểu 5 bài toán)

### Tóm tắt 5 bài toán đã hoàn thiện (Đủ 4 lăng kính & Định lượng số liệu)

| # | Lăng kính | Problem quan sát được | Ai chịu ảnh hưởng? | Dấu hiệu thật (số + bằng chứng) |
|---|---|---|---|---|
| 1 | **Lặp lại** | Khách quên đồ trên xe taxi Xanh SM; CSKH phải đối chiếu biển số, liên hệ tài xế qua tổng đài để xin liên lạc | Hành khách, Tài xế, CSKH | Gặp 15-20 ca/ngày; mất trung bình 25 phút/ca gọi tới gọi lui qua lại |
| 2  | **Tốn thời gian** | Tổng hợp báo cáo phân tích nguyên nhân hủy cuốc (Top cancellation reasons) vào cuối tuần từ file CSV hàng chục nghìn dòng | Trưởng ca CSKH, Vận hành | Mất 120 phút mỗi chiều thứ 6 để lọc pivot table, phân loại lý do định tính |
| 3 | **Pain từ người khác** | Tài xế phàn nàn trụ sạc VinFast/V-GREEN hiển thị "khả dụng" trên app nhưng tới nơi thì lỗi kết nối hoặc đã có xe cắm sạc đầy nhưng chưa rút | Tài xế Xanh SM, Đội vận hành trạm sạc | Nhóm Zalo/Facebook tài xế kêu ca liên tục; mất 30-45 phút tìm trạm sạc khác trong giờ cao điểm |
| 4  | **AI có thể tốt hơn** | Phân loại mức độ khẩn cấp (Urgency) và cảm xúc tiêu cực của ticket khiếu nại gửi qua app Xanh SM (ticket đe dọa, tai nạn bị lẫn với hỏi mã giảm giá/voucher) | CSKH ca trực, Khách hàng gặp sự cố | 300+ ticket/ngày; ticket nghiêm trọng bị xử lý trễ > 4 tiếng do xếp hàng tuần tự (FIFO); rủi ro khủng hoảng truyền thông |
| 5 | **Lặp lại** | Xử lý khiếu nại tranh chấp cước phí do lệch định vị GPS đón/trả hoặc cuốc xe tính sai phụ phí giờ cao điểm/cầu đường | Hành khách, CSKH, Kế toán đối soát | 25-30 ticket/ngày; CSKH mất 15-20 phút/ticket mở map đối chiếu tuyến đường thực tế với lộ trình hệ thống đề xuất |

**AI đã dùng ở Phase 1:**
- **Prompt đã hỏi:** "Tôi là Chuyên viên Vận hành CSKH tại taxi Xanh SM. Hãy gợi ý thêm các bài toán theo 4 lăng kính: Lặp lại, Tốn thời gian, AI có thể tốt hơn, Pain từ người khác dựa trên các khâu tiếp nhận ticket, hỗ trợ tài xế sạc xe và báo cáo hủy chuyến."
- **Ý dùng được:** Gợi ý bài toán phân loại mức độ khẩn cấp của ticket khiếu nại (Urgency detection) bằng NLP và bài toán đối soát lệch cước phí do GPS.
- **Ý bỏ vì không phải pain thật:** Ý tưởng "xây dựng chatbot tự động lái xe điều phối tới điểm sạc" và "AI tự phạt tiền tài xế khi khách phàn nàn" vì quá viển vông, vi phạm quy định pháp lý và quy chế nội bộ của công ty.

**Self-check Phase 1:**
- [x] Đủ 5+ dòng, mỗi dòng có actor + số đo cụ thể
- [x] Dùng ít nhất 3/4 lăng kính (Đã dùng đủ cả 4 lăng kính)
- [x] Không có dòng chung chung kiểu "mất nhiều thời gian"

---

## Phase 2 — Top 3 Problem Cards

### 2.1. Chọn top 3

| Rank | Problem (copy từ bảng scan) | Vì sao chọn (2-3 ý) | Điều còn chưa chắc |
|---|---|---|---|
| 1 | Khách quên đồ trên xe taxi Xanh SM; CSKH phải đối chiếu biển số, liên hệ tài xế qua tổng đài để xin liên lạc | 1. Tần suất cao hàng ngày (15-20 ca/ngày).<br>2. Workflow rõ ràng, điểm nghẽn nhận diện đồ vật và kết nối tài xế rất tốn công.<br>3. Tác động trực tiếp đến sự hài lòng của khách hàng (CSAT). | Khả năng tài xế đang chở khách khác không tiện kiểm tra ghế sau ngay lập tức. |
| 2 | Tổng hợp báo cáo phân tích nguyên nhân hủy cuốc (Top cancellation reasons) vào cuối tuần từ file CSV hàng chục nghìn dòng | 1. Tốn thời gian lớn cố định (120 phút/tuần).<br>2. Dữ liệu định tính (lý do hủy tài xế/khách gõ tay) rất hợp với AI tóm tắt, gom cụm (clustering).<br>3. Đầu ra báo cáo phục vụ trực tiếp cho quyết định vận hành. | Độ chính xác của AI khi phân loại lý do hủy bằng tiếng lóng hoặc viết tắt của tài xế. |
| 3 | Phân loại mức độ khẩn cấp (Urgency) và cảm xúc tiêu cực của ticket khiếu nại gửi qua app Xanh SM | 1. Giảm thiểu rủi ro khủng hoảng truyền thông trên mạng xã hội.<br>2. AI thế mạnh về xử lý ngôn ngữ tự nhiên (sentiment analysis).<br>3. Metric đo lường rõ: thời gian phản hồi đầu tiên (First Response Time). | Cần tích hợp vào phần mềm Helpdesk/CRM hiện có của công ty. |

---

### 2.2. Problem Cards chi tiết

#### Problem Card #1 — Hỗ trợ kết nối tìm đồ thất lạc trên xe Xanh SM

```text
Problem 1 câu:
Khách hàng quên đồ trên taxi Xanh SM mất trung bình 25 phút để xác minh và liên hệ với tài xế do CSKH phải tra cứu cuốc thủ công và làm cầu nối gọi điện qua lại nhiều lần.

Actor:
Hành khách để quên đồ, Tài xế Xanh SM, Chuyên viên CSKH trực tổng đài.

Thời điểm / bối cảnh:
Ngay sau khi kết thúc chuyến đi, khách phát hiện bỏ quên tài sản (điện thoại, ví, chìa khóa, túi xách) trên xe.

Current workflow 3-7 bước:
1. Khách gọi tổng đài hoặc gửi yêu cầu hỗ trợ "Quên đồ" qua app Xanh SM (3 phút)
2. CSKH nhận ticket, tra cứu số điện thoại khách trên CRM để tìm mã cuốc xe và thông tin tài xế gần nhất (5 phút)
3. CSKH gọi điện cho tài xế để mô tả đặc điểm đồ vật và hỏi tài xế kiểm tra xe (7 phút)  <-- BOTTLENECK
4. Nếu tài xế xác nhận thấy đồ, CSKH tạo cuộc gọi ghép 3 bên hoặc xin ý kiến khách để kết nối tài xế đem đồ trả lại (7 phút)
5. CSKH ghi nhận kết quả và đóng ticket trên hệ thống (3 phút)

Bottleneck:
Bước 3 và 4 — CSKH làm trung gian truyền đạt mô tả đồ vật qua điện thoại, gọi nhiều cuộc vì tài xế đang di chuyển hoặc khách mô tả không rõ ràng (mất 14/25 phút).

Impact:
15-20 ca/ngày x 25 phút = 375-500 phút (hơn 6-8 giờ làm việc của 1 nhân sự CSKH/ngày). Khách sốt ruột, lo mất tài sản, đánh giá 1 sao trên app.

Success metric:
Giảm thời gian xử lý ban đầu từ 25 phút xuống dưới 5 phút; tăng tỷ lệ kết nối thành công tài xế - hành khách trong vòng 10 phút đầu tiên lên 85%.

Non-AI alternative:
Tạo tính năng bấm nút "Gọi bảo mật cho tài xế chuyến vừa đi" trong vòng 2 tiếng sau cuốc xe (Masked Calling). Tuy nhiên cách này không có biên bản lưu trữ bằng chứng hình ảnh đồ vật để bảo vệ tài xế tránh bị vu oan đánh tráo đồ.

AI hypothesis:
Khách chụp ảnh/mô tả đồ quên qua app, AI tự động trích xuất đặc điểm đồ vật, match ngay với chuyến xe vừa đi và gửi thông báo đẩy (push notification) kèm ảnh mô phỏng vào app tài xế: "Có phải đồ này ở ghế sau không? Bấm xác nhận Có/Không".

Quick gut:
[x] Workflow
```

**Draft workflow Card #1:**

```text
CURRENT STATE — 25 phút
[1 Khách gọi: 3'] → [2 CSKH tra cuốc: 5'] → [3 CSKH gọi tài xế hỏi đồ: 7'] (Bottleneck) → [4 Ghép nối liên lạc: 7'] → [5 Đóng ticket: 3']

FUTURE STATE — 4 phút
[1 Khách báo đồ quên trên app + chụp/mô tả: 1'] 
→ [2 Hệ thống tự map mã cuốc & AI chuẩn hóa thông tin đồ vật: 30s (Rule + AI)] 
→ [3 Push thông báo xác nhận vào app tài xế: 1'] 
→ [4 CSKH review xác nhận & kích hoạt kênh liên lạc an toàn: 1.5' (Human boundary)]

Fallback: Nếu tài xế không phản hồi app trong 5 phút hoặc không tìm thấy, hệ thống tự động chuyển ticket sang cho CSKH gọi điện trực tiếp theo quy trình cũ.
```

---

#### Problem Card #2 — Phân tích nguyên nhân hủy cuốc từ dữ liệu định tính

```text
Problem 1 câu:
Trưởng ca CSKH Xanh SM mất 120 phút mỗi chiều thứ Sáu để đọc và phân loại thủ công hàng nghìn dòng lý do hủy cuốc dạng text tự do do khách và tài xế nhập trên app để làm báo cáo tuần.

Actor:
Trưởng ca CSKH, Chuyên viên Vận hành Xanh SM.

Thời điểm / bối cảnh:
Chiều thứ Sáu hàng tuần trước buổi họp giao ban vận hành định kỳ với Giám đốc Vận hành.

Current workflow 3-7 bước:
1. Export file CSV dữ liệu chuyến bị hủy trong tuần từ database (10 phút)
2. Mở Excel, chạy pivot table lọc các lý do hủy chọn sẵn (system reason) (15 phút)
3. Đọc và phân loại thủ công cột "Lý do khác" (text tự do của tài xế và khách gõ) vào các nhóm nguyên nhân chính (60 phút)  <-- BOTTLENECK
4. Tính tỷ lệ % của từng nhóm nguyên nhân (xe đến chậm, khách đổi ý, kẹt xe, trạm sạc quá tải) (15 phút)
5. Viết phần nhận định/insight và hoàn thiện slide báo cáo tuần (20 phút)

Bottleneck:
Bước 3 — Đọc hàng nghìn dòng text gõ tay, viết tắt, không dấu, tiếng lóng để gom nhóm thủ công mất 60 phút và dễ nhầm lẫn.

Impact:
Mất 120 phút/tuần của quản lý ca; báo cáo dễ bị trễ giờ họp giao ban; các nguyên nhân hệ thống như "trạm sạc hết chỗ" bị bỏ sót trong đống text không có cấu trúc.

Success metric:
Giảm thời gian tổng hợp báo cáo từ 120 phút xuống dưới 20 phút; phân loại chính xác 100% các dòng text tự do vào đúng cụm nguyên nhân.

Non-AI alternative:
Bỏ ô nhập text tự do, bắt buộc khách/tài xế chỉ được chọn lý do có sẵn (Drop-down list). Nhược điểm: Người dùng sẽ chọn bừa lý do đầu tiên để thoát app nhanh, làm sai lệch hoàn toàn dữ liệu vận hành thực tế.

AI hypothesis:
AI tự động đọc cột text tự do, phân tích ngữ nghĩa, tự động gom cụm (semantic clustering) thành các nhóm nguyên nhân gốc rễ và trích xuất tỷ lệ phần trăm cùng các câu trích dẫn tiêu biểu.

Quick gut:
[x] Workflow
```

**Draft workflow Card #2:**

```text
CURRENT STATE — 120 phút
[1 Export CSV: 10'] → [2 Pivot Excel: 15'] → [3 Đọc & phân loại tay text tự do: 60'] (Bottleneck) → [4 Tính tỷ lệ: 15'] → [5 Viết nhận định: 20']

FUTURE STATE — 18 phút
[1 Script auto-export data: 2' (Rule)] 
→ [2 AI phân loại & gom cụm text lý do hủy: 3' (AI)] 
→ [3 AI draft biểu đồ & gạch đầu dòng insight nổi cộm: 3' (AI)] 
→ [4 Quản lý ca review số liệu, chỉnh sửa nhận định: 10' (Human boundary)]

Fallback: Nếu AI phân loại sai nhóm (>10% lỗi), người dùng nhấn nút xuất danh sách các dòng nghi vấn để kiểm tra lại bằng bộ lọc Excel thủ công.
```

---

#### Problem Card #3 — Cảnh báo và điều hướng sự cố trụ sạc VinFast/V-GREEN hiển thị khả dụng ảo

```text
Problem 1 câu:
Tài xế taxi điện Xanh SM mất 30–45 phút giờ cao điểm tìm và di chuyển tới trạm sạc khác vì app hiển thị trụ sạc VinFast/V-GREEN đang "khả dụng" nhưng thực tế trụ bị lỗi kết nối hoặc đã có xe cắm sạc đầy nhưng chưa rút.

Actor:
Tài xế Xanh SM, Đội vận hành trạm sạc V-GREEN / VinFast, Khách hàng đặt xe giờ cao điểm (chịu ảnh hưởng gián tiếp).

Thời điểm / bối cảnh:
Khung giờ cao điểm trưa (11h30 - 13h30) và chiều tối (17h30 - 19h30), khi mức pin xe taxi điện xuống dưới 20% cần sạc nhanh để tiếp tục đón khách.

Current workflow 3-7 bước:
1. Tài xế mở app Xanh SM Driver / VinFast tra cứu trạm sạc gần nhất hiển thị trạng thái "Khả dụng" (2 phút)
2. Lái xe 10-15 phút đến trạm sạc theo định vị bản đồ (15 phút)
3. Đến nơi phát hiện súng sạc báo lỗi đèn đỏ (lỗi kết nối) hoặc xe khác sạc đầy 100% nhưng chủ xe chưa rút súng để rời đi (5 phút)  <-- BOTTLENECK
4. Tài xế gọi hotline hỗ trợ V-GREEN hoặc nhắn lên nhóm Zalo điều phối khu vực để báo sự cố (7 phút)
5. Tài xế mở lại app, tìm trạm sạc dự phòng thứ 2 cách đó 3-5 km và tiếp tục di chuyển (18 phút)

Bottleneck:
Bước 3 — Trạng thái trụ sạc trên app bị "mù" dữ liệu thực địa (app chỉ ghi nhận tín hiệu online về điện lưới, nhưng không nhận diện được lỗi súng sạc cơ học hoặc xe đỗ chiếm chỗ sau khi sạc đầy), khiến tài xế mất trắng 30-45 phút vô ích.

Impact:
Mỗi ngày hàng trăm tài xế mất 40-45 phút không thể đón khách (thất thoát doanh thu 100.000đ - 150.000đ/tài xế/ca); đội xe bị thiếu hụt nghiêm trọng trong giờ cao điểm làm tỷ lệ hủy cuốc của khách tăng 15-20%.

Success metric:
Giảm tỷ lệ tài xế gặp sự cố "hớ trạm sạc" từ 25% xuống dưới 5%; giảm thời gian tìm và tiếp cận trạm sạc khả dụng thực tế từ 45 phút xuống dưới 15 phút.

Non-AI alternative:
- Áp dụng phí phạt đỗ xe quá giờ sau khi sạc đầy (Idle Fee) bằng quy tắc cứng.
- Cắt cử nhân viên điều phối/bảo vệ đứng trực tại từng trạm sạc lớn (Chi phí nhân sự rất cao, không thể phủ sóng hàng nghìn trạm sạc toàn quốc).

AI hypothesis:
AI phân tích dữ liệu telemetry từ xe (nếu pin 100% quá 15 phút hoặc có 2 tài xế liên tiếp cắm sạc thất bại trong 3 phút) kết hợp camera giám sát trạm: tự động gắn nhãn "Nghi ngờ lỗi / Bị chiếm chỗ" trên app, đồng thời thuật toán tự động gợi ý và giữ chỗ sạc tại trạm khả dụng thực tế gần nhất cho tài xế.

Quick gut:
[x] Workflow
```

**Draft workflow Card #3:**

```text
CURRENT STATE — 47 phút
[1 Tìm trạm trên app: 2'] → [2 Lái xe đến trạm: 15'] → [3 Phát hiện trụ hỏng/chiếm chỗ: 5'] (Bottleneck) → [4 Báo hotline/Zalo: 7'] → [5 Tìm & lái sang trạm khác: 18']

FUTURE STATE — 14 phút
[1 AI/Telemetry phân tích realtime: tự động gắn nhãn "Trụ nghi ngờ lỗi/Chiếm chỗ": 30s (AI + Rule)] 
→ [2 App tự động gợi ý trạm sạc khả dụng thực tế gần nhất & giữ slot 15': 1'] 
→ [3 Tài xế lái thẳng đến trạm dự phòng có chỗ trống: 11'] 
→ [4 Cắm sạc thành công & xác nhận trên app: 1.5' (Human boundary: tài xế xác nhận)]

Fallback: Nếu hệ thống dự đoán sai hoặc mất kết nối mạng, tài xế có thể bấm nút "Báo cáo thực địa thủ công" để cộng đồng tài xế cùng cập nhật và hệ thống tự động hoàn điểm thưởng hỗ trợ.
```


---

### 2.3. Card muốn pitch nhất (Chuẩn bị 2 phút)

**Card tôi muốn pitch nhất:**
> **Problem Card #1: Hỗ trợ kết nối tìm đồ thất lạc trên xe Xanh SM.**

**Vì sao (2-3 câu: workflow gì, số đo gì, impact gì):**
- **Workflow cực kỳ chuẩn xác:** Đi từ lúc khách nhận ra quên đồ → đối chiếu cuốc xe → kết nối tài xế → trả đồ an toàn.
- **Số đo rõ ràng và thuyết phục:** Xảy ra 15-20 lần/ngày; hiện tại mất 25 phút/ca gọi qua gọi lại; kỳ vọng giảm xuống dưới 5 phút.
- **Impact thiết thực:** Giải phóng hơn 6 giờ lao động thủ công mỗi ngày cho tổ trực CSKH và nâng cao trực tiếp chỉ số hài lòng khách hàng (CSAT) của Xanh SM.

**Câu hỏi tôi muốn nhóm challenge (1-2 câu hỏi đúng chỗ yếu):**
1. *Nếu tài xế đang chở cuốc tiếp theo trên đường cao tốc và không thể nhìn màn hình điện thoại để bấm xác nhận, workflow sẽ xử lý thế nào để không làm gián đoạn việc lái xe an toàn?*
2. *Làm thế nào để bảo mật thông tin số điện thoại của hành khách và tài xế trong suốt quá trình trả đồ thất lạc?*

**AI phản biện Card (nếu có):**
- **Điểm yếu AI chỉ ra:** Đề xuất ban đầu định để AI tự động cung cấp số điện thoại tài xế cho khách hàng gọi trực tiếp, điều này vi phạm nghiêm trọng chính sách bảo mật dữ liệu cá nhân của Vingroup/Xanh SM và dễ gây xung đột giữa khách và tài xế.
- **Tôi sửa gì:** Đổi sang cơ chế thông báo xác nhận nội bộ trong app tài xế và gọi qua số tổng đài ảo bảo mật (Masked Call) có sự phê duyệt của CSKH (*Human boundary*).

---

### Self-check nộp phần 01
- [x] Có 5+ problems + top 3 Cards đủ field
- [x] Mỗi Card có workflow trước/sau + bottleneck + metric + fallback
- [x] Đã chọn 1 card pitch + câu hỏi challenge
