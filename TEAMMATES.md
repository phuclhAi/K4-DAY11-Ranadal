# Thành viên và phân vai — Day11 SVM 360 Fisheye

## 1. Thông tin nhóm

- Khóa/lớp: K4-L2
- Tên nhóm: Ranadal
- Repo Public: https://github.com/phuclhAi/K4-DAY11-Ranadal
- Máy giữ hồ sơ chính / người quản lý: Phúc
- Slice chung lấy từ `mode.json`: `phuc,nhi,tuan` → phuc=`B1-mid`, nhi=`B3-center`, tuan=`B4-dense`
- Tên định danh dùng cho `--self`: `phuc`, `nhi`, `tuan`
- Kênh trao đổi nội bộ: [Điền — ví dụ Zalo nhóm/Messenger]
- Đại diện nộp: Lý Hồng Phúc, MSSV `2A202602221`
- Commit chốt bài (repo nhóm): [Điền sau khi push repo nhóm]

Mỗi thành viên tự thực hiện **đủ ba vai** (Annotator → QA → Diagnostician) trên slice của chính mình qua P2–P4;
không chia cố định một người chỉ vẽ/một người chỉ QA. Bảng dưới liệt kê từng người theo đúng cột vlearn yêu cầu.

## 2. Thành viên và bằng chứng đóng góp

