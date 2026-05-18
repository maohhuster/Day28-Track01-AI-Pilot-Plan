---
title: 00 — Context (bối cảnh nhóm + track)
section: Day 28 — điền 1 lần đầu buổi, dùng lại cho mọi lần hỏi AI
format: Nhóm 3
time: Điền ~5 phút đầu buổi
---

# 00-context.md — Context nhóm + track

## 1. Bối cảnh AI20k

Khóa **AI Thực Chiến** có ~500 học viên (sinh viên năm cuối + người đi làm), đang chuẩn bị cho giai đoạn 6 tuần thực chiến sau Day 28. Lab này do track Product làm. Hoạt động cả khóa nằm trên Discord, LMS, lớp live, lab, quiz, nộp bài và coaching.

Lãnh đạo chương trình muốn xây **AI20k Learning OS** — một hệ công cụ AI hỗ trợ học và vận hành khóa. Nhóm không pitch xây toàn bộ hệ thống, mà bóc tách Track 1 thành các use case độc lập và chọn một Quick Win đủ nhỏ để pilot.

## 2. Track của nhóm

- **Track số / tên**: Track 1 — Personalized Learning Path / Lộ trình học cá nhân hóa
- **Big Ask — chép nguyên văn câu yêu cầu trong track card**:

```text
Hệ thống cá nhân hóa lộ trình học cho từng học viên dựa trên mục tiêu, level, tiến độ, điểm yếu, hành vi học.
```

- **Công cụ lớn này phục vụ ai**: Học viên là người dùng đầu tiên; coach và instructor là người review/giám sát.
- **2 Red Flag đáng lo nhất**:
  1. Cá nhân hóa giả: chỉ đổi tên học viên nhưng khuyến nghị gần như giống nhau.
  2. Khuyến nghị quá nhiều gây quá tải, hoặc dùng dữ liệu nhạy cảm khi chưa có consent rõ.

## 3. Ràng buộc mọi track phải tôn trọng

- **Privacy** — data học viên/submission/Discord nhạy cảm; trong lab dùng data mẫu/giả định, nói rõ dùng cái gì.
- **Human review** — output rủi ro cao phải có người review, AI không tự quyết việc quan trọng.
- **Citation** — trả lời dựa trên tài liệu khóa thì phải có nguồn; thiếu nguồn thì nói "không biết", không bịa.
- **Budget nhỏ** — ưu tiên tool/API có sẵn, prototype nhanh, không xây platform lớn.
- **Formative ≠ summative** — feedback/chấm bằng AI là formative, chưa phải điểm chính thức nếu chưa có người calibrate.
- **Adoption** — tool không ai dùng = $0 dù accuracy 99%.
- **Pilot đủ nhỏ** — chạy được trong bối cảnh khóa hiện tại.

## 4. Ghi chú thêm

- Phạm vi nhóm chọn: không xây toàn bộ Learning OS; pilot chỉ tạo **checklist/lộ trình bù cá nhân sau D28** cho một nhóm học viên trước giai đoạn 6 tuần thực chiến.
- Dữ liệu lab dùng: bài nộp D28, self-assessment 5 câu, tiến độ LMS, điểm quiz/rubric nếu có. Số liệu trong bài là giả định để lập kế hoạch, cần xác nhận bằng baseline tuần 1.
- Thành viên nhóm: Nguyễn Đức Mạnh (2A202600151) phụ trách Frame; Hoàng Quang Thắng (2A202600069) phụ trách Solution; Lê Quang Minh (2A202600381) phụ trách Pilot Plan + pitch.
