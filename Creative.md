# Theo dõi góp ý và cải tiến qua ba Sprint – RikkeiAssist

*Người đề xuất: Thu Hà, Scrum Master. Cùng thống nhất với Product Owner Minh Anh và 5 Developers.*

**Nguyên tắc thiết kế:** một bảng nhẹ cho góp ý, một bảng nhẹ cho Improvement. Hai bảng chỉ nối với nhau ở một chỗ duy nhất: cùng được xem lại trong hai sự kiện riêng. Sprint Review xem bảng góp ý, Sprint Retrospective xem bảng Improvement. Không thêm cuộc họp mới, không gộp hai sự kiện.

---

## Phần 1 – Chu trình theo dõi

### 1.1 Đường đi của một góp ý (Sprint Review → Product Backlog)

```
[1] Ghi nhận ──► [2] Làm rõ ──► [3] Gộp trùng & kiểm tra xung đột ──► [4] PO quyết định xử lý
 Thu Hà          Minh Anh           Minh Anh + Thu Hà                      Minh Anh
 (Review)    (cuối Review / trước       (trước Refinement)                       │
              Refinement)                                                        ▼
[6] Phản hồi người góp ý ◄── [5] Sắp xếp trong Product Backlog ◄── PBI xác nhận / Để theo dõi / Không làm (có lý do)
   Minh Anh                          Minh Anh                          
 (Review Sprint sau)             (Refinement)
```

| Bước | Việc làm | Ai cập nhật | Trạng thái sau bước |
| --- | --- | --- | --- |
| 1. Ghi nhận | Ghi nguyên văn lời góp ý, nguồn, Sprint. Không diễn giải lại. | Thu Hà (trong Sprint Review) | **Mới** |
| 2. Làm rõ | Hỏi người góp ý để biết: vấn đề thật là gì, ngưỡng/số liệu, rủi ro. Thiếu thông tin thì đánh dấu, không bỏ qua. | Minh Anh | **Cần làm rõ** hoặc **Đã làm rõ** |
| 3. Gộp trùng, kiểm tra xung đột | Gộp theo ý định (không theo câu chữ), giữ nguyên mã gốc. Gắn nhãn nếu mâu thuẫn với góp ý khác. | Minh Anh + Thu Hà | Gắn **Nhóm G-xx** / **Xung đột** |
| 4. Quyết định xử lý | PO chọn một: đưa vào xem xét Product Backlog (có PBI), Để theo dõi, hoặc Không làm (ghi lý do). Liên kết PBI phải được **xác nhận** (bỏ dấu ?). | Minh Anh | **Đã đưa vào xem xét PB** / **Để theo dõi** / **Không làm** |
| 5. Sắp xếp | PBI được xếp thứ tự trong Product Backlog theo giá trị và rủi ro. | Minh Anh (với Developers đánh giá khả thi) | Trạng thái của PBI |
| 6. Phản hồi | Báo lại người góp ý kết quả ở Sprint Review sau. Đây là lần kiểm tra của góp ý. | Minh Anh, Thu Hà ghi | Góp ý **Đã phản hồi** |

**Điểm quan trọng:** “Đã tiếp nhận” không phải trạng thái. Một góp ý chỉ được coi là tiến lên khi có thông tin làm rõ hoặc có quyết định của PO. Đưa vào xem xét Product Backlog **không** có nghĩa là cam kết sẽ làm.

### 1.2 Đường đi của một Improvement (Sprint Retrospective → kiểm tra ở Sprint sau)

```
Retro Sprint N                                         Trong Sprint N+1                      Retro Sprint N+1
[1] Nhận diện vấn đề nội bộ ──► [2] Chọn Improvement ──► [3] Thực hiện & ghi bằng chứng ──► [4] Kiểm tra bằng chứng ──► [5] Quyết định
    Cả Scrum Team                 Cả Scrum Team             Người theo dõi (Developers)           Cả Scrum Team            Cả Scrum Team
    Thu Hà ghi                    Thu Hà ghi                (cập nhật tại Daily Scrum)           Thu Hà ghi               Thu Hà ghi
                                                                                                                              │
                                       Đóng (đạt) / Giữ mở (nêu bước tiếp) / Điều chỉnh / Dừng (nêu lý do) ◄──────────────────┘
                                                       ▲ nếu Giữ mở hoặc Điều chỉnh: quay lại bước 3 cho Sprint N+2
```

