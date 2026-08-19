# Track 1 — Day 18 — Multiple Prototypes - Human–AI design

## Thông tin cá nhân và nhóm

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

# 1. Problem Hypothesis

## 1.1 Problem Hypothesis chốt

> Khi phụ trách nhiều học viên cùng lúc, instructor khó nhận ra kịp thời ai đang gặp khó và ở đâu vì thiếu công cụ/thời gian rà soát tín hiệu từng người → can thiệp trễ hoặc bỏ sót → học viên gặp khó âm thầm cho đến khi hậu quả xảy ra như rớt bài hoặc bỏ học.

## 1.2 Điều cần kiểm chứng

Giả thuyết này dựa trên chuỗi logic:

1. Instructor phụ trách nhiều học viên cùng lúc.
2. Instructor không đủ thời gian để rà soát thủ công tín hiệu của từng người.
3. Vì vậy instructor khó phát hiện sớm ai đang gặp khó và gặp khó ở đâu.
4. Việc phát hiện muộn dẫn đến can thiệp trễ hoặc bỏ sót.
5. Nếu instructor được hỗ trợ nhận biết và ưu tiên đúng người, khả năng can thiệp sớm sẽ tăng.

## 1.3 Điều có thể bác bỏ Problem Hypothesis

Problem Hypothesis bị lung lay hoặc cần điều chỉnh nếu:

- Instructor thực tế đã biết rõ ai đang gặp khó nhưng vẫn không can thiệp được.
- Nguyên nhân chính không phải thiếu khả năng nhận biết mà là thiếu thời gian, quyền hạn hoặc nguồn lực để hỗ trợ.
- Các tín hiệu học tập không đủ đáng tin để xác định học viên đang gặp khó.
- Instructor không xem việc phát hiện sớm học viên gặp khó là vấn đề quan trọng.
- Việc biết ai gặp khó không làm thay đổi thời điểm hoặc chất lượng can thiệp.

> Điểm bác bỏ quan trọng: Nếu instructor đã biết “ai cần hỗ trợ và ở đâu” nhưng vẫn không can thiệp sớm hơn, bottleneck có thể không nằm ở khả năng nhận biết/prioritize mà nằm ở workload, communication cost hoặc intervention workflow.

---

# 2. Solution – Gỡ solution khỏi hình thức cụ thể

## 2.1 Directive

Sau mỗi phiên học, hệ thống phân tích các tín hiệu như di chuyển giữa slide, dừng lâu hoặc xem lại, highlight và ghi chú, đánh dấu “Chưa hiểu”, thay đổi câu trả lời, và nội dung trao đổi với AI Chat.

## 2.2 Những phần trong directive đang mô tả feature hoặc cách triển khai

Các yếu tố mang tính solution/feature cụ thể:

- Di chuyển giữa slide.
- Dừng lâu hoặc xem lại.
- Highlight.
- Ghi chú.
- Nút hoặc trạng thái “Chưa hiểu”.
- Thay đổi câu trả lời.
- Nội dung trao đổi với AI Chat.
- Việc AI tự động phân tích các tín hiệu này.

Những yếu tố trên là các cách thu thập hoặc xử lý tín hiệu, không phải capability cốt lõi.

## 2.3 Capability trung tính

> Giúp chương trình nhận biết và ưu tiên những học viên đang cần được hỗ trợ.

Hoặc diễn đạt đầy đủ hơn:

> Cho phép instructor nhận biết sớm học viên nào đang gặp khó, vấn đề nằm ở đâu và ai cần được ưu tiên hỗ trợ trước.

Capability này không phụ thuộc vào:

- tên màn hình;
- dashboard;
- heatmap;
- nút “Chưa hiểu”;
- AI Chat;
- một loại dữ liệu cụ thể;
- một cách hiển thị cụ thể.

---

# 3. Change – Chuỗi thay đổi được kỳ vọng

Không nhảy trực tiếp từ feature đến outcome. Chuỗi thay đổi được kỳ vọng là:

## 3.1 Output

