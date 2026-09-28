# Day 11 SVM/360 Fisheye Lab — Nhóm Ranadal

Repo này là **điểm vào chung** của bài nộp nhóm Day 11 (SVM/360 Fisheye Lab). Bài làm thật (nhãn, export, báo cáo)
nằm trong repo cá nhân của từng thành viên để giữ nguyên đường dẫn ảnh và quan hệ giữa các file — repo này chỉ
tổng hợp và trỏ tới bằng chứng. Chi tiết phân vai, bàn giao từng pha, và bất đồng đã xử lý xem ở [TEAMMATES.md](TEAMMATES.md).

## Thành viên

| Họ và tên | Vai trò trong bài | Slice | Repo cá nhân |
|---|---|---|---|
| Lý Hồng Phúc *(đại diện nộp)* | Annotator + QA + Diagnostician trên slice của mình — **hoàn thành P0–P6** | `B1-mid` | https://github.com/phuclhAi/K4-L2-DAY11-LyHongPhuc-2A202602221-SVM-360-View |
| Võ Lê Xuân Nhi | Annotator + QA + Diagnostician trên slice của mình — **hoàn thành P0–P6** | `B3-center` | https://github.com/XuanNhi183/K4-L2-DAY11-VoLeXuanNhi-2A202602202-SVM360-Fisheye-Lab-Student |
| Phạm Nguyễn Tuân | Annotator + QA + Diagnostician trên slice của mình — **hoàn thành P0–P6** | `B4-dense` | https://github.com/phamnguyentuan0311/K4-L2-DAY11-PhamNguyenTuan-2A202602091-SVM360-Fisheye-Lab |

Mỗi người tự thực hiện đủ ba vai (Annotator → QA → Diagnostician) trên slice của chính mình qua P2–P4; vòng QA mù
ở P3 đổi bài chéo theo `submission/00_setup/team.json` sinh ra từ lệnh `mode --members phuc,nhi,tuan`.

## Bằng chứng theo từng người (tại commit chốt)

