# RikkeiGo – Chốt nhãn MoSCoW cho Sprint tới ("Tháng khuyến mãi")

**Người soạn:** Lan (Scrum Master) – **Gửi:** Đức (Product Owner)
**Năng lực Sprint:** 10 điểm – **Tổng điểm các hạng mục:** 15 điểm (nên phải cắt 5 điểm)

---

## Phần 1 – Đề xuất: 2 cách gán nhãn

**Cách A – "Kiểm tra hậu quả khi thiếu" (theo tiêu chí chung).**
Mọi hạng mục, bất kể bộ phận nào đề xuất, đều trả lời cùng 2 câu hỏi: (1) Thiếu nó, bản phát hành cuối Sprint có chạy được / có gây hại không? (2) Đã có cách xử lý tạm thời chưa? Không chạy được hoặc gây thiệt hại → Must; có cách tạm → hạ nhãn.

**Cách B – "Theo bộ phận đề xuất" (thương lượng / bỏ phiếu).**
Mỗi bộ phận (Marketing, CSKH, Kỹ thuật…) tự nói hạng mục nào là Must; PO tổng hợp theo số phiếu hoặc mức độ ưu tiên của bộ phận, rồi cắt cho vừa năng lực.

---

## Phần 2 – So sánh

| Tiêu chí | Cách A – Hậu quả khi thiếu | Cách B – Theo bộ phận đề xuất |
|---|---|---|
| Khách quan khi nhiều bộ phận cùng đề xuất | **(+)** Mọi bộ phận bị đo bằng cùng một thước, nên không ai thắng chỉ vì nói to hay "đúng dịp". | **(–)** Marketing đòi #6, CSKH đòi #5 đều là Must; kết quả phụ thuộc sức ảnh hưởng, dễ thành "ai nhiều phiếu thì thắng". |
| Bảo vệ được hạng mục bắt buộc như #1 | **(+)** #1 đang thu sai tiền khách, hậu quả nặng nên chắc chắn thành Must, không bị ai đòi bỏ. | **(–)** #1 là sửa lỗi, không bộ phận nào "sở hữu" nên dễ bị lấn bởi các tính năng có người bảo vệ. |

**Chọn: Cách A.**

---

## Phần 3 – Áp dụng Cách A

| # | Hạng mục | Điểm | Nhãn | Lý do (gắn với bản phát hành cuối Sprint) |
|---|---|---|---|---|
| 1 | Sửa lỗi hiển thị sai cước sau KM | 2 | **Must** | Đang thu sai tiền khách; phát hành chương trình KM mà không sửa sẽ làm lỗi lan rộng, rủi ro pháp lý và uy tín. |
| 2 | Áp mã khuyến mãi khi đặt xe | 2 | **Must** | Là lõi của "Tháng khuyến mãi"; thiếu nó thì chương trình không chạy được. |
| 3 | Thanh toán bằng ví RikkeiPay | 3 | **Should** | Tiện và hỗ trợ KM, nhưng khách vẫn trả tiền mặt nên bản phát hành vẫn chạy được. |
| 4 | Hẹn giờ đặt xe trước | 3 | **Could** | Tăng số chuyến đặt trong tháng KM, nhưng không ảnh hưởng chương trình nếu thiếu; cắt đầu tiên nếu trễ. |
| 5 | Chat với tài xế | 3 | **Won't (bản này)** | CSKH coi là Must, nhưng khách vẫn gọi điện được (đã có cách tạm); không vừa năng lực. |
| 6 | Giao diện trang trí KM | 2 | **Won't (bản này)** | Nghe "đúng dịp" nhưng thiếu nó bản phát hành vẫn chạy bình thường, không gây hại. |

### Danh sách vào Sprint (vừa 10 điểm)

| Nhãn | Hạng mục | Điểm |
|---|---|---|
| Must | #1, #2 | 4 |
| Should | #3 | 3 |
| Could | #4 | 3 |
| **Tổng** | | **10 / 10** |

**Tỷ lệ Must = 4 / 10 = 40%.**

> **Lưu ý cho Đức:** Quy tắc nói Must khoảng 60% (≈ 6 điểm), nhưng chỉ có 2 hạng mục thực sự bắt buộc (4 điểm). Muốn đủ 6 điểm phải nâng #6 (trang trí) hoặc một mục 3 điểm có cách xử lý tạm lên Must, và như vậy là gán sai nhãn. Nên mình giữ Must ở 40% và để phần dư làm Should/Could, đây cũng là phần đệm có thể cắt khi trễ (6 điểm).

### Thông báo hạng mục Won't cho bên liên quan

- **Marketing (#6):** Giao diện trang trí không vào bản này. Chương trình KM vẫn chạy đủ chức năng; có thể xem xét ở Sprint sau nếu còn thời gian KM.
- **CSKH (#5):** Chat với tài xế không vào bản này. Khách vẫn gọi điện cho tài xế như hiện tại; đưa vào Backlog cho Sprint sau.
