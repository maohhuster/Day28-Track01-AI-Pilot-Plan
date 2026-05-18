---
artifact: 1 — Track & Big Ask + 2 — Tool Breakdown
bai-tap: Frame — nghe đúng đề rồi tách nhỏ
phase: Double Diamond vòng 1 · ◇ giãn (nghe rộng, chưa chốt)
time: ~12 phút
input: 00-context.md · track card · prompts/01-breakdown.md
nop-cuoi: Không — file trung gian
---

# 1 — Intake & Breakdown: nghe đúng đề, tách nhỏ

## Phần A — Phát biểu lại Big Ask bằng lời nhóm

- **Big Ask, viết lại bằng lời nhóm**: Stakeholder muốn một hệ thống giúp mỗi học viên biết mình nên học gì tiếp theo, cần ôn lại phần nào và cần chuẩn bị ra sao trước 6 tuần thực chiến. Nhóm không hiểu đây là "chatbot học tập cho mọi thứ", mà là một lớp hỗ trợ ra quyết định học tập dựa trên bằng chứng từ bài làm, tiến độ và mục tiêu của học viên.
- **Tại sao bây giờ**: Sau Day 28, học viên chuyển sang giai đoạn thực chiến; nếu không biết mình yếu ở đâu thì các lỗ hổng từ D2/D27/D28 sẽ đi theo vào dự án thật. Với quy mô ~500 học viên, coach khó tự đọc từng bài, nhắc từng người và cá nhân hóa lộ trình thủ công.
- **Người dùng đầu tiên cụ thể**: Học viên vừa hoàn thành D28 và sắp bước vào 6 tuần thực chiến; coach là người review gợi ý trước khi gửi rộng.

## Phần B — Tách công cụ lớn thành 5–8 use case

| # | Use case (AI làm gì · cho ai · để họ làm được gì) | Người dùng | Làm được độc lập? |
|---|---|---|---|
| 1 | AI đọc bài nộp D28 + self-assessment để tạo checklist "điểm yếu trước thực chiến" cho từng học viên | Học viên | Có |
| 2 | AI gợi ý 3 tài liệu/ngày học cần xem lại dựa trên lỗi trong bài nộp D28 | Học viên | Có |
| 3 | AI sinh lộ trình bù 7 ngày cho học viên yếu ở Build/Buy/Boost và Pilot Plan | Học viên | Có |
| 4 | AI tạo view cho coach: nhóm/học viên nào cần can thiệp trước khi vào project thật | Coach | Có, nếu có bài nộp/rubric |
| 5 | AI theo dõi tiến độ theo concept xuyên suốt D2, D27, D28 để nhắc học viên ôn đúng chỗ | Học viên, coach | Không — cần taxonomy concept ổn định |
| 6 | AI gợi ý peer hỗ trợ dựa trên điểm mạnh/yếu bổ sung giữa các học viên | Học viên | Không — cần consent và dữ liệu hồ sơ rộng hơn |
| 7 | AI chẩn đoán kỹ năng đầu/giữa khóa bằng quiz adaptive | Học viên, instructor | Có, nhưng cần ngân hàng câu hỏi |
| 8 | AI cá nhân hóa lộ trình theo mục tiêu nghề nghiệp PM/founder/engineer/operator | Học viên | Có, nhưng cần goal profile rõ |

## Phát hiện ban đầu

- Quick Win nên nằm ở khoảnh khắc ngay sau D28, vì dữ liệu vừa có, nhu cầu chuẩn bị 6 tuần thực chiến rất rõ.
- Use case liên quan peer matching và tracking dài hạn hấp dẫn nhưng dễ chạm privacy/consent và cần dữ liệu nhiều hơn.
- "Personalized Learning Path" chỉ có giá trị nếu khuyến nghị khác nhau theo lỗi thật, không chỉ template chung thay tên.

## Câu hỏi mở (mang sang bước chọn Quick Win)

- Có lấy được bài nộp/rubric D28 ở định dạng đủ máy đọc không?
- Coach có thời gian review bao nhiêu mẫu trước khi gửi khuyến nghị cho học viên?
- Học viên muốn nhận lộ trình qua kênh nào: LMS, Discord DM, hay file cá nhân?

## Tổng kiểm tra trước khi sang `2-quick-win.md`

| Hạng mục | Xong? |
|---|---|
| Cả nhóm phát biểu lại Big Ask giống nhau, không cần nhìn card | X |
| Có 5–8 use case dạng "AI làm X cho ai để Y" | X |
| Có ≥4 use case thật sự độc lập | X |
| Nhóm KHÔNG còn ý định pitch "build cả platform" | X |
