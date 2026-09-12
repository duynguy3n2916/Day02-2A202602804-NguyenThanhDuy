# 03 — Individual Reflection

> Viết bằng lời của bạn (Phase 7 trong `01-worksheet.md`). Có thể dùng AI gợi ý câu hỏi tự soi, không dùng AI viết thay. 8-12 câu, có chuyện cụ thể.

## Thông tin cá nhân

- Họ và tên: Nguyễn Thành Duy
- Mã học viên: 2A202602804
- Nhóm: ZONE B - Công ty TNHH 1 mình tôi
- Candidate problem nhóm chọn: Sinh viên sử dụng Discord cho việc học phải dành khoảng 20-30 phút mỗi ngày để đọc và
lọc nhiều channel nhằm tìm task, assignment, deadline hoặc thay đổi lịch, nhưng vẫn có
nguy cơ bỏ sót thông tin cần hành động.


---

## 1. Tôi đã tham gia vào phần nào?

Ghi việc cụ thể + kết quả cụ thể. Không ghi chung chung kiểu "tham gia thảo luận".

| Hoạt động | Tôi đã làm gì? (việc cụ thể) | Kết quả / ảnh hưởng tới nhóm |
|---|---|---|
| Scan cá nhân | Chuẩn bị 5 bài toán vận hành Xanh SM và 3 Problem Cards nộp vào danh sách nhóm. | Đóng góp 3 bài toán (#7, #8, #9) vào pool 18 candidate chung. |
| Pitch Problem Card | Pitch 2 bài toán về xử lý khiếu nại taxi (#7) và phân tích hủy cuốc (#8). | Giúp nhóm có thêm góc nhìn thực tế về bài toán dữ liệu doanh nghiệp. |
| Challenge bài của bạn khác | Phản biện bài #18 của Vũ Anh về việc API LMS đóng kín và quyền riêng tư email. | Nhóm đồng ý thu hẹp phạm vi, chỉ tập trung vào channel Discord học tập. |
| Gom trùng / cluster | Điều phối nhóm gom 18 bài vào 4 cụm; xếp bài taxi/trạm sạc vào cụm D để loại. | Nhóm thống nhất nhanh cấu trúc 4 cụm và loại bớt các bài không khả thi. |
| Chọn candidate problem | Cùng nhóm chấm điểm ma trận và thống nhất chọn bài #18 của Vũ Anh. | Nhóm đạt đồng thuận cao (34/35 điểm), tập trung vào bài toán sát sườn. |
| Validation / research | Hoàng và Đạt phụ trách chính; tôi hỗ trợ phỏng vấn 1 bạn và chạy survey 8 sinh viên. | Bổ sung dữ liệu thực tế về pain point đọc tin nhắn cho nhóm. |
| Workflow nhóm | Việt Anh dựng workflow; tôi góp ý chèn bước Human Confirm và cơ chế Fallback. | Đảm bảo an toàn, không để AI tự ý ghi đè vào lịch học của sinh viên. |
| Problem Statement | Vũ Anh chấp bút; tôi rà soát, đồng bộ và chốt các chỉ số Success Metric. | Thống nhất bộ số đo cụ thể (recall ≥90%, FP ≤2/ngày/người) trong PS v1. |
| Rule / Workflow / Agent | Cùng nhóm thảo luận, phản biện đề xuất làm Agent tự động để chốt mức Workflow. | Giúp nhóm chọn đúng mức giải pháp vừa sức, tránh ảo giác và spam. |
| Decision | Điều phối nhóm trả lời 6 câu hỏi checklist để chốt quyết định cuối cùng. | Nhóm thống nhất Go cho pilot nhỏ 100 tin nhắn và Not Yet cho production. |

**Dấu tay rõ nhất của tôi trong artifact cuối (1-2 câu):**

```text
Tôi điều phối nhóm thu hẹp bài toán về riêng Discord học tập, đồng thời kiên quyết giữ chốt chặn sinh viên phải ấn Confirm trước khi ghi vào lịch thật.
```

---

## 2. Bảng dùng AI (mỗi dòng 1 phase có dùng AI — 2 cột cuối bắt buộc)

| Phase | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai / hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| Scan | Brainstorm các điểm nghẽn vận hành thực tế tại bộ phận Chăm sóc khách hàng & Vận hành Xanh SM. | Gợi ý nhanh các mảng công việc như đối soát hành lý thất lạc, phân loại đánh giá tài xế, quản lý trụ sạc xe điện. | Đề xuất giải pháp mang tính chung chung, dùng AI Agent tự động xử lý mọi thứ mà bỏ qua quy trình bảo mật và dữ liệu nhạy cảm. | Tự cắt nhỏ thành 5 quy trình nghiệp vụ hẹp, gắn rõ role Executive, thời gian xử lý thủ công (15-20 phút/ticket) và rủi ro thực tế. |
| Problem Card | Cấu trúc hóa 3 Problem Card theo đúng khung: Actor, Current, Desired, Metric, Skeptical. | Tạo form trình bày chuẩn chỉnh, giúp diễn đạt trôi chảy phần Current vs Desired State. | Metric AI đưa ra rất sáo rỗng kiểu "tăng 50% hiệu suất", "nâng cao trải nghiệm khách hàng", không có cách đo. | Tự đặt lại metric đo lường: thời gian xử lý khiếu nại (giảm từ 45' xuống 15'), tỷ lệ hủy cuốc giờ cao điểm, kèm câu hỏi phản biện gắt về tính khả thi. |
| Workflow | Sinh các bước xử lý message từ Discord sang Google Calendar theo luồng tự động. | Vẽ sơ đồ luồng dữ liệu (Mermaid) và liệt kê tương đối đầy đủ các thực thể (Message, Task, Deadline). | AI vẽ workflow kiểu "Black-box AI": tin nhắn vào -> AI xử lý tất cả -> tự động add thẳng vào Google Calendar mà không có bước kiểm duyệt. | Chèn thêm 2 bước kiểm soát chặt chẽ: Rule lọc keyword/announcement trước AI, và sinh viên bắt buộc review (Confirm/Edit/Ignore) trước khi ghi lịch. |
| Research | Tìm kiếm các giải pháp, extension hoặc bot Discord đang có trên thị trường để quản lý task/deadline. | Tìm ra các case điển hình như Todoist Discord integration, Zapier Webhook, Motion AI. | AI đưa ra một số link bị ảo (404/hallucinated URL) và khen ngợi công cụ một chiều mà không chỉ ra điểm yếu. | Tự vào website chính thức kiểm tra link thực tế, phân tích rõ khoảng trống: Todoist/Zapier chỉ nhận lệnh slash command gõ sẵn chứ không hiểu ngữ cảnh chat tự do. |
| Problem Statement | Gợi ý câu từ để viết gọn các field Actor, Impact, Boundary trong Problem Statement v0 và v1. | Giúp câu văn gãy gọn, đúng cấu trúc bảng yêu cầu của worksheet. | AI viết Boundary rất mơ hồ ("hạn chế thông tin không liên quan"), không nêu rõ những gì hệ thống KHÔNG ĐƯỢC LÀM. | Viết lại Boundary dứt khoát: KHÔNG đọc tin nhắn riêng (DM), KHÔNG kết nối LMS/email, KHÔNG tự ý tạo/sửa lịch nếu chưa có thao tác Confirm của sinh viên. |
| Rule / Workflow / Agent | Lập luận so sánh giữa Rule-based, Workflow kết hợp AI và Autonomous Agent. | Liệt kê các tiêu chí so sánh về chi phí, độ phức tạp, rủi ro và khả năng kiểm soát. | AI thiên vị Agent, cổ vũ việc tạo Agent tự động giao tiếp với các bạn trong nhóm học tập. | Bác bỏ Agent vì rủi ro đạo văn, hallucination và spam thông báo; chọn Workflow vì các bước xử lý đã cố định, AI chỉ cần hỗ trợ extract text. |
| Decision | Lên khung checklist 6 câu hỏi cho quyết định Go / Not Yet / No-Go và kế hoạch pilot nhỏ nhất. | Cung cấp dàn ý câu hỏi phản biện tốt về baseline, dữ liệu và hậu quả khi AI gặp lỗi. | AI kết luận vội vã là "Go toàn diện" mà quên mất nhóm chưa có baseline dữ liệu đo lường thực tế trên nhiều tuần. | Điều chỉnh quyết định thành "Go cho pilot bán thủ công 100 tin nhắn, Not Yet cho production bot", kèm tiêu chí rollback cụ thể. |

> Nếu phase nào không dùng AI, ghi `Không dùng` và vì sao tự làm.

---

## 3. Reflection câu hỏi mở

Chọn 3-4 câu trong 6 câu dưới để viết thành đoạn 8-12 câu (không trả lời bullet 1 dòng):
- Tôi học được gì khi nghe top 3 problems của các bạn khác?
- Nhóm có lúc nào bị solution-first, đòi làm Agent cho ngầu không?
- Tôi có thay đổi ý kiến sau khi bị challenge không, vì sao đổi?
- Tôi đóng góp gì thật sự vào artifact cuối, phần nào có dấu tay của tôi?
- Điều khó nhất khi viết Problem Statement là gì, metric hay boundary?
- Nếu làm lại, tôi sẽ challenge nhóm mạnh hơn ở điểm nào?

**Reflection:**

```text
Trong suốt buổi thảo luận, nhóm tôi không ít lần bị cuốn vào bẫy 'solution-first' khi một số bạn hào hứng đề xuất dựng hẳn một multi-agent system có khả năng tự trò chuyện trong Discord, tự phân công công việc và tự đồng bộ lịch. Lúc đó tôi phải kéo nhóm lại bằng câu hỏi: 'Nếu bot hiểu nhầm câu đùa thành deadline gấp rồi spam thông báo cho cả lớp lúc nửa đêm thì ai chịu trách nhiệm?'. Bản thân tôi ban đầu cũng rất tâm đắc với bài toán phân tích tỷ lệ tài xế hủy cuốc tại Xanh SM vì đã có sẵn góc nhìn nghiệp vụ thực tế. Tuy nhiên, khi bị các bạn chất vấn về việc không thể chia sẻ dữ liệu log nội bộ và bài toán quá xa vời với thời lượng lab 4 tiếng, tôi nhận ra mình đang quá bảo thủ với bài toán của riêng mình nên đã chủ động đổi phiếu sang bài toán Discord của bạn Vũ Anh. Dấu ấn rõ nét nhất của tôi trong báo cáo cuối cùng chính là việc kiên quyết siết chặt Boundary và thiết kế cơ chế 'Human Confirm' ở bước cuối, không để AI can thiệp trực tiếp vào lịch học của sinh viên. Qua bài lab này, tôi thấy phần khó nhất khi viết Problem Statement chính là xác định Metric chứ không phải Boundary. Để tìm ra một bộ chỉ số vừa phản ánh đúng chất lượng trích xuất (recall ≥90%), vừa lượng hóa được sự khó chịu của người dùng qua số lượng cảnh báo sai (false positive ≤2/ngày/người) đòi hỏi nhóm phải phỏng vấn và chạy thử nghiệm trên dữ liệu thật. Nếu được làm lại từ đầu, tôi sẽ thúc đẩy nhóm thu thập sẵn một tập dữ liệu chat thực tế từ tuần trước thay vì chỉ dựa vào ước lượng thời gian 20-30 phút/ngày, giúp nhóm có một baseline vững chắc hơn để tự tin ra quyết định Go hay Not Yet.
```

---

## 4. Tự kiểm cuối bài (check trước khi nộp repo)

- [x] [12đ] Cá nhân có 5+ problems + top 3 Problem Cards
- [x] [12đ] Tôi đã pitch rõ + challenge nhóm đúng trọng tâm (ghi ở bảng mục 1)
- [x] Nhóm có nhật ký hội tụ từ candidates về 1 bài
- [x] [15đ] Nhóm có workflow trước/sau
- [x] [20đ] Nhóm có PS v0/v1 với metric + boundary rõ
- [x] [15đ] Nhóm có so sánh No AI / Rule / Workflow / Agent
- [x] [10đ] Nhóm có Go / Not Yet / No-Go + lý do rõ
- [x] [10đ] Reflection này có vai trò thật + AI giúp/sai ở đâu + điều học được + nếu làm lại đổi gì
- [x] [6đ] Tôi tự giải thích được mạch problem → workflow → metric → boundary → độ phù hợp AI

