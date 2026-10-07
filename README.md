

## Dữ liệu đối chiếu

Đường lý tưởng = 40 − 4 × ngày (giảm đều 4 SP/ngày, 40 SP / 10 ngày).

| Ngày | 0 | 1 | 2 | 3 | 4 | 5 | 6 | 7 | 8 | 9 | 10 |
|---|---|---|---|---|---|---|---|---|---|---|---|
| Lý tưởng | 40 | 36 | 32 | 28 | 24 | 20 | 16 | 12 | 8 | 4 | 0 |
| Thực tế | 40 | 38 | 36 | 36 | 36 | 36 | 32 | 29 | 26 | 23 | 20 |
| Chênh lệch (thực tế − lý tưởng) | 0 | +2 | +4 | +8 | +12 | +16 | +16 | +17 | +18 | +19 | +20 |

Chênh lệch luôn dương, nghĩa là đường thực tế **luôn nằm trên** đường lý tưởng.

---

## Phần 1 – Phân tích

| Nhận định | Đúng/Sai | Dẫn chứng số liệu | Cách hiểu đúng |
|---|---|---|---|
| **N1.** Trục dọc thể hiện số giờ làm việc đã dùng | **Sai** | Bảng số liệu ghi "Còn lại" tính bằng Story Points: từ 40 giảm xuống 20 ở ngày 10, không phải giờ làm và không tăng dần. | Trục Y là **khối lượng công việc còn lại (Story Points)**; trục X là các ngày làm việc trong Sprint. |
| **N2.** Đường lý tưởng giảm đều 4 điểm/ngày, chạm 0 vào ngày 10 | **Đúng** (giữ nguyên) | 40 SP / 10 ngày = 4 SP/ngày; ngày 5 còn 20, ngày 10 còn 0. | Đường lý tưởng giảm đều từ tổng khối lượng về 0 vào ngày cuối Sprint. |
| **N3.** Ngày 2–5 đường thực tế đi ngang chứng tỏ đội làm việc ổn định | **Sai** | Ngày 2, 3, 4, 5 đều còn 36 SP, tức 3 ngày liên tiếp (ngày 3, 4, 5) đội burn 0 SP; đến ngày 5 lệch lý tưởng +16 SP (36 so với 20). | Đường đi ngang nghĩa là **không có việc nào hoàn thành**, dấu hiệu **bị chặn (impediment)**, không phải ổn định. |
| **N4.** Đường thực tế luôn dưới đường lý tưởng nên đội nhanh hơn kế hoạch | **Sai** | Ngược lại: ngày 1 là 38 > 36, ngày 5 là 36 > 20, ngày 10 là 20 > 0 (chênh +2 → +20). Cuối Sprint còn 20/40 SP (50%) chưa xong. | Đường thực tế **nằm trên** đường lý tưởng nghĩa là **trễ lịch trình**; chưa có thời điểm nào đội trước lịch trình. |

---

## Phần 2 – Vá lỗi (các hiện tượng bị bỏ qua)

**Hiện tượng 1 – Bị chặn (ngày 3–5, burn 0 SP trong 3 ngày liên tiếp).**
Phải nêu ngay trong Daily Scrum của **ngày 3** (khi đường đi ngang lần đầu xuất hiện): Developers báo impediment, **Scrum Master Lan** chịu trách nhiệm gỡ vướng (liên hệ bên liên quan, xử lý phụ thuộc/môi trường) trong chính ngày đó, không để kéo sang ngày 5.

**Hiện tượng 2 – Trễ lịch trình kéo dài (lệch +16 SP ở ngày 5, +20 SP ở ngày 10).**
Ngay tại điểm giữa Sprint (**ngày 5–6**), **Product Owner Đức** cùng Developers (Tú, Vy, Khoa) rà lại khối lượng và đàm phán cắt/hoãn các User Story giá trị thấp để giữ Sprint Goal; phần chưa đạt Definition of Done cuối Sprint được trả về Product Backlog để PO sắp xếp lại ở **Sprint Review/Planning kế tiếp**, đồng thời đưa nguyên nhân trễ vào **Retrospective**.