| Bước | Việc làm | Ai cập nhật |
| --- | --- | --- |
| 1. Nhận diện | Nêu vấn đề nội bộ (quy trình, kỹ thuật, phối hợp). Không trộn với góp ý sản phẩm, không nêu tên người. | Cả Scrum Team, Thu Hà ghi |
| 2. Chọn Improvement | Chọn ít (1–3). Mỗi cái ghi: **dấu hiệu thành công đo được**, **bằng chứng sẽ xem**, **người theo dõi**, **Retro kiểm tra lần đầu**. | Cả Scrum Team, Thu Hà ghi |
| 3. Thực hiện, ghi bằng chứng | Đưa việc cần làm vào Sprint Backlog nếu cần. Người theo dõi chỉ giữ số liệu/bằng chứng, **không chịu chỉ tiêu cá nhân**. | Developers (người theo dõi) |
| 4. Kiểm tra | Đầu Retro Sprint sau: xem bằng chứng, kết luận **Có tác động / Chưa đủ / Không tác động**. | Cả Scrum Team |
| 5. Quyết định | Đóng (đạt mục tiêu) / Giữ mở / Điều chỉnh / Dừng có lý do. Ghi lý do và ngày. | Cả Scrum Team, Thu Hà ghi |

### 1.3 Nhịp dùng bảng (không thêm họp)

- **Sprint Review:** dành một phần ngắn trong thời lượng sẵn có để xem **bảng góp ý**: góp ý mới, góp ý còn “Cần làm rõ”, kết quả phản hồi cho người góp ý. Người tham gia là Scrum Team và các bên liên quan, đúng như hiện tại.
- **Sprint Retrospective:** dành một phần ngắn để xem **bảng Improvement**: Improvement đến hạn kiểm tra, vấn đề nội bộ lặp lại. Chỉ Scrum Team tham gia.
- Bảng góp ý không được dùng để bàn vấn đề nội bộ, và bảng Improvement không được dùng để bàn góp ý của khách hàng/CSKH.
- Chỉ **thêm dòng** để ghi trạng thái mới; không sửa hay xóa dòng cũ, để lịch sử lần theo được.

---

## Phần 2 – Bảng theo dõi

Mỗi bảng có hai lớp: (a) **dòng hiện tại** của mỗi mục, (b) **nhật ký theo Sprint**, chỉ thêm dòng, không sửa dòng cũ.

### 2.1 Bảng góp ý

**Cột:** Mã | Nguồn | Nội dung (nguyên văn) | Sprint ghi nhận | Trạng thái | Thông tin còn thiếu | Rủi ro / xung đột | Nhóm | Liên kết PBI | PBI đã xác nhận? (Có/Chưa) | Quyết định của PO | Người cập nhật, ngày | Việc kế tiếp

**Mẫu điền cho F-11-04 (nhật ký Sprint 11–13):**

| Thời điểm | Trạng thái | Thông tin đã biết / còn thiếu | Liên kết PBI | Người cập nhật | Việc kế tiếp |
| --- | --- | --- | --- | --- | --- |
| Sprint 11 Review | Mới → **Cần làm rõ** | Nguồn: Trưởng nhóm CSKH. Nội dung: chuyển người sớm hơn khi AI không chắc chắn. **Chưa rõ ngưỡng** (thế nào là “không chắc”?). | Không có | Thu Hà ghi; Minh Anh nhận việc làm rõ | Minh Anh hỏi Trưởng nhóm CSKH về ngưỡng trước Refinement |
| Sprint 12 Review | **Cần làm rõ** (giữ nguyên) | Dữ liệu không cho thấy ngưỡng đã được làm rõ. Ghi chú “quá 1 Sprint chưa làm rõ”. Xuất hiện F-12-11 (chủ cửa hàng muốn tự động hóa 90%): gắn nhãn **Xung đột**. | Không có | Thu Hà | Minh Anh đặt buổi làm rõ với cả hai bên (CSKH và chủ cửa hàng) |
| Sprint 13 Review | **Cần làm rõ**, gộp **Nhóm G-01** | F-13-05 (nhân viên CSKH ca tối) cùng ý, khác câu chữ, đều chưa rõ ngưỡng. Hai nguồn, hai Sprint. Mã gốc F-11-04 và F-13-05 giữ nguyên. | Không có | Minh Anh, Thu Hà | Sau khi làm rõ ngưỡng, PO quyết định: có đưa vào xem xét Product Backlog không. Đây mới là đề xuất, chưa phải cam kết |

### 2.2 Bảng Improvement