| Người | `manifest.json` | Bản nhãn đã khoá | QA review | Rework/delta | Exit ticket | Commit chốt |
|---|---|---|---|---|---|---|
| Phúc | [manifest.json](https://github.com/phuclhAi/K4-L2-DAY11-LyHongPhuc-2A202602221-SVM-360-View/blob/main/submission/manifest.json) | [r1_craft/annotations.xml](https://github.com/phuclhAi/K4-L2-DAY11-LyHongPhuc-2A202602221-SVM-360-View/blob/main/submission/r1_craft/annotations.xml) · [lock.txt](https://github.com/phuclhAi/K4-L2-DAY11-LyHongPhuc-2A202602221-SVM-360-View/blob/main/submission/r1_craft/lock.txt) | [qa_review.md](https://github.com/phuclhAi/K4-L2-DAY11-LyHongPhuc-2A202602221-SVM-360-View/blob/main/submission/r2_qa/qa_review.md) (QA bài Tuân) | [rework/delta.md](https://github.com/phuclhAi/K4-L2-DAY11-LyHongPhuc-2A202602221-SVM-360-View/blob/main/submission/rework/delta.md) | [50_exit_ticket.md](https://github.com/phuclhAi/K4-L2-DAY11-LyHongPhuc-2A202602221-SVM-360-View/blob/main/submission/50_exit_ticket.md) | `8a9fadc` |
| Nhi | [manifest.json](https://github.com/XuanNhi183/K4-L2-DAY11-VoLeXuanNhi-2A202602202-SVM360-Fisheye-Lab-Student/blob/main/submission/manifest.json) (`failed_gates: []`) | [r1_craft/annotations.xml](https://github.com/XuanNhi183/K4-L2-DAY11-VoLeXuanNhi-2A202602202-SVM360-Fisheye-Lab-Student/blob/main/submission/r1_craft/annotations.xml) · [lock.txt](https://github.com/XuanNhi183/K4-L2-DAY11-VoLeXuanNhi-2A202602202-SVM360-Fisheye-Lab-Student/blob/main/submission/r1_craft/lock.txt) | [qa_review.md](https://github.com/phamnguyentuan0311/K4-L2-DAY11-PhamNguyenTuan-2A202602091-SVM360-Fisheye-Lab/blob/main/submission/r2_qa/qa_review.md) (Tuân QA bài Nhi, trong repo Tuân) | [rework/delta.md](https://github.com/XuanNhi183/K4-L2-DAY11-VoLeXuanNhi-2A202602202-SVM360-Fisheye-Lab-Student/blob/main/submission/rework/delta.md) | [50_exit_ticket.md](https://github.com/XuanNhi183/K4-L2-DAY11-VoLeXuanNhi-2A202602202-SVM360-Fisheye-Lab-Student/blob/main/submission/50_exit_ticket.md) | `567c35e` |
| Tuân | [manifest.json](https://github.com/phamnguyentuan0311/K4-L2-DAY11-PhamNguyenTuan-2A202602091-SVM360-Fisheye-Lab/blob/main/submission/manifest.json) (`failed_gates: []`) | [r1_craft/annotations.xml](https://github.com/phamnguyentuan0311/K4-L2-DAY11-PhamNguyenTuan-2A202602091-SVM360-Fisheye-Lab/blob/main/submission/r1_craft/annotations.xml) · [lock.txt](https://github.com/phamnguyentuan0311/K4-L2-DAY11-PhamNguyenTuan-2A202602091-SVM360-Fisheye-Lab/blob/main/submission/r1_craft/lock.txt) | [qa_review.md](https://github.com/phamnguyentuan0311/K4-L2-DAY11-PhamNguyenTuan-2A202602091-SVM360-Fisheye-Lab/blob/main/submission/r2_qa/qa_review.md) (QA bài Nhi) | [rework/delta.md](https://github.com/phamnguyentuan0311/K4-L2-DAY11-PhamNguyenTuan-2A202602091-SVM360-Fisheye-Lab/blob/main/submission/rework/delta.md) | [50_exit_ticket.md](https://github.com/phamnguyentuan0311/K4-L2-DAY11-PhamNguyenTuan-2A202602091-SVM360-Fisheye-Lab/blob/main/submission/50_exit_ticket.md) | `bbe1a8d` |

`check` gate: **cả ba** đều đạt `✓ Hồ sơ hình thức đầy đủ` với `manifest.json` có `failed_gates` rỗng tại commit
chốt.

## Cách nhóm chia việc

- Cả ba dùng chung danh sách tên `phuc,nhi,tuan` qua `mode --members ... --self <tên>` để công cụ tự chia slice
  (`B1-mid`, `B3-center`, `B4-dense`) và vòng QA.
- P0–P2: mỗi người tự làm slice của mình (setup, calibration C0, gán nhãn, self-QC, khoá) trong repo riêng. Cả ba
  đã khoá `r1_craft` xong.
- P3: vòng QA khép kín theo `team.json` — Nhi QA bài `B1-mid` của Phúc (qua chat); Phúc QA bài `B4-dense` của Tuân
  (trong repo); Tuân QA bài `B3-center` của Nhi (trong repo). Cả ba chiều đều có bằng chứng.
- P4–P6: cả ba đã tự chẩn đoán, rework và hoàn thiện báo cáo trên slice của mình. Thảo luận chung (nếu có) về
  guideline patch và kế hoạch bốn camera diễn ra qua kênh nội bộ, không gộp file `submission/` của các repo lại
  với nhau.

## Bất đồng đã xử lý và phần việc còn mở

Chi tiết đầy đủ (frame/object_ref, ý kiến từng bên, bằng chứng, quyết định) xem mục 4 của
[TEAMMATES.md](TEAMMATES.md#4-bất-đồng-và-phối-hợp). Tóm tắt:

- **Đã xử lý (1):** một box `Car` lấn sang `ThreeWheeler` trong slice `B1-mid` (rework theo đề nghị QA của Nhi);
  một nghi vấn trùng box `Bike` được giải quyết là "giữ nguyên" sau khi đối chiếu reference cho thấy QA (soát mù,
  chưa có reference) nghi ngờ nhầm.
- **Đã xử lý (2):** Tuân QA bài `B3-center` của Nhi, phát hiện Nhi dùng **polygon thay vì bounding box** để gán
  nhãn phương tiện, cộng thêm nghi class `Car`/`Bus` và một ca người dắt xe chưa tách. Nhi đã rework: đổi
  `Car`→`Bus` ở frame `212280`, tách `Pedestrian`+`Bike` ở frame `167700`.
- **Còn mở:** mẫu lỗi hệ thống `ThreeWheeler` bị gán nhầm thành `Car` (5 lần trong slice `B4-dense` của Tuân) đã
  được escalate đề xuất patch guideline R04, nhưng **chưa có patch chính thức được duyệt** và Tuân chưa xác nhận
  đã tự soát lại phần còn lại của slice mình.
- **Ca ngoài nhóm:** Nhi escalate riêng một nghi vấn về chính **teaching reference** (vị trí `ego_body` ở frame
  `167700` có thể sai) — chuyển Lab Coach xử lý, không phải bất đồng giữa các thành viên.
- **Còn thiếu để hoàn thiện repo nhóm:** xác nhận repo nhóm này đã bật Public trước khi gửi link.

## Trước khi nộp

1. Đại diện (Phúc) mở lại từng link trong bảng trên, đối chiếu slice/vòng QA/mã khoá/bằng chứng, xác nhận cả ba
   repo cá nhân và repo nhóm này đều **Public**.
2. Commit và push hai file này (`README.md`, `TEAMMATES.md`) — **không** chạy `lab11.py check` trong repo nhóm vì
   repo này không có `lab11.py`/`submission/` đầy đủ, công cụ đó chỉ chạy trong repo thực hành.
3. Gửi link repo nhóm (`https://github.com/phuclhAi/K4-DAY11-Ranadal`) qua kênh lớp công bố — không cần từng thành
   viên nộp thêm lượt cá nhân cho cùng bài nhóm, trừ khi giảng viên yêu cầu khác.
