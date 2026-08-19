# Track 1 — Day 18 — Multiple Prototypes - Human–AI design

## 1. Thông tin cá nhân và nhóm

| | |
|---|---|
| MHV | 2A202601742 |
| Họ và tên | Nguyễn Vũ Việt Anh |
| Tên nhóm | Anh Trai Mâm Hai |
| Case đã chọn | Case C — AI Support Radar |

**Thành viên nhóm:**

| Họ và tên | Mã học viên | Vai trò |
|---|---|---|
| Nguyễn Vũ Việt Anh | 2A202601742 | Human–AI decisions |
| Nguyễn Đình Quốc | 2A202601935 | Shared context/content |
| Mai Tiến Mạnh | 2A202601922 | Facilitation |
| Nguyễn Đức Anh | 2A202601870 | Tổng hợp feedback |

---

## 2. Hypothesis Problem (Day 18)

> Khi phụ trách nhiều học viên cùng lúc, instructor khó nhận ra kịp thời ai đang gặp khó và ở đâu, vì thiếu công cụ/thời gian rà soát tín hiệu từng người, dẫn đến **can thiệp trễ hoặc bỏ sót** — học viên gặp khó âm thầm cho đến khi hậu quả xảy ra như rớt bài hoặc bỏ học.

**Chuỗi logic hỗ trợ giả thuyết:**
1. Instructor phụ trách nhiều học viên cùng lúc.
2. Instructor không đủ thời gian để rà soát thủ công tín hiệu của từng người.
3. Vì vậy instructor khó phát hiện sớm ai đang gặp khó và gặp khó ở đâu.
4. Việc phát hiện muộn dẫn đến can thiệp trễ hoặc bỏ sót.
5. Nếu instructor được hỗ trợ nhận biết và ưu tiên đúng người, khả năng can thiệp sớm sẽ tăng.

**Điều có thể bác bỏ Problem Hypothesis:**
- Instructor thực tế đã biết rõ ai đang gặp khó nhưng vẫn không can thiệp được.
- Nguyên nhân chính không phải thiếu khả năng nhận biết mà là thiếu thời gian, quyền hạn hoặc nguồn lực để hỗ trợ.
- Các tín hiệu học tập không đủ đáng tin để xác định học viên đang gặp khó.
- Instructor không xem việc phát hiện sớm học viên gặp khó là vấn đề quan trọng.
- Việc biết ai gặp khó không làm thay đổi thời điểm hoặc chất lượng can thiệp.

> Điểm bác bỏ quan trọng: Nếu instructor đã biết "ai cần hỗ trợ và ở đâu" nhưng vẫn không can thiệp sớm hơn, bottleneck có thể không nằm ở khả năng nhận biết/prioritize mà nằm ở workload, communication cost hoặc intervention workflow.

**Capability trung tính (đã gỡ khỏi hình thức cụ thể):**

> Cho phép instructor nhận biết sớm học viên nào đang gặp khó, vấn đề nằm ở đâu và ai cần được ưu tiên hỗ trợ trước.

Không phụ thuộc vào: tên màn hình, dashboard, heatmap, nút "Chưa hiểu", AI Chat, một loại dữ liệu cụ thể, hay một cách hiển thị cụ thể.

---

## 3. Three Solution Options

