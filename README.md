# Day 11 SVM/360 Fisheye Lab — Nhóm Ranadal

Repo này là **điểm vào chung** của bài nộp nhóm Day 11 (SVM/360 Fisheye Lab). Bài làm thật (nhãn, export, báo cáo)
nằm trong repo cá nhân của từng thành viên để giữ nguyên đường dẫn ảnh và quan hệ giữa các file — repo này chỉ
tổng hợp và trỏ tới bằng chứng. Chi tiết phân vai, bàn giao từng pha, và bất đồng đã xử lý xem ở [TEAMMATES.md](TEAMMATES.md).

## Thành viên

| Họ và tên | Vai trò trong bài | Slice | Repo cá nhân |
|---|---|---|---|
| Lý Hồng Phúc *(đại diện nộp)* | Annotator + QA + Diagnostician trên slice của mình — **hoàn thành P0–P6** | `B1-mid` | https://github.com/phuclhAi/K4-DAY11-LyHongPhuc-2A202602221 |
| Võ Lê Xuân Nhi | Annotator + QA + Diagnostician trên slice của mình — **mới xong P0, chưa khoá `r1_craft`** | `B3-center` | https://github.com/XuanNhi183/K4-L2-DAY11-VoLeXuanNhi-2A202602202-SVM360-Fisheye-Lab-Student |
| Phạm Nguyễn Tuấn | Annotator + QA + Diagnostician trên slice của mình — **hoàn thành P0–P6** | `B4-dense` | https://github.com/phamnguyentuan0311/K4-L2-DAY11-PhamNguyenTuan-2A202602091-SVM360-Fisheye-Lab |

Mỗi người tự thực hiện đủ ba vai (Annotator → QA → Diagnostician) trên slice của chính mình qua P2–P4; vòng QA mù
ở P3 đổi bài chéo theo `submission/00_setup/team.json` sinh ra từ lệnh `mode --members phuc,nhi,tuan`.

## Bằng chứng theo từng người (tại commit chốt)

