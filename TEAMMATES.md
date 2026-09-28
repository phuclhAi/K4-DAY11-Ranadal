# Thành viên và phân vai — Day11 SVM 360 Fisheye

## 1. Thông tin nhóm

- Khóa/lớp: K4-L2
- Tên nhóm: Ranadal
- Repo Public: https://github.com/phuclhAi/K4-DAY11-Ranadal
- Máy giữ hồ sơ chính / người quản lý: Phúc
- Slice chung lấy từ `mode.json`: `phuc,nhi,tuan` → phuc=`B1-mid`, nhi=`B3-center`, tuan=`B4-dense`
- Tên định danh dùng cho `--self`: `phuc`, `nhi`, `tuan`
- Kênh trao đổi nội bộ: Nhóm ZALO
- Đại diện nộp: Lý Hồng Phúc, MSSV `2A202602221`
- Commit chốt bài (repo nhóm): [Điền sau khi push repo nhóm]

Mỗi thành viên tự thực hiện **đủ ba vai** (Annotator → QA → Diagnostician) trên slice của chính mình qua P2–P4;
không chia cố định một người chỉ vẽ/một người chỉ QA. Bảng dưới liệt kê từng người theo đúng cột vlearn yêu cầu.

## 2. Thành viên và bằng chứng đóng góp