Team tạo ra khả năng:

- thu thập hoặc tiếp nhận các tín hiệu học tập;
- tổng hợp tín hiệu của nhiều học viên;
- phát hiện dấu hiệu bất thường hoặc khó khăn;
- cung cấp thông tin ưu tiên cho instructor.

## 3.2 User change

Instructor:

- biết học viên nào có khả năng đang gặp khó;
- biết họ gặp khó ở phần nào;
- giảm thời gian rà soát thủ công;
- có cơ sở để quyết định ai cần được kiểm tra trước.

## 3.3 Behavior change

Instructor:

- kiểm tra sớm hơn;
- ưu tiên đúng người hơn;
- chủ động tiếp cận học viên có dấu hiệu gặp khó;
- can thiệp trước khi vấn đề trở nên nghiêm trọng.

## 3.4 Outcome

Kỳ vọng:

- giảm số học viên gặp khó nhưng bị bỏ sót;
- giảm độ trễ giữa lúc học viên bắt đầu gặp khó và lúc instructor can thiệp;
- tăng khả năng hỗ trợ đúng người, đúng thời điểm;
- giảm nguy cơ học viên rớt bài hoặc bỏ học do khó khăn kéo dài không được phát hiện.

## 3.5 Chuỗi thay đổi

```text
Tín hiệu học tập
      ↓
Nhận biết dấu hiệu gặp khó
      ↓
Instructor biết ai cần chú ý
      ↓
Instructor ưu tiên đúng người
      ↓
Can thiệp sớm hơn
      ↓
Giảm bỏ sót / giảm hậu quả nghiêm trọng
```

---

# 4. Chọn ba cách giải

Ba options cùng xuất phát từ một Problem Hypothesis nhưng đại diện cho ba Solution Hypotheses khác nhau.

Mục tiêu không phải tạo ba layout khác nhau, mà là tạo ba cơ chế Human–AI interaction khác nhau.

---

## 4.1 Những thứ phải giữ nguyên cho A/B/C

| Thành phần | Quyết định chung cho A/B/C |
|---|---|
| **Target user** | Instructor phụ trách nhiều học viên cùng lúc |
| **Situation** | Trong hoặc sau phiên học, instructor không có đủ thời gian để rà soát tình trạng từng học viên |
| **Task** | Xác định học viên nào đang cần hỗ trợ và vấn đề nằm ở đâu để quyết định ưu tiên can thiệp |
| **Desired outcome** | Instructor phát hiện khó khăn sớm hơn, ưu tiên đúng người và giảm trường hợp học viên gặp khó nhưng bị bỏ sót |
| **Content/data fixture** | Cùng một tập dữ liệu học viên và các tín hiệu học tập như xem lại/dừng lâu ở nội dung, highlight/ghi chú, đánh dấu chưa hiểu, thay đổi câu trả lời, trao đổi với AI, kết quả bài tập |

---

## 4.2 Những thứ được phép khác

### Option A – Prioritized Support Radar

**Solution mechanism**

AI tổng hợp tín hiệu học tập của nhiều học viên và tạo một danh sách ưu tiên để instructor chủ động rà soát.

**User làm gì?**

- Mở danh sách học viên cần chú ý.
- Xem thứ tự ưu tiên.
- Chọn một học viên.
- Xem lý do tại sao học viên đó được đánh dấu.
- Quyết định có cần can thiệp hay không.

**AI làm gì?**

- Tổng hợp các tín hiệu học tập.
- Phát hiện pattern có khả năng liên quan đến khó khăn.
- Ước lượng mức cần hỗ trợ.
- Xếp hạng học viên.
- Hiển thị các tín hiệu chính làm căn cứ.

**Trigger**

Instructor chủ động mở hệ thống để kiểm tra tình trạng lớp.

**Trade-off chính**

Ưu điểm:

- Cho instructor cái nhìn tổng quan.
- Dễ so sánh nhiều học viên.
- Instructor vẫn giữ quyền quyết định.

Hạn chế:

