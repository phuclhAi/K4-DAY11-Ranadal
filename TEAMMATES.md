# Thành viên và phân vai — Day11 SVM 360 Fisheye

## 1. Thông tin nhóm

- Khóa/lớp: K4 [Xác nhận lại]
- Tên nhóm: Ranadal
- Repo Public: https://github.com/phuclhAi/K4-DAY11-Ranadal
- Máy giữ hồ sơ chính / người quản lý: Phúc
- Slice chung lấy từ `mode.json`: `phuc,nhi,tuan` → phuc=`B1-mid`, nhi=`B3-center`, tuan=`B4-dense`
- Tên định danh dùng cho `--self`: `phuc`, `nhi`, `tuan`
- Kênh trao đổi nội bộ: [Điền — ví dụ Zalo nhóm/Messenger]
- Đại diện nộp: Phúc [MSSV: xác nhận lại — nghi là `2A202602221` theo tên repo cá nhân]
- Commit chốt bài (repo nhóm): [Điền sau khi commit + push repo nhóm]

Mỗi thành viên tự thực hiện **đủ ba vai** (Annotator → QA → Diagnostician) trên slice của chính mình qua P2–P4;
không chia cố định một người chỉ vẽ/một người chỉ QA. Bảng dưới liệt kê từng người theo đúng cột vlearn yêu cầu.

## 2. Thành viên và bằng chứng đóng góp