| Họ và tên | MSSV | Tên dùng trong `mode` | Slice được giao | QA bài của ai | Phần việc và bằng chứng | Link repo cá nhân | Commit nộp |
|---|---|---|---|---|---|---|---|
| Lý Hồng Phúc | `2A202602221` | `phuc` | `B1-mid` | QA bài `B4-dense` của Tuấn (mã khoá `AEBB-D053`) | Gán nhãn + self-QC 9 mục ([`r1_craft/selfqc.md`](https://github.com/phuclhAi/K4-L2-DAY11-LyHongPhuc-2A202602221-SVM-360-View/blob/main/submission/r1_craft/selfqc.md)) · khoá bản đầu mã `4B7F-EB27` ([`r1_craft/lock.txt`](https://github.com/phuclhAi/K4-L2-DAY11-LyHongPhuc-2A202602221-SVM-360-View/blob/main/submission/r1_craft/lock.txt)) · QA bài Tuấn ([`r2_qa/qa_review.md`](https://github.com/phuclhAi/K4-L2-DAY11-LyHongPhuc-2A202602221-SVM-360-View/blob/main/submission/r2_qa/qa_review.md)) · chẩn đoán 30+ dòng ([`findings.csv`](https://github.com/phuclhAi/K4-L2-DAY11-LyHongPhuc-2A202602221-SVM-360-View/blob/main/submission/findings.csv)) · rework mã `2335-08B8` ([`rework/delta.md`](https://github.com/phuclhAi/K4-L2-DAY11-LyHongPhuc-2A202602221-SVM-360-View/blob/main/submission/rework/delta.md)) · [`exit ticket`](https://github.com/phuclhAi/K4-L2-DAY11-LyHongPhuc-2A202602221-SVM-360-View/blob/main/submission/50_exit_ticket.md) | https://github.com/phuclhAi/K4-L2-DAY11-LyHongPhuc-2A202602221-SVM-360-View | `67784af` |
| Võ Lê Xuân Nhi | `2A202602202` | `nhi` | `B3-center` | Tuấn QA bài của Nhi (mã `673A-7072`, xem [`qa_review.md`](https://github.com/phamnguyentuan0311/K4-L2-DAY11-PhamNguyenTuan-2A202602091-SVM360-Fisheye-Lab/blob/main/submission/r2_qa/qa_review.md) trong repo Tuấn) | Đã QA bài `B1-mid` của Phúc (nhận xét R02/R03/R04, gửi qua chat — Phúc đã trích dẫn trong [`findings.csv`](https://github.com/phuclhAi/K4-L2-DAY11-LyHongPhuc-2A202602221-SVM-360-View/blob/main/submission/findings.csv) round `r2_qa` slice `B1-mid`). **Chưa hoàn thành phần gán nhãn của chính mình**: repo cá nhân tại commit mới nhất (`b2cd962`) mới có các file P0 (`sensor_context.md`, `findings.csv` rỗng khung, sampling plan...), **chưa commit** `p1_calib/`, `r1_craft/`, `r2_qa/`, `r3_diag/`, `rework/` hay `manifest.json`. Tuấn QA (mù) trên bản Nhi gửi riêng đã chỉ ra vấn đề: dùng polygon để gán nhãn phương tiện thay vì bounding box (sai quy trình R02), và một số ca nghi `ThreeWheeler`/`occluded` cần soát lại. | https://github.com/XuanNhi183/K4-L2-DAY11-VoLeXuanNhi-2A202602202-SVM360-Fisheye-Lab-Student | `b2cd962` *(chưa phải bản hoàn chỉnh — cần Nhi tự cập nhật)* |
| Phạm Nguyễn Tuấn | `2A202602091` | `tuan` | `B4-dense` | Phúc QA bài của Tuấn (mã `AEBB-D053`) | Hoàn thành đầy đủ P0–P6: `manifest.json` có `failed_gates: []` ([xem](https://github.com/phamnguyentuan0311/K4-L2-DAY11-PhamNguyenTuan-2A202602091-SVM360-Fisheye-Lab/blob/main/submission/manifest.json)) · khoá `r1_craft` ([`lock.txt`](https://github.com/phamnguyentuan0311/K4-L2-DAY11-PhamNguyenTuan-2A202602091-SVM360-Fisheye-Lab/blob/main/submission/r1_craft/lock.txt)) · đã QA bài `B3-center` của Nhi mã `673A-7072` ([`r2_qa/qa_review.md`](https://github.com/phamnguyentuan0311/K4-L2-DAY11-PhamNguyenTuan-2A202602091-SVM360-Fisheye-Lab/blob/main/submission/r2_qa/qa_review.md)) · rework ([`rework/delta.md`](https://github.com/phamnguyentuan0311/K4-L2-DAY11-PhamNguyenTuan-2A202602091-SVM360-Fisheye-Lab/blob/main/submission/rework/delta.md)) · được Phúc QA phát hiện mẫu lỗi `ThreeWheeler`→`Car` lặp lại 5 lần, đã escalate (xem `20_guideline_patch.md`, `30_escalation_ticket.md` trong repo Phúc) — **Tuấn chưa xác nhận đã tự soát lại theo escalation này**. | https://github.com/phamnguyentuan0311/K4-L2-DAY11-PhamNguyenTuan-2A202602091-SVM360-Fisheye-Lab | `bbe1a8d` |

## 3. Bàn giao theo pha

| Mốc | Người giao → nhận | File / commit / mã khóa | Người nhận đã kiểm gì? | Trạng thái / vướng mắc |
|---|---|---|---|---|
| P0 · Chốt môi trường và vai | Phúc chạy `mode --members phuc,nhi,tuan` | `mode.json`, `team.json`, slice mỗi người | Mỗi người tự xác nhận slice của mình qua `status` | Xong |
| P2 · Khóa bản đầu | Phúc → Nhi (để QA); Tuấn → Phúc (để QA); Nhi → Tuấn (để QA) | Phúc: ZIP + `4B7F-EB27` (`B1-mid`); Tuấn: ZIP + `AEBB-D053` (`B4-dense`); Nhi: ZIP + `673A-7072` (`B3-center`) | Phúc và Tuấn đã chạy `lab11.py qa` xác nhận mã khớp | Xong (Phúc, Tuấn); Nhi **chưa khoá `r1_craft` trong repo của mình** (không có `lock.txt`/`manifest.json` ở commit `b2cd962`) dù đã gửi bản để Tuấn QA riêng — cần xác nhận Nhi đã khoá bằng file nào |
| P3 · Chốt QA mù | Nhi → Phúc (review `B1-mid`); Phúc → Tuấn (review `B4-dense`); Tuấn → Nhi (review `B3-center`) — đúng vòng khép kín theo `team.json` | Nhi gửi `qa_review (1) phuc.md` qua chat; Phúc tạo `r2_qa/qa_review.md` (5 nhận xét `R04`) trong repo mình; Tuấn tạo `r2_qa/qa_review.md` (mã `673A-7072`) trong repo Tuấn, review bài Nhi | Phúc đã đọc và trích dẫn nhận xét của Nhi vào `findings.csv`. Tuấn phát hiện Nhi dùng **polygon thay vì bounding box** để gán nhãn phương tiện (sai quy trình, xem mục 4) | Cả 3 chiều QA đã có bằng chứng (2 trong repo Tuấn/Phúc, 1 qua chat); Nhi cần tự đọc và phản hồi nhận xét của Tuấn trong repo của Nhi |
| P4 · Quyết định sửa | Phúc và Tuấn tự chẩn đoán slice của mình | Phúc: `findings.csv` round `r3_diag`, `40_decision_log.csv` (4 dòng, 1 `escalated`); Tuấn: `r3_diag/` đầy đủ trong repo Tuấn | Phúc: đối chiếu `compare.md`/`model_compare.md`, giải quyết 3 nhận xét QA của Nhi (1 rework, 1 giữ nguyên có bằng chứng, 1 giải toả nghi vấn class) | Xong (Phúc, Tuấn); Nhi chưa tới bước này (chưa có `r1_craft` đã khoá để mở reference) |
| P5 · Kiểm bản sửa | Phúc sửa box `L9` (`adasind_034080.jpg`); Tuấn cũng đã rework (xem `rework/delta.md` repo Tuấn) | Phúc: ZIP sau sửa + mã `2335-08B8`, `rework/delta.md`. Tuấn: `rework/annotations-v2.xml`, `lock2.txt` | Số liệu zone không đổi ở phía Phúc (đã giải thích lý do trong `delta.md`) | Xong (Phúc, Tuấn) |
| P6 · Chốt nộp | Phúc và Tuấn → cả nhóm | Phúc: `manifest.json`, commit `67784af`. Tuấn: `manifest.json` (`failed_gates: []`), commit `bbe1a8d` | `check` của cả hai đều báo đạt | Xong (Phúc, Tuấn); Nhi cần hoàn thành P1–P6 trong repo của mình rồi mới chạy `check` |

## 4. Bất đồng và phối hợp

- Một ca đã phân xử: `adasind_034080.jpg`, box `Car` (`L9`) lấn sang thân `ThreeWheeler` (`L10`) phía trước. Ý kiến Nhi (QA, rule R02): cần thu mép trái box. Đối chiếu `compare.md` (so với teaching reference) xác nhận cùng vấn đề (`BOX_GEOMETRY`) — hai nguồn hội tụ. Quyết định: rework, kéo mép trái từ x≈466 vào x≈510. Bằng chứng: [`40_decision_log.csv`](https://github.com/phuclhAi/K4-L2-DAY11-LyHongPhuc-2A202602221-SVM-360-View/blob/main/submission/40_decision_log.csv) dòng 2, [`rework/delta.md`](https://github.com/phuclhAi/K4-L2-DAY11-LyHongPhuc-2A202602221-SVM-360-View/blob/main/submission/rework/delta.md).
- Một ca khác: Nhi nghi hai box `Bike` (`L2`/`L6`, cùng frame) là trùng lặp (rule R03). Đối chiếu teaching reference cho thấy cả hai box đều khớp riêng biệt với 2 box reference khác nhau — không nằm trong danh sách `SPURIOUS`. Quyết định: giữ nguyên, không sửa (`keep_with_reason`), vì bằng chứng sau khi có reference cho thấy đây nhiều khả năng là 2 vật thật mà Nhi không thể biết lúc soát mù. Bằng chứng: `40_decision_log.csv` dòng 3.
- Ca còn mở (1): Mẫu lỗi `ThreeWheeler`→`Car` lặp lại 5 lần trong bài `B4-dense` của Tuấn (phát hiện khi Phúc làm QA) đã được escalate lên `owner=guideline` (xem `30_escalation_ticket.md`), nhưng **chưa có patch rule chính thức được duyệt** và Tuấn **chưa xác nhận đã tự soát lại** các box `Car` còn lại trong slice của mình. Người theo dõi: Phúc (đã mở ticket) + Tuấn (cần tự kiểm). Phép kiểm tiếp theo: Tuấn chạy lại `qa`/`selfqc` trên slice của mình sau khi đọc `20_guideline_patch.md`.
- Ca còn mở (2): Tuấn QA bài `B3-center` của Nhi (mã `673A-7072`) và phát hiện **Nhi dùng polygon để gán nhãn phương tiện** (`Bike`, `Truck`) thay vì bounding box — vi phạm quy trình vẽ box (không thuộc rule `ignore_region`), cộng thêm 1 ca nghi class `Truck`/`ThreeWheeler` và 1 ca nghi `occluded` cần soát lại (xem `r2_qa/qa_review.md` trong repo Tuấn). Đây là lỗi cấu trúc nghiêm trọng hơn các ca khác vì ảnh hưởng đến việc đo đạc tự động (`compare`/`local-quality` không đọc được polygon như box). **Nhi chưa phản hồi hay sửa** — repo của Nhi hiện chưa có `r1_craft/annotations.xml` được khoá.
- Đóng góp của từng người vào kế hoạch bốn camera (`45_sampling_plan.csv`, `46_gold_set_plan.md`) và exit ticket: mỗi người tự viết trong repo riêng (không gộp); [Điền — xác nhận Nhi đã viết `45_sampling_plan.csv`/`46_gold_set_plan.md` của mình dù chưa xong phần fisheye].
- Thay đổi phân công nếu có: Không đổi so với `mode.json` ban đầu.

## 5. Xác nhận trước khi nộp

- [x] Phúc xác nhận nhãn và export đúng phiên bản `B1-mid`: `lab11.py check` → `✓ Hồ sơ hình thức đầy đủ`, commit `67784af`.
- [ ] Nhi xác nhận đã QA độc lập trước reference và kiểm lại ca sửa: **chưa** — repo Nhi chưa có `r1_craft` đã khoá, chưa mở được `reference`.
- [x] Tuấn xác nhận nhãn và export đúng phiên bản `B4-dense`: `manifest.json` có `failed_gates: []`, commit `bbe1a8d`.
- [ ] `manifest.json` của **cả ba** repo cá nhân tại commit chốt có `failed_gates` rỗng — đã xác nhận Phúc và Tuấn; **Nhi chưa có file này**.
- [ ] Repo nhóm và cả ba repo cá nhân đều Public — đã xác nhận repo Phúc, Nhi, Tuấn Public (mở được); repo nhóm cần bật Public trước khi gửi link.
- [ ] Đại diện (Phúc) đã push repo nhóm + gửi link qua kênh lớp công bố — **chưa push**, đang chờ Nhi hoàn thành trước.

Chỉ đánh dấu việc đã kiểm thật — các ô `[ ]` còn lại cần Nhi/Tuấn tự xác nhận trước khi tick.
