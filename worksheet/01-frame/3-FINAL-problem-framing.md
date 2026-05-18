---
artifact: 4 — Problem Framing (bản nộp phase Frame)
bai-tap: Frame — đóng khung vấn đề thật
phase: Double Diamond vòng 1 · ◆ output (chốt — owner xác nhận)
time: ~13 phút
input: 2-quick-win.md · prompts/03-problem-framing-challenge.md
nop-cuoi: Có — đây là bản nộp của phase Frame
---

# 3 — FINAL: Problem Framing

## 9 mục Problem Framing

1. **Original Ask**: "Hệ thống cá nhân hóa lộ trình học cho từng học viên dựa trên mục tiêu, level, tiến độ, điểm yếu, hành vi học."

2. **Reframed problem**: Sau D28, học viên không biết chính xác mình còn hổng concept nào trước 6 tuần thực chiến; coach không đủ thời gian đọc từng bài và biến lỗi trong bài nộp thành lộ trình ôn tập cá nhân. Vấn đề cần giải trước không phải là một platform cá nhân hóa đầy đủ, mà là một cơ chế tạo checklist/lộ trình bù nhỏ, có nguồn, có coach review.

3. **Current workflow**: Học viên tự đọc lại slide/LMS nếu thấy cần, hỏi Discord khi kẹt, hoặc chờ coach feedback thủ công. Feedback nếu có thường nằm trong bài nộp hoặc trao đổi rời rạc, chưa chuyển thành 2-3 hành động học tập cụ thể cho từng học viên.

4. **Pain evidence — bằng SỐ**:

```text
Giả định lab cần xác nhận ở tuần 1:
- Quy mô Track Product: ~80 học viên, tương đương khoảng 26 nhóm 3 người.
- Nếu coach đọc mỗi bài D28 8 phút và viết checklist cá nhân tối thiểu 5 phút/người, riêng phần chuyển lỗi thành action đã tốn khoảng 80 x 5 = 400 phút (~6.7 giờ), chưa tính review bài nhóm.
- Nếu không có checklist, giả định 50% học viên chỉ xem lại tài liệu chung, không biết 1-3 concept yếu nhất của mình trước thực chiến.
- Baseline cần đo: % học viên trả lời đúng câu "3 việc bạn cần ôn trước project là gì?" ngay sau D28; mục tiêu pilot là tăng từ baseline giả định 30-40% lên >=70%.
```

5. **Affected people**:
   - Người dùng: học viên sau D28, nhất là nhóm tự thấy chưa chắc về Problem Framing, Build/Buy/Boost, metric/exit criteria.
   - Người quyết: instructor/owner chương trình.
   - Người review/expert: coach phụ trách Track Product, có quyền sửa/ẩn khuyến nghị trước khi gửi.

6. **Constraints**:
   - Privacy: chỉ dùng dữ liệu học tập cần thiết; không dùng Discord DM hoặc dữ liệu nhạy cảm nếu chưa có consent.
   - Human review: checklist mẫu và các trường hợp low-confidence phải có coach review.
   - Citation: mọi tài liệu gợi ý phải trỏ về ngày học/handbook/template cụ thể; thiếu nguồn thì nói "không đủ dữ liệu".
   - Budget nhỏ: dùng LLM/API hoặc workflow no-code hiện có; không xây platform.
   - Formative: checklist chỉ là hỗ trợ học tập, không dùng để chấm điểm.
   - Adoption: output tối đa 3 action để học viên thật sự làm.

7. **Quick Win đã chọn**: Sau D28, AI tạo checklist/lộ trình bù cá nhân "bạn đang yếu chỗ nào trước 6 tuần thực chiến" và gợi ý tối đa 3 tài liệu/action cần xem lại.

8. **Open questions**:
   - Dữ liệu bài nộp D28 có đủ chuẩn hóa để trích lỗi theo concept không?
   - Coach muốn review 100% checklist hay chỉ review sample + checklist low-confidence?
   - Kênh gửi nào có adoption cao nhất: LMS, Discord, hay link riêng?
   - Học viên có phản hồi "đúng điểm yếu của tôi" sau khi nhận checklist không?

9. **Validation**:

```text
Owner giả định: Có, đây là vấn đề đáng giải nếu phạm vi giữ đủ nhỏ.
Lý do: giai đoạn sau D28 cần chuyển từ học framework sang thực chiến; một checklist đúng lúc giúp học viên biết ôn gì và giúp coach nhìn thấy nhóm cần can thiệp. Điều kiện: không được biến pilot thành platform cá nhân hóa đầy đủ, không dùng dữ liệu nhạy cảm thiếu consent, và phải đo adoption/quality sớm.
```

## Tự phản biện

- Khung đã tránh câu chung chung "học viên cần học tốt hơn"; nó chỉ rõ khoảnh khắc sau D28, người đau là học viên/coach, và việc cần làm là chuyển lỗi thành action học tập.
- Số liệu hiện là giả định lab, không dùng như fact. Tuần 1 phải đo baseline bằng survey 3 câu + audit 10-15 bài nộp D28.
- Nếu giả định chính sai (học viên không muốn nhận checklist), pilot chuyển sang coach dashboard trước, không gửi trực tiếp cho toàn bộ học viên.

## Tổng kiểm tra trước khi sang `02-solution/`

| Hạng mục | Xong? |
|---|---|
| Chỉ rõ 1 nhóm người + 1 khoảnh khắc cụ thể | X |
| Pain có số hoặc kế hoạch lấy số, nói rõ số từ đâu | X |
| Có baseline hoặc cách đo baseline + chỉ số có ngưỡng | X |
| Owner giả định xác nhận đúng vấn đề | X |