| Họ và tên | MSSV | Tên dùng trong `mode` | Slice được giao | QA bài của ai | Phần việc và bằng chứng | Link repo cá nhân | Commit nộp |
|---|---|---|---|---|---|---|---|
| Lý Hồng Phúc | `2A202602221` [xác nhận lại] | `phuc` | `B1-mid` | QA bài `B4-dense` của Tuấn (mã khoá `AEBB-D053`) | Gán nhãn + self-QC 9 mục ([`r1_craft/selfqc.md`](https://github.com/phuclhAi/K4-DAY11-LyHongPhuc-2A202602221/blob/main/submission/r1_craft/selfqc.md)) · khoá bản đầu mã `4B7F-EB27` ([`r1_craft/lock.txt`](https://github.com/phuclhAi/K4-DAY11-LyHongPhuc-2A202602221/blob/main/submission/r1_craft/lock.txt)) · QA bài Tuấn ([`r2_qa/qa_review.md`](https://github.com/phuclhAi/K4-DAY11-LyHongPhuc-2A202602221/blob/main/submission/r2_qa/qa_review.md)) · chẩn đoán 30+ dòng ([`findings.csv`](https://github.com/phuclhAi/K4-DAY11-LyHongPhuc-2A202602221/blob/main/submission/findings.csv)) · rework mã `2335-08B8` ([`rework/delta.md`](https://github.com/phuclhAi/K4-DAY11-LyHongPhuc-2A202602221/blob/main/submission/rework/delta.md)) · [`exit ticket`](https://github.com/phuclhAi/K4-DAY11-LyHongPhuc-2A202602221/blob/main/submission/50_exit_ticket.md) | https://github.com/phuclhAi/K4-DAY11-LyHongPhuc-2A202602221 | `67784af` |
| Nhi | [Điền MSSV] | `nhi` | `B3-center` | [Điền — ai QA bài của Nhi theo vòng team.json] | Đã QA bài `B1-mid` của Phúc (nhận xét về R02/R03/R04, gửi qua chat — Phúc đã trích dẫn trong [`findings.csv`](https://github.com/phuclhAi/K4-DAY11-LyHongPhuc-2A202602221/blob/main/submission/findings.csv) round `r2_qa` slice `B1-mid`) · [Điền phần gán nhãn/chẩn đoán của chính Nhi trên `B3-center`, kèm link] | [Điền link repo cá nhân của Nhi] | [Điền commit nộp của Nhi] |
| Tuấn | [Điền MSSV] | `tuan` | `B4-dense` | [Điền — ai QA bài của Tuấn theo vòng team.json, có vẻ là Phúc dựa trên mã `AEBB-D053` đã dùng] | Đã khoá bài `B4-dense` (mã `AEBB-D053`), được Phúc QA phát hiện mẫu lỗi `ThreeWheeler`→`Car` lặp lại 5 lần (xem [`20_guideline_patch.md`](https://github.com/phuclhAi/K4-DAY11-LyHongPhuc-2A202602221/blob/main/submission/20_guideline_patch.md), [`30_escalation_ticket.md`](https://github.com/phuclhAi/K4-DAY11-LyHongPhuc-2A202602221/blob/main/submission/30_escalation_ticket.md)) · [Điền phần Tuấn tự chẩn đoán/phản hồi escalation trên repo của Tuấn, kèm link] | [Điền link repo cá nhân của Tuấn] | [Điền commit nộp của Tuấn] |

## 3. Bàn giao theo pha

| Mốc | Người giao → nhận | File / commit / mã khóa | Người nhận đã kiểm gì? | Trạng thái / vướng mắc |
|---|---|---|---|---|
| P0 · Chốt môi trường và vai | Phúc chạy `mode --members phuc,nhi,tuan` | `mode.json`, `team.json`, slice mỗi người | Mỗi người tự xác nhận slice của mình qua `status` | Xong |
| P2 · Khóa bản đầu | Phúc → Nhi (để QA); Tuấn → Phúc (để QA) | Phúc: ZIP + `4B7F-EB27` (`B1-mid`); Tuấn: ZIP `tuan.zip` + `AEBB-D053` (`B4-dense`) | Phúc đã chạy `lab11.py qa` xác nhận mã khớp bài Tuấn | Xong (Phúc); [Điền — Nhi/Tuấn tự xác nhận bên repo của mình] |
| P3 · Chốt QA mù | Nhi → Phúc (review `B1-mid`); Phúc → Tuấn (review `B4-dense`, cần gửi lại `qa_review.md`) | Nhi gửi `qa_review (1) phuc.md` qua chat; Phúc tạo `r2_qa/qa_review.md` (5 nhận xét `R04`) trong repo mình | Phúc đã đọc và trích dẫn nhận xét của Nhi vào `findings.csv`; Phúc cần gửi lại `qa_review.md` cho Tuấn | Đã gửi cho Phúc; [Điền — Phúc gửi lại kết quả QA cho Tuấn chưa] |
| P4 · Quyết định sửa | Phúc tự chẩn đoán `B1-mid` | `findings.csv` round `r3_diag`, `40_decision_log.csv` (4 dòng, 1 `escalated`) | Đối chiếu `compare.md`/`model_compare.md`; giải quyết 3 nhận xét QA của Nhi (1 rework, 1 giữ nguyên có bằng chứng, 1 giải toả nghi vấn class) | Xong (Phúc); [Điền — Nhi/Tuấn tự chẩn đoán slice của mình] |
| P5 · Kiểm bản sửa | Phúc sửa box `L9` (`adasind_034080.jpg`) | ZIP sau sửa + mã `2335-08B8`, `rework/delta.md` | Số liệu zone không đổi (đã giải thích lý do trong `delta.md`) | Xong (Phúc) |
| P6 · Chốt nộp | Phúc → cả nhóm | `manifest.json`, commit `67784af`, push repo cá nhân | `check` báo `✓ Hồ sơ hình thức đầy đủ` | Xong (Phúc); [Điền — Nhi/Tuấn push repo cá nhân của mình + cập nhật bảng] |

## 4. Bất đồng và phối hợp

- Một ca đã phân xử: `adasind_034080.jpg`, box `Car` (`L9`) lấn sang thân `ThreeWheeler` (`L10`) phía trước. Ý kiến Nhi (QA, rule R02): cần thu mép trái box. Đối chiếu `compare.md` (so với teaching reference) xác nhận cùng vấn đề (`BOX_GEOMETRY`) — hai nguồn hội tụ. Quyết định: rework, kéo mép trái từ x≈466 vào x≈510. Bằng chứng: [`40_decision_log.csv`](https://github.com/phuclhAi/K4-DAY11-LyHongPhuc-2A202602221/blob/main/submission/40_decision_log.csv) dòng 2, [`rework/delta.md`](https://github.com/phuclhAi/K4-DAY11-LyHongPhuc-2A202602221/blob/main/submission/rework/delta.md).
- Một ca khác: Nhi nghi hai box `Bike` (`L2`/`L6`, cùng frame) là trùng lặp (rule R03). Đối chiếu teaching reference cho thấy cả hai box đều khớp riêng biệt với 2 box reference khác nhau — không nằm trong danh sách `SPURIOUS`. Quyết định: giữ nguyên, không sửa (`keep_with_reason`), vì bằng chứng sau khi có reference cho thấy đây nhiều khả năng là 2 vật thật mà Nhi không thể biết lúc soát mù. Bằng chứng: `40_decision_log.csv` dòng 3.
- Ca còn mở: Mẫu lỗi `ThreeWheeler`→`Car` lặp lại 5 lần trong bài `B4-dense` của Tuấn (phát hiện khi Phúc làm QA) đã được escalate lên `owner=guideline` (xem `30_escalation_ticket.md`), nhưng **chưa có patch rule chính thức được duyệt** và Tuấn **chưa xác nhận đã tự soát lại** các box `Car` còn lại trong slice của mình. Người theo dõi: Phúc (đã mở ticket) + Tuấn (cần tự kiểm). Phép kiểm tiếp theo: Tuấn chạy lại `qa`/`selfqc` trên slice của mình sau khi đọc `20_guideline_patch.md`.
- Đóng góp của từng người vào kế hoạch bốn camera (`45_sampling_plan.csv`, `46_gold_set_plan.md`) và exit ticket: [Điền — nhóm thảo luận chung ở P0/P6 hay từng người tự viết độc lập; mỗi người vẫn phải tự viết câu nhìn lại riêng trong `50_exit_ticket.md` của mình].
- Thay đổi phân công nếu có: Không đổi so với `mode.json` ban đầu.

## 5. Xác nhận trước khi nộp

- [x] Phúc xác nhận nhãn và export đúng phiên bản `B1-mid`: `lab11.py check` → `✓ Hồ sơ hình thức đầy đủ`, commit `67784af`.
- [ ] Nhi xác nhận đã QA độc lập trước reference và kiểm lại ca sửa: [Điền]
- [ ] Tuấn xác nhận nhãn và export đúng phiên bản `B4-dense`: [Điền]
- [ ] `manifest.json` của **cả ba** repo cá nhân tại commit chốt có `failed_gates` rỗng — hiện mới xác nhận được của Phúc.
- [ ] Repo nhóm và cả ba repo cá nhân đều Public.
- [ ] Đại diện (Phúc) đã push repo nhóm + gửi link qua kênh lớp công bố.

Chỉ đánh dấu việc đã kiểm thật — các ô `[ ]` còn lại cần Nhi/Tuấn tự xác nhận trước khi tick.
