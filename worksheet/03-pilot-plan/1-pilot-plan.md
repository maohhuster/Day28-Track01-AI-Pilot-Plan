---
artifact: 7 — AI Pilot Plan core
bai-tap: Pilot Plan — cam kết hai chiều: xin – hứa – đo – dừng
phase: Double Diamond vòng 2 · ◇ giãn → ◆ siết
time: ~10 phút
input: 02-solution/2-FINAL-solution.md · 00-context.md · prompts/06-pilot-plan-challenge.md
nop-cuoi: Không — file trung gian
---

# 1 — AI Pilot Plan core

## 10 mục core

1. **Tóm vấn đề**: Sau D28, học viên và coach thiếu một cách nhanh, có bằng chứng, để biết từng học viên cần ôn gì trước 6 tuần thực chiến.

2. **Cách làm + lý do**: Dùng hướng Boost: LLM/API sẵn + rubric/concept map/tài liệu AI20k để sinh checklist cá nhân có citation, vì pilot cần chứng minh adoption/quality trước khi xây platform lớn.

3. **Scope pilot**:
   - Đối tượng: 30-80 học viên Track Product sau D28, ưu tiên một cohort nhỏ trước nếu thiếu coach review.
   - Thời gian: 3 tuần pilot, đủ để đo baseline, gửi checklist, theo dõi action và phản hồi.
   - Phase: tuần 1 baseline + mapping; tuần 2 chạy batch nhỏ + coach review; tuần 3 gửi rộng hơn + đo adoption/quality.

4. **Người**:
   - Nhóm làm: Nguyễn Đức Mạnh (2A202600151) phụ trách Frame; Hoàng Quang Thắng (2A202600069) phụ trách Solution; Lê Quang Minh (2A202600381) phụ trách Pilot Plan + pitch.
   - Review output rủi ro cao: coach Track Product.
   - Quyết approve/dừng: instructor/owner chương trình, dựa trên metric và exit criteria.

5. **Data**:
   - Dùng: bài nộp D28, rubric/gate feedback, self-assessment 5 câu, mapping concept -> tài liệu D2/D27/D28, LMS/quiz nếu được cấp quyền.
   - Privacy: ẩn tên khi test; chỉ dùng dữ liệu cần thiết; không dùng Discord private data nếu chưa có consent.
   - Citation: mỗi action phải trỏ về tài liệu/template/ngày học; thiếu nguồn thì ghi "không đủ dữ liệu".

6. **Budget**:
   - API/tool: 🧮 2-5 USD/tuần cho batch nhỏ, đo thực tế tuần 1.
   - Thời gian nhóm: 6-8 giờ setup mapping + prompt + sheet; 2-3 giờ chạy và sửa batch.
   - Thời gian coach: 2 giờ review 15-20 checklist mẫu và toàn bộ low-confidence.
   - Hạng mục ẩn: training học viên/coach 30 phút, logging lỗi, maintenance mapping concept 1 giờ/tuần.

7. **Timeline + cổng giữa phase**:
   - Tuần 1 — Chuẩn hóa concept map, tạo self-assessment, đo baseline. Cổng: có >=10 concept và >=20 học viên trả lời baseline.
   - Tuần 2 — Chạy batch 15-20 học viên, coach review. Cổng: >=80% checklist pass review, không có lỗi privacy/citation nghiêm trọng.
   - Tuần 3 — Gửi checklist cho cohort pilot, đo mở/tick action/phản hồi. Cổng: đạt metric adoption + quality thì đề xuất mở rộng.

8. **Metrics**:

| Metric | Đo bằng gì · ai đo | Baseline | Ngưỡng đạt |
|---|---|---|---|
| Học viên biết 3 việc cần ôn trước project | Survey 3 câu trước/sau · nhóm đo | 🧮 30-40% trả lời rõ | >=70% sau khi nhận checklist |
| Checklist có chất lượng theo coach | Coach review rubric 4 tiêu chí | 0 vì chưa có tool | >=80% checklist pass, coach sửa <20% nội dung chính |
| Adoption: học viên mở và tick ít nhất 1 action | LMS/Sheet/Discord form · nhóm đo | 0 | >=60% mở, >=40% tick 1 action trong 7 ngày |
| Citation đúng | Audit 20 checklist · coach/nhóm đo | 0 | >=95% action có nguồn đúng |

Leading indicator trong 1-2 tuần: batch 15-20 checklist đầu tiên đạt >=80% pass coach review và không phát sinh lỗi privacy/citation nghiêm trọng.

9. **Exit criteria**:

| Mức | Điều kiện | Hành động | Ai có quyền dừng |
|---|---|---|---|
| Cảnh báo | <60% checklist pass coach review, hoặc học viên phản hồi "không đúng điểm yếu" >30% | Dừng mở rộng, sửa concept map/prompt, tăng review | Coach lead |
| Nghiêm trọng | Có rò rỉ dữ liệu nhạy cảm, khuyến nghị thiếu citation hàng loạt, hoặc AI gán nhãn gây hiểu sai năng lực học viên | Dừng pilot ngay, thu hồi checklist, audit log, báo owner | Instructor/owner chương trình |
| Không đáng mở rộng | Adoption <30% mở checklist sau 7 ngày dù đã nhắc 1 lần | Không mở rộng; chuyển sang coach dashboard hoặc đổi kênh nhận | Instructor/owner chương trình |

Exit criteria chặn 2 red flag chính: cá nhân hóa giả bị bắt qua quality/adoption; overload bị chặn bằng giới hạn 3 action và phản hồi học viên.

10. **Adoption**:
   - Người dùng đầu tiên: 15-20 học viên sau D28 trong batch nhỏ, sau đó mở rộng đến 30-80 học viên Track Product nếu qua cổng.
   - Workflow đổi ở đâu: sau khi nộp D28, học viên nhận checklist trong LMS/Sheet link; trong 7 ngày tick action và phản hồi "đúng/chưa đúng".
   - Train/support: 10 phút hướng dẫn trong Discord/LMS; coach có form báo lỗi checklist.
   - Nếu không ai dùng: không đổ thêm công build; chuyển output thành coach dashboard hoặc tích hợp vào feedback D28 thay vì gửi riêng.

## Tự phản biện

- Budget còn thiếu chi phí vận hành mapping concept nếu chương trình thay đổi tài liệu; đã ghi maintenance 1 giờ/tuần.
- Exit criteria có người dừng cụ thể: coach lead dừng mở rộng, instructor/owner dừng pilot.
- Giả định quan trọng nhất: học viên sẽ đọc checklist nếu action ít và đúng. Nếu sai, nhóm đo adoption và chuyển sang workflow coach dùng trước.

## Tổng kiểm tra trước khi sang `2-FINAL-pitch.md`

| Hạng mục | Xong? |
|---|---|
| Tóm vấn đề trong 1 câu | X |
| Budget tách hạng mục, không "miscellaneous" | X |
| Metric có baseline + ngưỡng + ai đo | X |
| Exit criteria có người có quyền thực thi | X |
| Adoption: chỉ rõ ai dùng đầu tiên | X |