| Họ và tên | MSSV | Tên dùng trong `mode` | Slice được giao | QA bài của ai | Phần việc và bằng chứng | Link repo cá nhân | Commit nộp |
|---|---|---|---|---|---|---|---|
| Lý Hồng Phúc | `2A202602221` | `phuc` | `B1-mid` | QA bài `B4-dense` của Tuân (mã khoá `AEBB-D053`) | Gán nhãn + self-QC 9 mục ([`r1_craft/selfqc.md`](https://github.com/phuclhAi/K4-L2-DAY11-LyHongPhuc-2A202602221-SVM-360-View/blob/main/submission/r1_craft/selfqc.md)) · khoá bản đầu mã `4B7F-EB27` ([`r1_craft/lock.txt`](https://github.com/phuclhAi/K4-L2-DAY11-LyHongPhuc-2A202602221-SVM-360-View/blob/main/submission/r1_craft/lock.txt)) · QA bài Tuân ([`r2_qa/qa_review.md`](https://github.com/phuclhAi/K4-L2-DAY11-LyHongPhuc-2A202602221-SVM-360-View/blob/main/submission/r2_qa/qa_review.md)) · chẩn đoán 30+ dòng ([`findings.csv`](https://github.com/phuclhAi/K4-L2-DAY11-LyHongPhuc-2A202602221-SVM-360-View/blob/main/submission/findings.csv)) · rework mã `2335-08B8` ([`rework/delta.md`](https://github.com/phuclhAi/K4-L2-DAY11-LyHongPhuc-2A202602221-SVM-360-View/blob/main/submission/rework/delta.md)) · [`exit ticket`](https://github.com/phuclhAi/K4-L2-DAY11-LyHongPhuc-2A202602221-SVM-360-View/blob/main/submission/50_exit_ticket.md) | https://github.com/phuclhAi/K4-L2-DAY11-LyHongPhuc-2A202602221-SVM-360-View | `8a9fadc` |
| Võ Lê Xuân Nhi | `2A202602202` | `nhi` | `B3-center` | QA bài `B1-mid` của Phúc (gửi qua chat, xem trích dẫn trong [`findings.csv`](https://github.com/phuclhAi/K4-L2-DAY11-LyHongPhuc-2A202602221-SVM-360-View/blob/main/submission/findings.csv) của Phúc) | Hoàn thành P0–P6: khoá `r1_craft` mã `673A-7072` ([`lock.txt`](https://github.com/XuanNhi183/K4-L2-DAY11-VoLeXuanNhi-2A202602202-SVM360-Fisheye-Lab-Student/blob/main/submission/r1_craft/lock.txt)) · đã QA bài `B1-mid` của Phúc (gửi qua chat, Phúc đã trích dẫn trong [`findings.csv`](https://github.com/phuclhAi/K4-L2-DAY11-LyHongPhuc-2A202602221-SVM-360-View/blob/main/submission/findings.csv) round `r2_qa` slice `B1-mid`) · rework mã `008A-1B71` phản hồi đúng nhận xét của Tuân — đổi `Car`→`Bus` ở frame `212280` và tách người dắt xe thành `Pedestrian`+`Bike` ở frame `167700` ([`40_decision_log.csv`](https://github.com/XuanNhi183/K4-L2-DAY11-VoLeXuanNhi-2A202602202-SVM360-Fisheye-Lab-Student/blob/main/submission/40_decision_log.csv) D03/D04) · escalate riêng 1 ca nghi ngờ `ego_body` của reference (D01) | https://github.com/XuanNhi183/K4-L2-DAY11-VoLeXuanNhi-2A202602202-SVM360-Fisheye-Lab-Student | `567c35e` |
| Phạm Nguyễn Tuân | `2A202602091` | `tuan` | `B4-dense` | QA bài `B3-center` của Nhi (mã `673A-7072`, xem [`qa_review.md`](https://github.com/phamnguyentuan0311/K4-L2-DAY11-PhamNguyenTuan-2A202602091-SVM360-Fisheye-Lab/blob/main/submission/r2_qa/qa_review.md) trong repo mình) | Hoàn thành đầy đủ P0–P6: `manifest.json` có `failed_gates: []` ([xem](https://github.com/phamnguyentuan0311/K4-L2-DAY11-PhamNguyenTuan-2A202602091-SVM360-Fisheye-Lab/blob/main/submission/manifest.json)) · khoá `r1_craft` ([`lock.txt`](https://github.com/phamnguyentuan0311/K4-L2-DAY11-PhamNguyenTuan-2A202602091-SVM360-Fisheye-Lab/blob/main/submission/r1_craft/lock.txt)) · đã QA bài `B3-center` của Nhi mã `673A-7072` ([`r2_qa/qa_review.md`](https://github.com/phamnguyentuan0311/K4-L2-DAY11-PhamNguyenTuan-2A202602091-SVM360-Fisheye-Lab/blob/main/submission/r2_qa/qa_review.md)) · rework ([`rework/delta.md`](https://github.com/phamnguyentuan0311/K4-L2-DAY11-PhamNguyenTuan-2A202602091-SVM360-Fisheye-Lab/blob/main/submission/rework/delta.md)) · được Phúc QA phát hiện mẫu lỗi `ThreeWheeler`→`Car` lặp lại 5 lần, đã escalate (xem `20_guideline_patch.md`, `30_escalation_ticket.md` trong repo Phúc) — **Tuân chưa xác nhận đã tự soát lại theo escalation này**. | https://github.com/phamnguyentuan0311/K4-L2-DAY11-PhamNguyenTuan-2A202602091-SVM360-Fisheye-Lab | `bbe1a8d` |

## 3. Bàn giao theo pha

| Mốc | Người giao → nhận | File / commit / mã khóa | Người nhận đã kiểm gì? | Trạng thái / vướng mắc |
|---|---|---|---|---|
| P0 · Chốt môi trường và vai | Phúc chạy `mode --members phuc,nhi,tuan` | `mode.json`, `team.json`, slice mỗi người | Mỗi người tự xác nhận slice của mình qua `status` | Xong |
| P2 · Khóa bản đầu | Phúc → Nhi (để QA); Tuân → Phúc (để QA); Nhi → Tuân (để QA) | Phúc: ZIP + `4B7F-EB27` (`B1-mid`); Tuân: ZIP + `AEBB-D053` (`B4-dense`); Nhi: ZIP + `673A-7072` (`B3-center`) | Cả ba đã chạy `lab11.py qa` xác nhận mã khớp | Xong cả ba |
| P3 · Chốt QA mù | Nhi → Phúc (review `B1-mid`); Phúc → Tuân (review `B4-dense`); Tuân → Nhi (review `B3-center`) — đúng vòng khép kín theo `team.json` | Nhi gửi `qa_review (1) phuc.md` qua chat; Phúc tạo `r2_qa/qa_review.md` (5 nhận xét `R04`) trong repo mình; Tuân tạo `r2_qa/qa_review.md` (mã `673A-7072`) trong repo Tuân, review bài Nhi | Phúc đã đọc và trích dẫn nhận xét của Nhi vào `findings.csv`. Tuân phát hiện Nhi dùng **polygon thay vì bounding box** để gán nhãn phương tiện (sai quy trình, xem mục 4) — Nhi đã đọc và rework | Xong cả ba |
| P4 · Quyết định sửa | Cả ba tự chẩn đoán slice của mình | Phúc: `findings.csv` round `r3_diag`, `40_decision_log.csv` (4 dòng, 1 `escalated`); Tuân: `r3_diag/` đầy đủ; Nhi: `40_decision_log.csv` 4 dòng (D01 escalated) | Phúc: giải quyết 3 nhận xét QA của Nhi. Nhi: giải quyết nhận xét QA của Tuân (D03 đổi `Car`→`Bus`, D04 tách Pedestrian/Bike) + tự escalate 1 ca nghi ngờ reference (D01, ego_body frame `167700`) | Xong cả ba |
| P5 · Kiểm bản sửa | Phúc sửa box `L9` (`adasind_034080.jpg`); Tuân và Nhi cũng đã rework | Phúc: ZIP sau sửa + mã `2335-08B8`, `rework/delta.md`. Tuân: `rework/annotations-v2.xml`, `lock2.txt`. Nhi: rework mã `008A-1B71` | Số liệu zone không đổi ở phía Phúc (đã giải thích lý do trong `delta.md`) | Xong cả ba |
| P6 · Chốt nộp | Cả ba → nhau | Phúc: `manifest.json`, commit `8a9fadc`. Tuân: `manifest.json` (`failed_gates: []`), commit `bbe1a8d`. Nhi: `manifest.json` (`failed_gates: []`), commit `567c35e` | `check` cả ba đều báo đạt | Xong cả ba |

## 4. Bất đồng và phối hợp

- Một ca đã phân xử: `adasind_034080.jpg`, box `Car` (`L9`) lấn sang thân `ThreeWheeler` (`L10`) phía trước. Ý kiến Nhi (QA, rule R02): cần thu mép trái box. Đối chiếu `compare.md` (so với teaching reference) xác nhận cùng vấn đề (`BOX_GEOMETRY`) — hai nguồn hội tụ. Quyết định: rework, kéo mép trái từ x≈466 vào x≈510. Bằng chứng: [`40_decision_log.csv`](https://github.com/phuclhAi/K4-L2-DAY11-LyHongPhuc-2A202602221-SVM-360-View/blob/main/submission/40_decision_log.csv) dòng 2, [`rework/delta.md`](https://github.com/phuclhAi/K4-L2-DAY11-LyHongPhuc-2A202602221-SVM-360-View/blob/main/submission/rework/delta.md).
- Một ca khác: Nhi nghi hai box `Bike` (`L2`/`L6`, cùng frame) là trùng lặp (rule R03). Đối chiếu teaching reference cho thấy cả hai box đều khớp riêng biệt với 2 box reference khác nhau — không nằm trong danh sách `SPURIOUS`. Quyết định: giữ nguyên, không sửa (`keep_with_reason`), vì bằng chứng sau khi có reference cho thấy đây nhiều khả năng là 2 vật thật mà Nhi không thể biết lúc soát mù. Bằng chứng: `40_decision_log.csv` dòng 3.
- Ca đã xử lý (3): Tuân QA bài `B3-center` của Nhi (mã `673A-7072`) và phát hiện Nhi dùng **polygon để gán nhãn phương tiện** (`Bike`, `Truck`) thay vì bounding box, cộng thêm nghi class `Car`/`Bus` ở frame `212280` và người dắt xe chưa tách ở frame `167700` (xem `r2_qa/qa_review.md` trong repo Tuân). Nhi đã đọc và rework: đổi `Car`→`Bus` (`40_decision_log.csv` D03) và tách `Pedestrian`+`Bike` cho người dắt xe (D04), khoá lại mã `008A-1B71`.
- Ca còn mở: Mẫu lỗi `ThreeWheeler`→`Car` lặp lại 5 lần trong bài `B4-dense` của Tuân (phát hiện khi Phúc làm QA) đã được escalate lên `owner=guideline` (xem `30_escalation_ticket.md`), nhưng **chưa có patch rule chính thức được duyệt** và Tuân **chưa xác nhận đã tự soát lại** các box `Car` còn lại trong slice của mình. Người theo dõi: Phúc (đã mở ticket) + Tuân (cần tự kiểm). Phép kiểm tiếp theo: Tuân chạy lại `qa`/`selfqc` trên slice của mình sau khi đọc `20_guideline_patch.md`.
- Ca Nhi tự mở (chưa thuộc bất đồng nội bộ nhóm): Nhi escalate 1 ca nghi ngờ chính **teaching reference** đặt sai vùng `ego_body` ở frame `167700` (`40_decision_log.csv` D01, ảnh `screenshots/167700_ego_body_review.png`) — chuyển Lab Coach xử lý, không phải bất đồng giữa thành viên trong nhóm.
- Đóng góp của từng người vào kế hoạch bốn camera (`45_sampling_plan.csv`, `46_gold_set_plan.md`) và exit ticket: mỗi người tự viết trong repo riêng (không gộp).
- Thay đổi phân công nếu có: Không đổi so với `mode.json` ban đầu.

## 5. Xác nhận trước khi nộp

- [x] Phúc xác nhận nhãn và export đúng phiên bản `B1-mid`: `lab11.py check` → `✓ Hồ sơ hình thức đầy đủ`, commit `8a9fadc`.
- [x] Nhi xác nhận đã QA độc lập trước reference và kiểm lại ca sửa: khoá `r1_craft` mã `673A-7072`, rework mã `008A-1B71`; chạy `check` trực tiếp trên bản mới nhất báo đạt.
- [x] Tuân xác nhận nhãn và export đúng phiên bản `B4-dense`: `manifest.json` có `failed_gates: []`, commit `bbe1a8d`.
- [x] `manifest.json` của **cả ba** repo cá nhân tại commit chốt có `failed_gates` rỗng.
- [ ] Repo nhóm và cả ba repo cá nhân đều Public — đã xác nhận repo Phúc, Nhi, Tuân Public (mở được); repo nhóm cần bật Public trước khi gửi link.
- [ ] Đại diện (Phúc) đã push repo nhóm + gửi link qua kênh lớp công bố — **chưa push**.

Chỉ đánh dấu việc đã kiểm thật.