- Instructor vẫn phải nhớ và chủ động mở hệ thống.
- Nếu instructor quá bận, danh sách tốt vẫn có thể không được xem kịp thời.

**Solution hypothesis**

> Nếu AI giúp instructor tổng hợp và ưu tiên học viên cần chú ý, instructor sẽ rà soát nhanh hơn và can thiệp sớm hơn.

---

### Option B – Proactive Intervention Alert

**Solution mechanism**

AI liên tục theo dõi tín hiệu và chủ động cảnh báo instructor khi phát hiện một học viên có dấu hiệu khó khăn đáng kể.

**User làm gì?**

- Nhận cảnh báo.
- Xem học viên nào đang được cảnh báo.
- Xem lý do hoặc bằng chứng.
- Quyết định bỏ qua, theo dõi thêm hoặc can thiệp.

**AI làm gì?**

- Theo dõi tín hiệu học tập.
- Phát hiện pattern hoặc mức rủi ro vượt ngưỡng.
- Xác định tình huống cần instructor chú ý.
- Gửi cảnh báo kèm lý do.

**Trigger**

AI tự kích hoạt khi phát hiện tín hiệu đáng lo hoặc rủi ro vượt một ngưỡng nhất định.

**Trade-off chính**

Ưu điểm:

- Không phụ thuộc instructor nhớ mở dashboard.
- Có khả năng phát hiện và phản ứng nhanh.

Hạn chế:

- Có nguy cơ false positive.
- Quá nhiều cảnh báo có thể gây alert fatigue.
- Nếu AI quá nhạy, instructor có thể mất niềm tin vào hệ thống.

**Solution hypothesis**

> Nếu hệ thống chủ động cảnh báo đúng lúc khi phát hiện dấu hiệu đáng lo, instructor sẽ can thiệp nhanh hơn so với việc phải tự rà soát.

---

### Option C – AI Support Investigator

**Solution mechanism**

Instructor chủ động đặt câu hỏi và AI điều tra dữ liệu học tập để trả lời ai đang cần hỗ trợ, gặp khó ở đâu và vì sao.

**User làm gì?**

Instructor có thể hỏi:

- “Ai đang gặp khó với phần X?”
- “Hôm nay ai cần tôi hỗ trợ nhất?”
- “Có học viên nào có dấu hiệu tụt lại không?”
- “Tại sao học viên A được xem là đang gặp khó?”

Sau đó instructor xem kết quả và quyết định hành động.

**AI làm gì?**

- Hiểu câu hỏi của instructor.
- Truy xuất các tín hiệu liên quan.
- Phân tích dữ liệu.
- Xác định học viên phù hợp với câu hỏi.
- Tóm tắt bằng chứng và lý do.
- Trả lời theo nhu cầu cụ thể của instructor.

**Trigger**

Instructor có câu hỏi hoặc đang cần đưa ra quyết định hỗ trợ.

**Trade-off chính**

Ưu điểm:

- Linh hoạt.
- Cho phép instructor điều tra theo context thực tế.
- Không buộc AI phải luôn tự quyết định ai là người “có vấn đề”.

Hạn chế:

- Phụ thuộc instructor biết mình cần hỏi gì.
- Có thể bỏ sót những trường hợp instructor không nghĩ đến.
- Chất lượng phụ thuộc vào khả năng giải thích và truy xuất của AI.

**Solution hypothesis**

> Nếu instructor có thể hỏi AI trực tiếp về tình trạng học viên và nhận câu trả lời có bằng chứng, instructor sẽ ra quyết định hỗ trợ nhanh và chính xác hơn.

---

# 5. Bảng so sánh A/B/C