| Option | Tên | Cơ chế chính | Link prototype |
|--------|-----|--------------|-----------------|
| **A** | Prioritized Support Radar | AI tổng hợp tín hiệu học tập của nhiều học viên → tạo danh sách ưu tiên để instructor **chủ động** rà soát (pull model: Human scans → AI prioritizes → Human decides) | [ai-support-radar.onrender.com](https://ai-support-radar.onrender.com/) (tab Option A) |
| **B** | Proactive Intervention Alert | AI theo dõi liên tục tín hiệu và **chủ động** cảnh báo instructor khi phát hiện rủi ro vượt ngưỡng (push model: AI monitors → AI detects → AI interrupts → Human decides) | [ai-support-radar.onrender.com](https://ai-support-radar.onrender.com/) (tab Option B) |
| **C** | AI Support Investigator | Instructor đặt câu hỏi tự do, AI điều tra dữ liệu học tập và trả lời kèm bằng chứng (query model: Human asks → AI investigates → AI explains → Human decides) | [ai-support-radar.onrender.com](https://ai-support-radar.onrender.com/) (tab Option C) |

**Prototype chung nhóm:** https://ai-support-radar.onrender.com/

**Những thứ giữ nguyên cho A/B/C** (Comparison Contract): Target user (instructor phụ trách nhiều học viên cùng lúc), Situation (trong/sau phiên học, không đủ thời gian rà soát), Task (xác định ai cần hỗ trợ và vấn đề ở đâu để ưu tiên can thiệp), Desired outcome (phát hiện sớm hơn, ưu tiên đúng người, giảm bỏ sót), Content/data fixture (cùng tập tín hiệu: xem lại/dừng lâu, highlight/ghi chú, đánh dấu "Chưa hiểu", đổi đáp án, trao đổi với AI, kết quả bài tập).

**Distance Check (A/B/C khác mechanism, không chỉ khác UI):**
- A khác B ở trigger: pull (instructor chủ động mở) vs push (AI tự cảnh báo).
- B khác C ở chủ thể hành động: B là AI tự phát hiện, C là AI phản hồi theo truy vấn của instructor.
- A khác C ở hình thức thông tin: A là overview cố định (danh sách xếp hạng), C là phân tích theo từng câu hỏi cụ thể.

**Human–AI Design Principle giữ xuyên suốt cả 3 option:** AI không tự kết luận tuyệt đối rằng một học viên "có vấn đề" (vd. tránh "Học viên A yếu" hay "chắc chắn sẽ rớt"); thay vào đó luôn dùng cách diễn đạt xác suất kèm bằng chứng (vd. "Có dấu hiệu cần chú ý", "Các tín hiệu sau làm tăng mức ưu tiên") để instructor tự kiểm tra thêm trước khi quyết định.

---

## 4. Đóng góp của tôi trong nhóm

- **Human–AI Decisions:**
  - Chốt **Problem Hypothesis** và xác định các điều có thể bác bỏ giả thuyết (falsification points).
  - Gỡ solution khỏi hình thức cụ thể (directive → capability trung tính), tránh gắn cứng vào dashboard/heatmap/nút bấm cụ thể.
  - Xây dựng chuỗi thay đổi kỳ vọng (Output → User change → Behavior change → Outcome) cho cả 3 option.
  - Thiết kế cơ chế Human–AI interaction khác nhau cho từng Option (Agency: ai chủ động, AI làm gì, trigger là gì, trade-off) và thực hiện **Distance Check** để đảm bảo A/B/C là 3 solution hypotheses thực sự khác nhau chứ không chỉ khác layout.
  - Xác định **Human–AI Design Principles** cần giữ (AI không tự kết luận tuyệt đối, luôn đưa bằng chứng/tín hiệu thay vì chỉ đưa score/label).
  - Xây dựng **Success Criteria** và **Failure/Falsification Criteria** cho prototype.
- **Shared work (cùng nhóm):**
  - Cùng nhóm xây dựng, code và deploy prototype 3 phần (A/B/C) lên `ai-support-radar.onrender.com`.
  - Tham gia phiên test thực tế với 3 tester ngoài nhóm và tổng hợp Group Feedback Synthesis.
  - Tham gia ghi nhận AI Support Log của nhóm.

---

## 5. Prototype Feedback (tóm tắt)

**Tổng hợp từ 3 Tester ngoài nhóm:**

| Tester | MHV | First action | Option chọn | Lý do & trade-off |
|---|---|---|---|---|
| Tester 1 | 2A202601420 | Nhìn vào số lượng học viên | **C** | Tiện lợi, AI giúp theo dõi và tổng hợp cảnh báo — trade-off: nếu thông tin ban đầu sai dẫn đến gợi ý không phù hợp |
| Tester 2 | 2A202601654 | Nhìn học viên đầu tiên bị cảnh báo ở Option A | **A** | Quen với thao tác của Option A hơn, có yếu tố con người — trade-off: người dùng phải trực tiếp đọc thông tin và tự quyết định |
| Tester 3 | 2A202601037 | Overview tiêu đề và evidence | **C** | Phù hợp bối cảnh nhiều học viên, cần hỗ trợ kịp thời — không có trade-off đáng kể |

**Pattern chung:** Cả 3 tester đều chú ý ngay vào thông tin tổng quan hoặc đối tượng cảnh báo đầu tiên; cần thời gian định hướng ở màn hình/option đầu tiên; và đều dựa vào phần **Evidence** cùng tiêu đề option để định hướng lại/lấy lại quyền kiểm soát khi do dự.

**Group Synthesis:**
- 2/3 tester chọn **Option C** (tiện lợi, hỗ trợ nhanh khi lớp đông học viên); 1/3 chọn **Option A** (ưu tiên yếu tố kiểm soát của con người).
- Evidence dẫn tới quyết định: Tester 1 lo ngại rủi ro "dữ liệu sai dẫn đến gợi ý sai"; Tester 2 chọn A vì muốn "giữ yếu tố kiểm soát của con người".
- **Next Change nhóm chốt:** Phát triển theo hướng **Option C (AI Investigation & Synthesis)** nhưng tích hợp thêm **khung Evidence minh bạch và cơ chế can thiệp** từ Option A, để người dùng vừa tiết kiệm thời gian vừa duy trì quyền kiểm soát dữ liệu.
- **Still Unproven:**
  - Chưa kiểm chứng được trong bối cảnh lớp học thật (real-time, nhiều học viên thực tế) liệu instructor có thực sự tin cậy và can thiệp sớm, hay vẫn bỏ sót/nghi ngờ kết quả do false positive.
  - Chưa đo lường được mức độ sẵn sàng can thiệp thực tế khi dữ liệu tín hiệu đầu vào bị nhiễu hoặc không đầy đủ.

---

## 6. AI Support Log

**AI đã giúp ở đâu?**
- Viết code và deploy HTML cho prototype 3 phần (A/B/C).
- Tìm câu hỏi dẫn dắt trong test prompt.
- Tổng hợp thông tin giữa 3 bản feedback của tester.

**AI sai, hời hợt hoặc làm các option giống nhau ở đâu?**
- AI quá chi tiết khi tổng hợp thông tin giữa 3 feedback, đưa ra lượng thông tin mới không cần thiết.

**Nhóm đã tự sửa hoặc quyết định lại điều gì?**
- Lược bỏ các ý dư thừa, chỉ giữ lại những từ khóa chính.

---

## Cấu trúc repo

```text
Track1_Day18_2A202601742_NguyenVuVietAnh/
├── README.md
├── three-option-design-sheet.md
├── prototype-link.md
├── prototype-feedback-note.md
├── group-feedback-synthesis.md
└── ai-support-log.md
```

---

**Tự kiểm 5 Gate**

| Gate | Trạng thái |
|------|------------|
| 1. Evidence Continuity | Chưa đủ — Problem Hypothesis rõ và có điều chưa chứng minh, nhưng **repo chưa có quote/evidence trực tiếp từ Day 17** để nối tiếp |
| 2. Meaningful Options | Đạt — A/B/C khác interaction model (pull/push/query), có Distance Check rõ ràng |
| 3. Human Control | Đạt — mỗi option có Agency (User làm gì/AI làm gì), có Human–AI Design Principles (AI không tự kết luận tuyệt đối) |
| 4. Test-ready | Đạt — có prototype thật (`ai-support-radar.onrender.com`) đã được 3 tester ngoài nhóm dùng thử |
| 5. Learning | Đạt — có Feedback Note của 3 tester + Group Synthesis + Next Change + Still Unproven |