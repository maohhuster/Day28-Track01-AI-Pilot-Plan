---
artifact: 5 — Solution Approach + 6 — Demo/Mockup/Flow (bản nộp phase Solution)
bai-tap: Solution — chốt cách làm + cho stakeholder nhìn thấy
phase: Double Diamond vòng 2 · ◆ siết (chốt 1 cách làm + 1 artifact trực quan)
time: ~12 phút
input: 1-find-existing-solutions.md · 00-context.md · templates/demo-examples.md · prompts/05-demo-challenge.md
nop-cuoi: Có — bản nộp của phase Solution
---

# 2 — FINAL: Solution Approach + Demo/Mockup/Flow

## Phần A — Chốt cách làm

- **Cách làm chốt**: **Boost** — dùng LLM/API có sẵn + dữ liệu riêng của AI20k (rubric, concept map, tài liệu D2/D27/D28, bài nộp D28, self-assessment) để sinh checklist cá nhân có citation và coach review.
- **Lý do CẦN**: Track này là productivity/learning-support layer, chưa phải lợi thế cạnh tranh lõi cần build platform từ đầu. Pilot cần chứng minh học viên có nhận đúng action học tập không trước khi đầu tư vào tracking dài hạn. Cách Boost tận dụng được pattern đã có ở adaptive learning/teacher tools nhưng giữ dữ liệu và rubric theo AI20k.
- **Vì sao KHÔNG "Build từ số 0"**: Build từ số 0 cần taxonomy concept hoàn chỉnh, tích hợp LMS/Discord, consent workflow, dashboard và logging; rủi ro vượt phạm vi 6 tuần. Nếu pilot nhỏ không chứng minh adoption/quality, platform lớn sẽ lãng phí.
- **Tool / API / vendor cần + ước lượng chi phí thô**:
  - LLM/API hoặc ChatGPT Team/Gemini/Claude dùng cho prototype: 🧮 2-5 USD/tuần nếu chạy batch nhỏ 80 học viên, cần đo thực tế theo token tuần 1.
  - Storage tạm: Google Sheet/CSV + Drive/LMS link, không lưu dữ liệu nhạy cảm ngoài phạm vi được phép.
  - Thời gian coach review: 🧮 2 giờ cho 15-20 checklist mẫu + toàn bộ checklist low-confidence.

## Phần B — Data & ai review

| Cần gì | Có sẵn trong AI20k? | Trong lab dùng (mẫu/giả định) | Privacy? |
|---|---|---|---|
| Data: bài nộp D28 + rubric/gate feedback | Có/giả định có | 5-10 bài mẫu hoặc bài nhóm hiện tại | Có dữ liệu học viên; ẩn tên khi test |
| Data: mapping concept -> tài liệu D2/D27/D28 | Có một phần trong handbook/template | Bảng mapping thủ công 10-15 concept chính | Không nhạy cảm |
| Data: self-assessment 5 câu | Chưa chắc có | Form giả định: mục tiêu, confidence, phần yếu, thời gian học, kênh nhận | Có, cần consent |
| Data: tiến độ LMS/quiz | Có thể có | Chỉ dùng nếu được cấp quyền; nếu không thì bỏ khỏi pilot đầu | Có, chỉ dùng tối thiểu |

- **Output rủi ro cao**: Gán nhãn "học viên yếu ở X" hoặc khuyến nghị sai khiến học viên ôn nhầm; output này không được dùng để chấm điểm hoặc đánh giá năng lực chính thức.
- **Ai review + bao nhiêu mẫu + pass/fail theo gì**: Coach review 15-20 checklist đầu tiên và 100% checklist low-confidence. Pass nếu >=80% checklist có đúng 1-3 điểm yếu bám evidence, mỗi action có citation, không có nhận định xúc phạm/định kiến, và coach không phải sửa quá 20% nội dung chính.
- **Có cần citation / nói "không biết" khi thiếu nguồn không**: Có. Mỗi action phải trỏ về tài liệu/ngày học/template; nếu không tìm được nguồn, output ghi "không đủ dữ liệu để khuyến nghị".

## Phần C — Bản vẽ trực quan

```text
BEFORE
Học viên nộp D28
   |
   v
Tự đoán mình yếu gì -> đọc lại tài liệu chung -> dễ quá tải / bỏ sót

AFTER: Personalized Learning Path Pilot

Inputs
  [Bài nộp D28]   [Rubric/Gate]   [Self-assessment 5 câu]   [Concept -> tài liệu]
        \              |                    |                       /
         \             |                    |                      /
          v            v                    v                     v
       +-------------------------------------------------------------+
       | AI Draft Checklist                                          |
       | - trích lỗi/evidence từ bài nộp                             |
       | - map lỗi -> concept D2/D27/D28                              |
       | - chọn tối đa 3 action học lại có citation                   |
       | - gắn confidence + lý do                                     |
       +-------------------------------+-----------------------------+
                                       |
                  low confidence hoặc sample review
                                       v
                            [COACH REVIEW / EDIT]
                                       |
                                       v
       +-------------------------------------------------------------+
       | Checklist gửi học viên                                      |
       | 1. Điểm yếu: Exit criteria còn mơ hồ                         |
       |    Evidence: slide pitch chưa nêu điều kiện dừng             |
       |    Action: xem lại D28 Pilot Plan template + sửa 2 dòng      |
       | 2. Điểm yếu: Build/Buy/Boost chọn theo cảm tính              |
       |    Action: làm lại decision tree trong 10 phút               |
       | 3. Điểm yếu: metric thiếu baseline                           |
       |    Action: viết baseline giả định + kế hoạch đo tuần 1       |
       +-------------------------------------------------------------+
                                       |
                                       v
                       Học viên tick action -> phản hồi "đúng/yếu/sai"

Chỗ con người review: coach review trước khi gửi batch đầu, review 100% output low-confidence,
và có quyền ẩn/sửa checklist nếu AI gán nhãn sai hoặc thiếu citation.
```

## Tổng kiểm tra trước khi sang `../03-pilot-plan/`

| Hạng mục | Xong? |
|---|---|
| Cách làm có lý do CẦN, không phải mặc định tự build | X |
| Nói rõ data cần + ai review output rủi ro cao | X |
| Có ≥1 bản vẽ trực quan, người ngoài hiểu trong ~20 giây | X |
| Có đánh dấu chỗ con người review | X |
