# Day 11 SVM/360 Fisheye Lab — Nhóm Ranadal

Repo này là **điểm vào chung** của bài nộp nhóm Day 11 (SVM/360 Fisheye Lab). Bài làm thật (nhãn, export, báo cáo)
nằm trong repo cá nhân của từng thành viên để giữ nguyên đường dẫn ảnh và quan hệ giữa các file — repo này chỉ
tổng hợp và trỏ tới bằng chứng. Chi tiết phân vai, bàn giao từng pha, và bất đồng đã xử lý xem ở [TEAMMATES.md](TEAMMATES.md).

## Thành viên

| Họ và tên | Vai trò trong bài | Slice | Repo cá nhân |
|---|---|---|---|
| Lý Hồng Phúc *(đại diện nộp)* | Annotator + QA + Diagnostician trên slice của mình | `B1-mid` | https://github.com/phuclhAi/K4-DAY11-LyHongPhuc-2A202602221 |
| Nhi | Annotator + QA + Diagnostician trên slice của mình | `B3-center` | [Điền link repo cá nhân của Nhi] |
| Tuấn | Annotator + QA + Diagnostician trên slice của mình | `B4-dense` | [Điền link repo cá nhân của Tuấn] |

Mỗi người tự thực hiện đủ ba vai (Annotator → QA → Diagnostician) trên slice của chính mình qua P2–P4; vòng QA mù
ở P3 đổi bài chéo theo `submission/00_setup/team.json` sinh ra từ lệnh `mode --members phuc,nhi,tuan`.

## Bằng chứng theo từng người (tại commit chốt)

| Người | `manifest.json` | Bản nhãn đã khoá | QA review | Rework/delta | Exit ticket | Commit chốt |
|---|---|---|---|---|---|---|
| Phúc | [manifest.json](https://github.com/phuclhAi/K4-DAY11-LyHongPhuc-2A202602221/blob/main/submission/manifest.json) | [r1_craft/annotations.xml](https://github.com/phuclhAi/K4-DAY11-LyHongPhuc-2A202602221/blob/main/submission/r1_craft/annotations.xml) · [lock.txt](https://github.com/phuclhAi/K4-DAY11-LyHongPhuc-2A202602221/blob/main/submission/r1_craft/lock.txt) | [qa_review.md](https://github.com/phuclhAi/K4-DAY11-LyHongPhuc-2A202602221/blob/main/submission/r2_qa/qa_review.md) (QA bài Tuấn) | [rework/delta.md](https://github.com/phuclhAi/K4-DAY11-LyHongPhuc-2A202602221/blob/main/submission/rework/delta.md) | [50_exit_ticket.md](https://github.com/phuclhAi/K4-DAY11-LyHongPhuc-2A202602221/blob/main/submission/50_exit_ticket.md) | `67784af` |
| Nhi | [Điền] | [Điền] | [Điền] | [Điền] | [Điền] | [Điền] |
| Tuấn | [Điền] | [Điền] | [Điền] | [Điền] | [Điền] | [Điền] |

`check` gate: chỉ mới xác nhận repo của **Phúc** đạt `✓ Hồ sơ hình thức đầy đủ` (`failed_gates` rỗng trong
`manifest.json`). Nhi và Tuấn cần tự chạy `python3 lab11.py check` trong repo thực hành của mình, xử lý lỗi nếu có,
commit/push, rồi cập nhật cột "Commit chốt" ở trên — kết quả check của một người **không đại diện cho cả nhóm**.

## Cách nhóm chia việc

- Cả ba dùng chung danh sách tên `phuc,nhi,tuan` qua `mode --members ... --self <tên>` để công cụ tự chia slice
  (`B1-mid`, `B3-center`, `B4-dense`) và vòng QA.
- P0–P2: mỗi người tự làm slice của mình (setup, calibration C0, gán nhãn, self-QC, khoá) trong repo riêng.
- P3: đổi file đã khoá + mã khoá theo vòng — Nhi đã QA bài `B1-mid` của Phúc; Phúc đã QA bài `B4-dense` của Tuấn.
  [Điền — Tuấn QA bài của ai theo vòng, đã hoàn thành chưa].
- P4–P6: mỗi người tự chẩn đoán, rework và hoàn thiện báo cáo trên slice của mình trong repo riêng; thảo luận chung
  (nếu có) về guideline patch và kế hoạch bốn camera diễn ra qua kênh nội bộ, không gộp file `submission/` của các
  repo lại với nhau.

## Bất đồng đã xử lý và phần việc còn mở

Chi tiết đầy đủ (frame/object_ref, ý kiến từng bên, bằng chứng, quyết định) xem mục 4 của
[TEAMMATES.md](TEAMMATES.md#4-bất-đồng-và-phối-hợp). Tóm tắt:

- **Đã xử lý:** một box `Car` lấn sang `ThreeWheeler` trong slice `B1-mid` (rework theo đề nghị QA của Nhi); một
  nghi vấn trùng box `Bike` được giải quyết là "giữ nguyên" sau khi đối chiếu reference cho thấy QA (soát mù, chưa
  có reference) nghi ngờ nhầm.
- **Còn mở:** mẫu lỗi hệ thống `ThreeWheeler` bị gán nhầm thành `Car` (5 lần trong slice `B4-dense` của Tuấn) đã
  được escalate đề xuất patch guideline R04, nhưng **chưa có patch chính thức được duyệt** và Tuấn chưa xác nhận
  đã tự soát lại phần còn lại của slice mình.
- **Còn thiếu để hoàn thiện repo nhóm:** link repo cá nhân + commit chốt của Nhi và Tuấn, MSSV của cả ba, xác nhận
  `check` exit 0 từ Nhi và Tuấn.

## Trước khi nộp

1. Nhi và Tuấn chạy `python3 lab11.py check` trong repo riêng, sửa lỗi nếu có, commit và push.
2. Đại diện (Phúc) mở lại từng link trong bảng trên, đối chiếu slice/vòng QA/mã khoá/bằng chứng, xác nhận cả ba
   repo cá nhân và repo nhóm này đều **Public**.
3. Cập nhật `TEAMMATES.md` (các ô `[Điền]` còn lại) và bảng "Bằng chứng theo từng người" ở trên với link/commit
   thật của Nhi và Tuấn.
4. Commit và push hai file này (`README.md`, `TEAMMATES.md`) — **không** chạy `lab11.py check` trong repo nhóm vì
   repo này không có `lab11.py`/`submission/` đầy đủ, công cụ đó chỉ chạy trong repo thực hành.
5. Gửi link repo nhóm (`https://github.com/phuclhAi/K4-DAY11-Ranadal`) qua kênh lớp công bố — không cần từng thành
   viên nộp thêm lượt cá nhân cho cùng bài nhóm, trừ khi giảng viên yêu cầu khác.