**Cột:** Mã | Sprint đề ra | Vấn đề nội bộ | Improvement | Dấu hiệu thành công (đo được) | Bằng chứng cần xem | Người theo dõi | Retro kiểm tra lần đầu | Kết quả kiểm tra | Quyết định | Lý do, ngày

**Mẫu điền cho IM-11-02 (nhật ký Sprint 11–13):**

| Thời điểm | Bằng chứng | Kết quả kiểm tra | Quyết định | Người ghi |
| --- | --- | --- | --- | --- |
| Sprint 11 Retro (đề ra) | Mức nền: Integration Test đầu tiên chạy ở **Ngày 8**. Improvement: cấp đủ quyền môi trường thử nghiệm từ Ngày 1 và chạy Integration Test khi PBI đầu tiên sẵn sàng. Người theo dõi: Developers (nên ghi tên một Developer giữ số liệu). Dấu hiệu thành công *(đề xuất, cả đội xác nhận)*: Integration Test đầu tiên không muộn hơn Ngày 5. Kiểm tra: Retro Sprint 12. | Chưa đến hạn | **Mở** | Thu Hà |
| Sprint 12 Retro (kiểm tra lần 1) | Integration Test đầu tiên ở **Ngày 7** | **Chưa đủ**: sớm hơn 1 ngày, chưa đạt dấu hiệu | **Giữ mở**; làm rõ nguyên nhân: quyền có thật sự được cấp từ Ngày 1 không, PBI đầu tiên sẵn sàng ngày mấy | Thu Hà |
| Sprint 13 Retro (kiểm tra lần 2) | Integration Test đầu tiên ở **Ngày 8** | **Chưa tạo tác động**: trở về mức nền | **Giữ mở và điều chỉnh**: tách thành hai phần (cấp quyền Ngày 1; PBI đầu tiên sẵn sàng sớm) để biết phần nào không chạy | Thu Hà |

**Đọc nhanh dữ liệu ba Sprint (để Review và Retro dùng):**

| Sprint | Ghi nhận | Đã hỏi rõ | Đã đưa vào xem xét PB | Improvement mới | Improvement còn mở |
| --- | --- | --- | --- | --- | --- |
| 11 | 12 | 5 (42%) | 3 (25%) | 3 | 2 |
| 12 | 15 | 7 (47%) | 6 (40%) | 2 | 3 |
| 13 | 18 | 10 (56%) | 5 (28%) | 2 | 4 |

Số góp ý tăng nhưng tỉ lệ được hỏi rõ chỉ nhích dần, và số Improvement còn mở tăng 2 → 3 → 4. Hai con số này cho thấy việc theo dõi đang thiếu, và là lý do cần chu trình ở Phần 1.

---

## Phần 3 – Quy tắc xử lý

### Tình huống 1 – Chủ cửa hàng muốn tăng tự động hóa, nhân viên CSKH muốn chuyển người sớm

- Cả hai là góp ý hợp lệ. Ghi nguyên văn cả hai, **không chọn bên** ngay trong Sprint Review và **không hứa** với ai.
- F-12-11 đang “chưa ghi rủi ro”: bắt buộc bổ sung rủi ro (ví dụ AI trả lời sai khi chính sách chưa chốt) và hỏi rõ “90%” nghĩa là gì (90% cuộc hội thoại? loại câu hỏi nào?). F-11-04 và F-13-05 cần làm rõ ngưỡng “không chắc”.
- Gắn nhãn **Xung đột** nối F-12-11 với nhóm G-01 (F-11-04 + F-13-05). F-12-07 (không trả lời đồ điện tử khi chính sách chưa chốt) là góp ý liên quan, ghi chung để PO nhìn đủ bức tranh.
- Minh Anh làm rõ với cả hai bên, Developers đánh giá khả thi. PO quyết định thứ tự trong Product Backlog dựa trên giá trị và rủi ro, rồi **giải thích lý do** cho cả hai bên ở Sprint Review sau. Có thể đề xuất một PBI nhỏ để xác định ngưỡng trước, vì cả hai góp ý đều cần ngưỡng này.

### Tình huống 2 – Góp ý lặp với câu chữ khác, và liên kết PBI-52 còn dấu hỏi

- **Gộp theo ý định, không theo câu chữ.** F-11-04 (Sprint 11) và F-13-05 (Sprint 13) cùng ý: gộp vào Nhóm G-01, giữ nguyên cả hai mã và nguồn, ghi “xuất hiện ở 2 Sprint, 2 nguồn”. Không xóa dòng nào. Trước khi gộp, PO xác nhận với người góp ý rằng hai câu cùng ý.
- Liên kết có dấu hỏi (F-12-07 – PBI-52?) có trạng thái **Chưa xác nhận**. Nó **không** được tính vào số “đã đưa vào xem xét Product Backlog”.
- Minh Anh mở PBI-52 đối chiếu với F-12-07 trước Refinement tới. Nếu đúng: bỏ dấu ?, ghi người xác nhận và ngày. Nếu không: ghi “không liên kết”, rồi quyết định tạo PBI mới hoặc để theo dõi.