| Thành phần | Option A | Option B | Option C |
|---|---|---|---|
| **Solution mechanism** | Prioritized Support Radar – AI tổng hợp và xếp hạng học viên cần chú ý | Proactive Intervention Alert – AI tự phát hiện và cảnh báo | AI Support Investigator – instructor hỏi và AI điều tra |
| **User làm gì?** | Chủ động mở danh sách và rà soát | Nhận cảnh báo và quyết định hành động | Đặt câu hỏi và xem kết quả phân tích |
| **AI làm gì?** | Tổng hợp → đánh giá → xếp hạng → giải thích | Theo dõi → phát hiện → cảnh báo → giải thích | Hiểu câu hỏi → truy xuất → phân tích → trả lời |
| **Trigger** | Instructor chủ động kiểm tra | AI phát hiện rủi ro | Instructor đặt câu hỏi |
| **Trade-off chính** | Tổng quan tốt nhưng vẫn cần user chủ động | Nhanh nhưng dễ alert fatigue / false positive | Linh hoạt nhưng phụ thuộc user biết hỏi gì |

---

# 6. Distance Check

Ba phương án không chỉ khác màu sắc, layout hoặc wording.

Chúng khác nhau ở mô hình tương tác giữa Human và AI.

## Option A

```text
Human scans
    ↓
AI prioritizes
    ↓
Human decides
```

Instructor vẫn là người chủ động khởi tạo quá trình kiểm tra.

## Option B

```text
AI monitors
    ↓
AI detects
    ↓
AI interrupts
    ↓
Human decides
```

AI chủ động kéo sự chú ý của instructor.

## Option C

```text
Human asks
    ↓
AI investigates
    ↓
AI explains
    ↓
Human decides
```

Instructor chủ động nêu câu hỏi, AI đóng vai trò điều tra.

### Kết luận Distance Check

- A khác B vì trigger khác nhau: pull vs push.
- B khác C vì B tự phát hiện còn C phản hồi theo truy vấn.
- A khác C vì A cung cấp overview cố định còn C cung cấp phân tích theo câu hỏi.

Do đó A/B/C là ba solution hypotheses khác nhau, không phải ba phiên bản UI của cùng một giải pháp.

---

# 7. Điều không nên làm

Không nên tạo:

- Option A = dashboard.
- Option B = heatmap.
- Option C = card list.

Nếu cả ba đều có logic:

```text
AI phân tích
→ tạo danh sách
→ instructor xem
```

thì chúng chỉ khác presentation, không khác solution mechanism.

Bài Multiple Prototypes cần kiểm tra các giả định khác nhau về cách Human và AI chia việc.

---

# 8. Các giả định đang được kiểm tra

## Option A kiểm tra giả định

> Instructor sẵn sàng chủ động kiểm tra nếu việc rà soát đã đủ nhanh và thông tin được ưu tiên tốt.

Nếu instructor có danh sách tốt nhưng vẫn không mở hoặc không hành động, giả định này yếu.

## Option B kiểm tra giả định

> Vấn đề chính là instructor không có thời gian hoặc không nhớ kiểm tra, vì vậy AI cần chủ động kéo sự chú ý.

Nếu cảnh báo liên tục nhưng instructor bỏ qua, solution này có thể không phù hợp.

## Option C kiểm tra giả định

> Instructor không cần AI luôn tự quyết định ai có vấn đề; họ cần một công cụ điều tra nhanh khi có câu hỏi.

Nếu instructor không biết hỏi gì hoặc không chủ động truy vấn, solution này có thể không giải quyết được việc bỏ sót.

---

# 9. Human–AI Design Principles cần giữ

Dù chọn Option nào, AI không nên tự kết luận tuyệt đối rằng một học viên “có vấn đề”.

Nên dùng cách diễn đạt như:

- “Có dấu hiệu cần chú ý.”
- “Có khả năng đang gặp khó.”
- “Các tín hiệu sau làm tăng mức ưu tiên.”
- “Instructor nên kiểm tra thêm trước khi quyết định.”

AI nên cung cấp bằng chứng hoặc tín hiệu làm căn cứ thay vì chỉ đưa ra một score hoặc label.

Ví dụ:

```text
Học viên A – mức ưu tiên cao

Tín hiệu:
- xem lại phần Backpropagation 4 lần;
- thay đổi đáp án 3 lần;
- đánh dấu “Chưa hiểu”;
- hỏi AI 5 câu liên quan cùng một khái niệm.

Gợi ý:
Có thể kiểm tra mức hiểu của học viên về Backpropagation.
```

