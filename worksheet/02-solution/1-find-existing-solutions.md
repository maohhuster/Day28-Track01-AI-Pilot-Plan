---
artifact: 5 — Solution Approach (phần khám phá)
bai-tap: Solution — tìm lời giải đã có sẵn trước khi tự xây
phase: Double Diamond vòng 2 · ◇ giãn (mở hết lựa chọn, chưa chốt)
time: ~8 phút
input: 01-frame/3-FINAL-problem-framing.md · 00-context.md · prompts/04-find-solutions.md
nop-cuoi: Không — file trung gian
---

# 1 — Find existing solutions (đừng xây lại từ số 0)

## Bước 0 — Bài này thực ra là dạng bài gì?

- **Quick Win của nhóm, viết lại thành 1 dạng bài chung**: Chuyển bằng chứng học tập cá nhân thành danh sách lỗ hổng năng lực và khuyến nghị ôn tập ưu tiên, có nguồn và có người review.
- **Input → output thực chất là gì**: Bài nộp/rubric/self-assessment/tiến độ → 2-3 điểm yếu + 3 action học tập + nguồn tài liệu liên quan.
- **Ràng buộc không bỏ được**: privacy, citation, human review, budget nhỏ, formative only, tránh overload.

## Phần A — Deep research: ai giải dạng bài này rồi, giải sao?

| Tầng | Hỏi AI/web câu gì | Tìm được gì | Nguồn / 🧮 nếu là giả định |
|---|---|---|---|
| 1 · Map | "Learning evidence to personalized study recommendations thường giải bằng hướng nào?" | 4 hướng chính: learning analytics dashboard; adaptive learning/mastery system; AI tutor/teacher assistant; rule-based recommender dựa trên rubric/concept map. | Springer Smart Learning Environments 2026: AI hỗ trợ personalized learning qua real-time feedback, adaptive sequencing, intelligent tutoring, dynamic learning pathways. https://link.springer.com/article/10.1186/s40561-026-00440-6 |
| 2 · Tiền lệ | "Đội nào đã dùng dữ liệu học tập để gợi ý can thiệp/học lại?" | Carnegie Mellon OLI dùng assessment gắn learning objectives, dashboard cho instructor xem concept học viên đang khó và can thiệp đúng chỗ. | CMU DataLab: https://www.cmu.edu/datalab/research/success-story-stats.html |
| 2 · Tiền lệ | "AI/edtech nào đang gợi ý nội dung tiếp theo cho giáo viên/học viên?" | Khanmigo Teacher Tools có Recommend Assignments và Class Snapshot: gợi ý nội dung Khan Academy nên làm tiếp, phân tích learning time, assignment completion, mastery progress. | Khan Academy Help Center: https://support.khanacademy.org/hc/en-us/articles/14799047733645-What-teacher-tools-are-available-on-Khanmigo |
| 3 · Phản chứng | "Ca nào dễ thất bại khi cá nhân hóa học tập?" | Rủi ro không nằm ở model hay UI mà ở định nghĩa cá nhân hóa mơ hồ, thiếu empirical validation, privacy/ethics/bias và human-AI collaboration. | Springer 2026 review nêu các khoảng trống: conceptual clarity, privacy, bias, ethics, teacher preparation, human-AI collaboration. https://link.springer.com/article/10.1186/s40561-026-00440-6 |
| 4 · Thu hẹp | "Với budget nhỏ, cần citation và coach review, hướng nào khả thi 6 tuần?" | Khả thi nhất là Boost: dùng LLM/API sẵn + rubric/concept map/tài liệu khóa riêng; sinh checklist cá nhân có citation, coach review sample/low-confidence. Không nên Build platform adaptive đầy đủ ở pilot đầu. | Kết luận nhóm dựa trên nguồn trên + ràng buộc AI20k; chi phí cụ thể là 🧮 giả định cần đo tuần 1. |

## Phần B — Rút về 2–3 hướng khả thi

| Hướng giải khả thi | Ai làm rồi (gần bài mình nhất) | Nguồn / 🧮 | Hợp ràng buộc `00-context`? |
|---|---|---|---|
| Boost: LLM + rubric/concept map + tài liệu khóa để tạo checklist cá nhân có citation | Khanmigo gợi ý assignment và phân tích lớp; CMU OLI dùng objective-level data để dashboard/can thiệp | Khan Academy Help Center; CMU DataLab | Có. Không xây platform, dùng dữ liệu riêng, có coach review. |
| Buy/Adapt: dùng LMS analytics hoặc tool edtech có sẵn rồi cấu hình khuyến nghị | Khanmigo/Khan Academy, các adaptive learning platform | Khan Academy; Springer review | Có thể, nhưng phụ thuộc tool hiện tại của AI20k và tích hợp LMS. |
| Build: hệ thống adaptive learning đầy đủ theo concept, goal, progress, behavior | OLI/adaptive learning systems | CMU DataLab; Springer review | Không phù hợp pilot đầu vì cần taxonomy, tracking, content graph, consent và vận hành lâu dài. |

**"Đi từ 5 lên" — nhóm kế thừa cụ thể cái gì**:

```text
Không phát minh lại "personalized learning". Nhóm kế thừa 3 nguyên tắc đã thấy ở OLI/Khanmigo: gắn output với learning objective/concept, chỉ khuyến nghị hành động tiếp theo, và để instructor/coach dùng dashboard hoặc review thay vì để AI tự quyết.
```

## Phát hiện ban đầu

- Cá nhân hóa hiệu quả cần concept map/rubric rõ hơn là model phức tạp.
- Nên thiết kế output dạng "ít nhưng đúng": tối đa 3 action, có lý do và nguồn.
- Human review là một phần của sản phẩm, không phải bước phụ sau cùng.

## Câu hỏi mở (mang sang bước chốt)

- Có mapping chính thức từ lỗi D28 sang tài liệu D2/D27/D28 chưa?
- Ngưỡng confidence nào bắt buộc coach review?
- Nên gửi checklist cho từng học viên hay trước tiên gửi cho coach để duyệt?

## Tổng kiểm tra trước khi sang `2-FINAL-solution.md`

| Hạng mục | Xong? |
|---|---|
| Gọi được dạng bài trong 1 câu, không còn chữ domain | X |
| Đủ 4 tầng deep research, tầng nào cũng có kết quả | X |
| Mỗi kết quả có nguồn, hoặc đánh dấu 🧮 nếu là giả định | X |
| Rút về 2–3 hướng + nói được "đi từ 5 lên" cái gì | X |