### Tình huống 3 – “Mọi góp ý là đã tiếp nhận” và “đóng mọi Improvement quá một Sprint”

**Về góp ý:** không dùng trạng thái “đã tiếp nhận”. Báo cáo theo đúng trạng thái: Mới / Cần làm rõ / Đã làm rõ / Đã đưa vào xem xét PB (có PBI xác nhận) / Để theo dõi / Không làm (có lý do). Ví dụ Sprint 13: 18 ghi nhận, 10 đã hỏi rõ, 5 đã đưa vào xem xét, nên còn 8 chưa làm rõ. Con số này được nêu thẳng ở Review thay vì gói thành “đã tiếp nhận”.

**Về Improvement:** một Improvement chỉ đóng khi (a) đạt dấu hiệu thành công có bằng chứng, hoặc (b) Scrum Team quyết định dừng vì không còn phù hợp, ghi lý do và ngày. **Thời gian mở không phải lý do đóng.** Mở từ 2 Sprint trở lên chỉ là tín hiệu bắt buộc đem ra thảo luận ở Retro. Bảng gọn là kết quả của việc xử lý đúng, không phải mục tiêu.

| Mã | Bằng chứng hiện có | Áp dụng quy tắc | Quyết định đề xuất cho Retro Sprint 13 |
| --- | --- | --- | --- |
| IM-11-02 | Integration Test đầu tiên: Ngày 8 → 7 → 8, chưa cải thiện. Vấn đề vẫn còn thật. | Không đạt mục tiêu và không có lý do dừng, nên **không đóng**. | **Giữ mở, điều chỉnh**: tách hai phần, kiểm tra nguyên nhân thật, đặt dấu hiệu rõ (không muộn hơn Ngày 5). Nếu Sprint 14 vẫn không đổi, đổi cách làm chứ không đóng. |
| IM-12-04 | Kênh đã ngừng thí điểm, không còn dùng. | Đủ lý do (b): không còn phù hợp. Đây là **dừng**, không phải “hoàn thành”, và không tính là có tạo tác động. | **Dừng** bằng quyết định của Scrum Team, ghi lý do và ngày. Gia Huy xác nhận trước rằng không còn khách nào dùng kênh này. Nếu lỗi có thể lặp lại ở kênh khác, ghi thành vấn đề mới. |
| IM-13-03 | Hai phiên Pairing, thời gian tái hiện giảm; mới kiểm tra một lần. | Mới đề ra ở Sprint 13, nên chưa quá một Sprint. Một lần kiểm tra và chưa có con số cụ thể là chưa đủ để đóng. | **Giữ mở**: ghi thời gian tái hiện trước và sau; kiểm tra lại ở Retro Sprint 14. Nếu giảm ổn định thì đóng (đạt). |

### Tiêu chí đo được sau 3 Sprint tới

> Ít nhất **2 Improvement** được đóng với kết quả **“đạt dấu hiệu thành công”**, mỗi cái có bằng chứng số liệu ở ít nhất 2 Sprint liên tiếp. Ví dụ: ngày chạy Integration Test đầu tiên không muộn hơn Ngày 5 trong 2 Sprint liên tiếp.

Tiêu chí này chỉ đạt khi có thay đổi thật trong cách làm việc. Việc Review và Retro diễn ra đúng lịch hay bảng được cập nhật đều không làm nó đạt, và đóng Improvement vì để lâu hay vì dừng không được tính.

---

## Giữ ranh giới và sự an toàn khi nói thẳng

- Review và Retro giữ nguyên mục tiêu, người tham gia, thời lượng. Hai bảng không thay thế hai sự kiện, chỉ là chỗ ghi quyết định.
- Góp ý là đầu vào cho Product Backlog, quyền quyết định thuộc PO. Improvement thuộc cả Scrum Team và không phải chỉ tiêu cá nhân; người theo dõi chỉ giữ bằng chứng.
- Vấn đề nội bộ ghi theo hiện tượng, không ghi tên người. Khi thông tin chưa đủ thì đánh dấu và làm rõ, không sửa hay xóa lịch sử để báo cáo đẹp hơn.