| Người | `manifest.json` | Bản nhãn đã khoá | QA review | Rework/delta | Exit ticket | Commit chốt |
|---|---|---|---|---|---|---|
| Phúc | [manifest.json](https://github.com/phuclhAi/K4-DAY11-LyHongPhuc-2A202602221/blob/main/submission/manifest.json) | [r1_craft/annotations.xml](https://github.com/phuclhAi/K4-DAY11-LyHongPhuc-2A202602221/blob/main/submission/r1_craft/annotations.xml) · [lock.txt](https://github.com/phuclhAi/K4-DAY11-LyHongPhuc-2A202602221/blob/main/submission/r1_craft/lock.txt) | [qa_review.md](https://github.com/phuclhAi/K4-DAY11-LyHongPhuc-2A202602221/blob/main/submission/r2_qa/qa_review.md) (QA bài Tuấn) | [rework/delta.md](https://github.com/phuclhAi/K4-DAY11-LyHongPhuc-2A202602221/blob/main/submission/rework/delta.md) | [50_exit_ticket.md](https://github.com/phuclhAi/K4-DAY11-LyHongPhuc-2A202602221/blob/main/submission/50_exit_ticket.md) | `67784af` |
| Nhi | **chưa có** | **chưa khoá** — repo mới có file P0 | Đã QA bài Phúc qua chat (không phải file trong repo Nhi) | — | [Điền — kiểm xem Nhi đã viết chưa] | `b2cd962` *(chưa hoàn chỉnh)* |
| Tuấn | [manifest.json](https://github.com/phamnguyentuan0311/K4-L2-DAY11-PhamNguyenTuan-2A202602091-SVM360-Fisheye-Lab/blob/main/submission/manifest.json) (`failed_gates: []`) | [r1_craft/annotations.xml](https://github.com/phamnguyentuan0311/K4-L2-DAY11-PhamNguyenTuan-2A202602091-SVM360-Fisheye-Lab/blob/main/submission/r1_craft/annotations.xml) · [lock.txt](https://github.com/phamnguyentuan0311/K4-L2-DAY11-PhamNguyenTuan-2A202602091-SVM360-Fisheye-Lab/blob/main/submission/r1_craft/lock.txt) | [qa_review.md](https://github.com/phamnguyentuan0311/K4-L2-DAY11-PhamNguyenTuan-2A202602091-SVM360-Fisheye-Lab/blob/main/submission/r2_qa/qa_review.md) (QA bài Nhi) | [rework/delta.md](https://github.com/phamnguyentuan0311/K4-L2-DAY11-PhamNguyenTuan-2A202602091-SVM360-Fisheye-Lab/blob/main/submission/rework/delta.md) | [50_exit_ticket.md](https://github.com/phamnguyentuan0311/K4-L2-DAY11-PhamNguyenTuan-2A202602091-SVM360-Fisheye-Lab/blob/main/submission/50_exit_ticket.md) | `bbe1a8d` |

`check` gate: **Phúc và Tuấn** đạt `✓ Hồ sơ hình thức đầy đủ` (`failed_gates` rỗng trong `manifest.json`). **Nhi
chưa chạy/chưa commit `check`** — repo của Nhi ở commit mới nhất mới có các file P0, chưa có `p1_calib/`,
`r1_craft/`, `r2_qa/`, `r3_diag/`, `rework/`. Nhi cần hoàn thành phần fisheye, khoá `r1_craft`, chạy `check`, rồi
commit/push và cập nhật lại bảng này — kết quả check của Phúc/Tuấn **không đại diện cho phần của Nhi**.

## Cách nhóm chia việc

- Cả ba dùng chung danh sách tên `phuc,nhi,tuan` qua `mode --members ... --self <tên>` để công cụ tự chia slice
  (`B1-mid`, `B3-center`, `B4-dense`) và vòng QA.
- P0–P2: mỗi người tự làm slice của mình (setup, calibration C0, gán nhãn, self-QC, khoá) trong repo riêng.
  Phúc và Tuấn đã khoá xong; Nhi chưa khoá `r1_craft`.
- P3: vòng QA khép kín theo `team.json` — Nhi QA bài `B1-mid` của Phúc; Phúc QA bài `B4-dense` của Tuấn; Tuấn QA
  bài `B3-center` của Nhi. Cả ba chiều đều đã có bằng chứng (2 lưu trong repo, 1 gửi qua chat).
- P4–P6: Phúc và Tuấn đã tự chẩn đoán, rework và hoàn thiện báo cáo trên slice của mình, `check` exit 0 cả hai.
  Nhi chưa tới được các bước này vì chưa khoá bản đầu. Thảo luận chung (nếu có) về guideline patch và kế hoạch bốn
  camera diễn ra qua kênh nội bộ, không gộp file `submission/` của các repo lại với nhau.

## Bất đồng đã xử lý và phần việc còn mở

Chi tiết đầy đủ (frame/object_ref, ý kiến từng bên, bằng chứng, quyết định) xem mục 4 của
[TEAMMATES.md](TEAMMATES.md#4-bất-đồng-và-phối-hợp). Tóm tắt:

- **Đã xử lý:** một box `Car` lấn sang `ThreeWheeler` trong slice `B1-mid` (rework theo đề nghị QA của Nhi); một
  nghi vấn trùng box `Bike` được giải quyết là "giữ nguyên" sau khi đối chiếu reference cho thấy QA (soát mù, chưa
  có reference) nghi ngờ nhầm.
- **Còn mở (1):** mẫu lỗi hệ thống `ThreeWheeler` bị gán nhầm thành `Car` (5 lần trong slice `B4-dense` của Tuấn) đã
  được escalate đề xuất patch guideline R04, nhưng **chưa có patch chính thức được duyệt** và Tuấn chưa xác nhận
  đã tự soát lại phần còn lại của slice mình.
- **Còn mở (2):** Tuấn QA bài `B3-center` của Nhi và phát hiện Nhi **dùng polygon để gán nhãn phương tiện thay vì
  bounding box** — sai quy trình, ảnh hưởng tới việc đo tự động. Nhi chưa phản hồi hay sửa; repo Nhi hiện chưa có
  bản `r1_craft` đã khoá.
- **Còn thiếu để hoàn thiện repo nhóm:** MSSV chính xác của Phúc (đang suy từ tên repo), kênh liên lạc nội bộ,
  Nhi hoàn thành P1–P6 + `check` exit 0 + commit chốt trong repo của Nhi, xác nhận repo nhóm đã bật Public.

## Trước khi nộp

1. **Nhi hoàn thành phần fisheye còn lại** (P1–P6: khoá `r1_craft`, self-QC, mở reference, chẩn đoán, rework, báo
   cáo P6) trong repo cá nhân, đọc và phản hồi nhận xét QA của Tuấn (đặc biệt lỗi dùng polygon thay box), rồi chạy
   `python3 lab11.py check` tới khi đạt, commit và push.
2. Đại diện (Phúc) mở lại từng link trong bảng trên, đối chiếu slice/vòng QA/mã khoá/bằng chứng, xác nhận cả ba
   repo cá nhân và repo nhóm này đều **Public**.
3. Cập nhật `TEAMMATES.md` và bảng "Bằng chứng theo từng người" ở trên với commit chốt thật của Nhi sau khi xong
   bước 1; xác nhận lại MSSV của Phúc.
4. Commit và push hai file này (`README.md`, `TEAMMATES.md`) — **không** chạy `lab11.py check` trong repo nhóm vì
   repo này không có `lab11.py`/`submission/` đầy đủ, công cụ đó chỉ chạy trong repo thực hành.
5. Gửi link repo nhóm (`https://github.com/phuclhAi/K4-DAY11-Ranadal`) qua kênh lớp công bố — không cần từng thành
   viên nộp thêm lượt cá nhân cho cùng bài nhóm, trừ khi giảng viên yêu cầu khác.