Không nên:

```text
Học viên A yếu.
```

hoặc:

```text
Học viên A chắc chắn sẽ rớt.
```

---

# 10. Success Criteria

Prototype được xem là có tín hiệu tốt nếu instructor:

- xác định được nhanh hơn ai đang cần hỗ trợ;
- hiểu được tại sao học viên đó được ưu tiên;
- cảm thấy đủ tin tưởng để quyết định bước tiếp theo;
- giảm thời gian rà soát thủ công;
- có khả năng phát hiện trường hợp mà trước đó họ có thể bỏ sót.

Không chỉ đo:

- prototype đẹp;
- instructor thích giao diện;
- instructor thấy AI “thông minh”.

Điều cần kiểm tra là:

> Prototype có giúp instructor đưa ra quyết định hỗ trợ tốt hơn hay không?

---

# 11. Failure / Falsification Criteria

Giải pháp cần xem xét lại nếu:

- Instructor không tin các tín hiệu AI đưa ra.
- Instructor mất quá nhiều thời gian để hiểu kết quả.
- AI tạo nhiều false positive.
- Instructor đã biết ai gặp khó mà không cần hệ thống.
- Instructor biết ai gặp khó nhưng vẫn không thể can thiệp.
- Việc sử dụng AI không làm thay đổi quyết định hoặc thời điểm can thiệp.
- Học viên bị gắn nhãn sai hoặc bị ưu tiên dựa trên tín hiệu không phù hợp.

Nếu các trường hợp này xảy ra, cần quay lại Problem Hypothesis thay vì chỉ sửa giao diện.

---

# 12. Bản chốt ngắn để điền vào bài

## Problem Hypothesis

> Khi phụ trách nhiều học viên cùng lúc, instructor khó nhận ra kịp thời ai đang gặp khó và ở đâu vì thiếu công cụ/thời gian rà soát tín hiệu từng người → can thiệp trễ hoặc bỏ sót → học viên gặp khó âm thầm cho đến khi hậu quả xảy ra như rớt bài hoặc bỏ học.

## Capability

> Cho phép instructor nhận biết sớm học viên nào đang gặp khó, vấn đề nằm ở đâu và ai cần được ưu tiên hỗ trợ trước.

## Option A

**Solution mechanism:** AI tổng hợp và xếp hạng học viên cần chú ý.

**User:** Chủ động mở danh sách, xem ưu tiên và kiểm tra chi tiết.

**AI:** Phân tích tín hiệu, xếp hạng và giải thích lý do.

**Trigger:** Instructor chủ động kiểm tra.

**Trade-off:** Tổng quan tốt nhưng vẫn phụ thuộc instructor chủ động mở hệ thống.

## Option B

**Solution mechanism:** AI chủ động cảnh báo khi phát hiện dấu hiệu đáng lo.

**User:** Nhận cảnh báo, xem lý do và quyết định can thiệp.

**AI:** Theo dõi tín hiệu, phát hiện rủi ro và gửi cảnh báo.

**Trigger:** AI phát hiện pattern/risk vượt ngưỡng.

**Trade-off:** Phát hiện nhanh nhưng có nguy cơ false positive và alert fatigue.

## Option C

**Solution mechanism:** Instructor hỏi, AI điều tra dữ liệu để xác định người cần hỗ trợ.

**User:** Đặt câu hỏi và xem kết quả.

**AI:** Hiểu câu hỏi, truy xuất dữ liệu, phân tích và giải thích.

**Trigger:** Instructor có câu hỏi hoặc cần ra quyết định.

**Trade-off:** Linh hoạt nhưng phụ thuộc instructor biết mình cần hỏi gì.

## Distance check

```text
A: Human scans → AI prioritizes
B: AI monitors → AI alerts Human
C: Human asks → AI investigates
```

Ba option khác nhau ở interaction model và solution mechanism, không chỉ khác layout hoặc wording.
