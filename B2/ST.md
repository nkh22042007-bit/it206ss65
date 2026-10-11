# RikkeiGo – Quy trình xử lý story mới (dùng cho mọi bộ phận)

**Người soạn:** Lan (Scrum Master) – **Gửi:** Đức (Product Owner) xem xét

**Phạm vi:** Áp dụng cho mọi story mới từ Marketing, Chăm sóc khách hàng (CSKH), Vận hành, từ lúc nhận đến lúc nghiệm thu. Không áp dụng cho sự cố khẩn (lỗi đang gây thiệt hại thật); sự cố đó xử lý theo kênh hotfix riêng.

**Nguyên tắc chung:**
- Story mới luôn vào **Backlog**, không vào thẳng Sprint đang chạy.
- Nhãn MoSCoW do **một tiêu chí chung** quyết định, không theo người đề xuất.
- Một DoD chung cho mọi story; chỉ nâng dần theo năng lực đội.

---

## Phần 1 – Thiết kế quy trình (5 bước)

| Bước | Việc cần làm | Người chịu trách nhiệm | Điều kiện sang bước sau |
|---|---|---|---|
| **1. Tiếp nhận** | Người đề xuất gửi story theo mẫu "Là… tôi muốn… để…", nêu mục tiêu kinh doanh và bản phát hành mong muốn. Lan ghi vào Backlog. | Người đề xuất (bộ phận); Lan ghi nhận | Story có đủ: mô tả, giá trị mang lại, bản phát hành mong muốn, người đề xuất. Chưa gán nhãn. |
| **2. Làm rõ & viết AC** | Đức cùng Dev/QA và người đề xuất họp ngắn, viết **3–7 AC** theo Given – When – Then; ước lượng điểm. | Đức (chịu trách nhiệm nội dung); Dev/QA cùng viết | Có 3–7 AC, cả đội hiểu như nhau, đã ước lượng điểm. Thiếu AC thì **không** sang bước 3. |
| **3. Gán nhãn MoSCoW** | Lan hỏi 3 câu chung cho mọi story: (a) Thiếu nó, bản phát hành này có chạy được không? (b) Có cách xử lý tạm không? (c) Có gây hại (tiền, pháp lý, an toàn) không? Đức chốt nhãn gắn với **một bản phát hành cụ thể**. | Đức (quyết định); Lan điều phối | Mỗi story có đúng 1 nhãn + 1 dòng lý do. Must của bản phát hành ≈ 60% năng lực. Hạng mục Won't được báo cho người đề xuất. |
| **4. Chọn vào Sprint** | Tại Sprint Planning, Đức đề xuất thứ tự, Dev chọn theo năng lực thực tế. Ưu tiên Must, rồi Should, rồi Could. | Dev (cam kết); Đức (thứ tự) | Mọi story được chọn đều có AC, điểm, nhãn; tổng điểm ≤ năng lực Sprint. |
| **5. Làm & nghiệm thu theo DoD** | Dev làm xong, kiểm thử theo AC; Đức nghiệm thu ở Sprint Review. Retro xem có nên nâng DoD không. | Dev (làm đạt DoD); Đức (nghiệm thu) | Mọi AC đạt **và** story đạt DoD chung. Chưa đạt thì quay về Backlog, không tính điểm. |

---

## Phần 2 – Xử lý hai tình huống

### Tình huống 1: Giữa Sprint, Marketing đòi đưa "Tặng mã giới thiệu bạn bè" (chưa có AC) vào Sprint đang chạy

**Cách xử lý:** Story đi vào **bước 1** và nằm ở Backlog, không vào Sprint đang chạy, vì chưa có AC nên không thể vào Sprint (bước 2 chưa xong) và Sprint Goal đang được đội cam kết. Lan báo Marketing: AC sẽ được viết với Đức, nhãn gắn với bản phát hành, và story được cân nhắc ở Sprint Planning kế tiếp. Chỉ khi Đức thấy thật sự khẩn, Đức thương lượng trực tiếp với Dev: story đã có AC đầy đủ, và đổi lấy một story **cùng điểm** ra khỏi Sprint, miễn là Sprint Goal không bị ảnh hưởng.

**AC mẫu** (1 trong 3–7 AC của story):

> **Given** khách A đã có tài khoản và có mã giới thiệu riêng,
> **When** bạn bè mới đăng ký bằng mã của A và hoàn thành chuyến đi đầu tiên,
> **Then** cả A và bạn bè đều nhận mã giảm giá trong ví khuyến mãi, và mỗi mã giới thiệu chỉ được tính một lần cho một tài khoản mới.

### Tình huống 2: Cả 3 bộ phận đều cho rằng yêu cầu của mình là Must

**Cách xử lý:** Nhãn không do bộ phận tự gán. Ở **bước 3**, cả ba story đi qua cùng 3 câu hỏi (chạy được không / có cách tạm không / có gây hại không), và Đức chốt theo bản phát hành. Vì Must chỉ ≈ 60% năng lực, không thể cả ba cùng Must; story nào có cách tạm sẽ bị hạ nhãn và lý do được ghi lại, báo cho người đề xuất.

**Cách gán nhãn mẫu** (ví dụ giả định, bản phát hành "Tháng khuyến mãi"):

| Bộ phận | Story (ví dụ) | Tự gán | Kết quả 3 câu hỏi | Nhãn chốt |
|---|---|---|---|---|
| CSKH | Hoàn tiền cho chuyến bị tính sai cước | Must | Thiếu thì tiếp tục thu sai tiền khách, không có cách tạm tốt | **Must** |
| Vận hành | Màn hình xem tài xế đang rảnh | Must | Thiếu vẫn chạy được, đang xem tạm bằng bảng cũ | **Should** |
| Marketing | Tặng mã giới thiệu bạn bè | Must | Thiếu vẫn chạy được, chưa có AC | **Could** (chưa Ready; xét lại ở Sprint Planning sau) |

---

## Tóm tắt một dòng

**Nhận → Làm rõ (đủ 3–7 AC) → Gán nhãn theo tiêu chí chung → Vào Sprint khi đủ điều kiện → Làm xong khi đạt DoD.** Story mới giữa Sprint luôn quay về Backlog.
