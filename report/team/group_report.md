# Báo cáo nhóm — Day 02 Discovery & Problem Framing

> Bản chung của nhóm, viết trên repo do nhóm trưởng fork. Không copy file này sang repo cá nhân.
> Template chi tiết và prompt mẫu: [docs/01-worksheet.md](../../docs/01-worksheet.md). Bài mẫu: [docs/02-deliverable-example.md](../../docs/02-deliverable-example.md).

## 1. Thông tin nhóm

- Tên nhóm: Nhom3AE
- Thành viên: xem `TEAM.md`
- Candidate problem được chọn (1 câu): Khi nhận yêu cầu đặt lịch, cố vấn dịch vụ muốn có mô tả nhu cầu đủ rõ, để chuyển cho kỹ thuật viên mà không phải hỏi lại khách nhiều đợt.
- Quyết định cuối: Not Yet

---

## 2. Hội tụ nhóm (CP3)

### 2.1. Pitch

| # | Người đưa ra | Candidate (Job Story ngắn) | Actor | Bottleneck | Câu hỏi phản biện nhận được (ai hỏi) |
|---:|---|---|---|---|---|
| 1 | | | | | |
| 2 | | | | | |
| 3 | | | | | |
| 4 | Phan Gia Bảo | Khi chuẩn bị báo cáo tuần, muốn nhận biết những triệu chứng được khách phản ánh nhiều, để trưởng xưởng ưu tiên kiểm tra và theo dõi. | Cố vấn dịch vụ | Phải đọc từng phiếu và gộp các mô tả cùng nghĩa nhưng khác câu chữ trước khi thống kê, dễ đếm trùng hoặc bỏ sót. | |
| 5 | Phan Gia Bảo | Khi tiếp nhận xe khách đã sửa chữa trước đó, muốn nắm nhanh lịch sử sự cố và cách xử lý, để tránh hỏi lại và cung cấp đủ thông tin cho kỹ thuật viên. | Cố vấn dịch vụ, khách hàng | Phải đọc nhiều phiếu sửa chữa và ghi chú rời rạc để tìm thông tin liên quan đến triệu chứng hiện tại. | |
| 6 | Phan Gia Bảo | Khi bàn giao xe sau sửa chữa, muốn giải thích dễ hiểu những hạng mục đã làm và lưu ý sử dụng, để khách hiểu và thực hiện đúng. | Cố vấn dịch vụ, nhân viên | Phiếu sửa chữa có thuật ngữ và ghi chú kỹ thuật; phải diễn giải lại theo tình trạng từng xe, dễ bỏ sót lưu ý. |  |
| 7 | | | | | Nếu đã có bảng giá cố định, vì sao vẫn phải chờ người trả lời?<br>Giá sơ bộ có đủ để báo khách khi chưa kiểm tra xe không? |
| 8 | | | |  | Chỉ dựa vào điều khoản bảo hành đã xác định được việc nào miễn phí chưa? |
| 9 | | | |  | Thông tin đặt lịch đã đủ để kỹ thuật viên bắt đầu sửa chữa chưa? Cần kiểm tra những thông tin nào trước khi tạo lệnh sửa chữa? |
| 10 | | | | | |
| 11 | | | | | |
| 12 | | | | | |

### 2.2. Cluster

| Cluster | Các candidate | Pattern chung |
|---|---|---|
| A | | |
| B | | |
| C | | |

### 2.3. Opportunity Solution Tree rút gọn

Gốc là **1 outcome**. Nhánh là **opportunity** (nhu cầu, pain), không phải tính năng hay công cụ.

```text
OUTCOME: 
├── Opportunity A: 
├── Opportunity B: 
└── Opportunity C: 
```

Những ý đã gạch bỏ vì là solution đội lốt opportunity:

- 

### 2.4. Chấm điểm shortlist (1–5)

| Candidate | Actor rõ | Quy trình rõ | Pain có bằng chứng | Impact đo được | Vừa sức lab | So sánh được No AI/Rule/Workflow/Agent | Nhóm hiểu domain | Tổng |
|---|---:|---:|---:|---:|---:|---:|---:|---:|
| | | | | | | | | |
| | | | | | | | | |
| | | | | | | | | |

**Candidate được chọn:**

**Vì sao chọn:**

**Vì sao loại các candidate còn lại:**

**Xử lý bất đồng (nếu có):**

---

## 3. Kiểm chứng + research giải pháp đã có (CP4)

### 3.1. Assumption Map

| # | Giả định | Loại (Value / Usability / Feasibility / Viability) | Quan trọng (1–5) | Đã có bằng chứng (1–5) | Kiểm chứng trước? |
|---:|---|---|---:|---:|---|
| 1 | | | | | |
| 2 | | | | | |
| 3 | | | | | |
| 4 | Công ty cho phép đưa nội dung đặt lịch của khách vào công cụ xử lý bên ngoài | Viability | 4 | 1 | Sau lab (hỏi người làm ở xưởng) | Phan Gia Bảo |

Giả định nhóm kiểm chứng trong buổi này:

### 3.2. Kiểm chứng

Cách đã dùng: Phỏng vấn / Survey / Log, ticket, review

**Snapshot 2 — tư liệu công khai (diễn đàn quản lý xưởng DealersEdge)**

| Trường | Nội dung |
|---|---|
| Người được hỏi (vai trò) | Quản lý xưởng dịch vụ, cố vấn dịch vụ, tư vấn đại lý |
| Câu nói đáng nhớ nhất (nguyên văn) | "Customer states there is a problem with the brakes." |
| Lần gần nhất gặp vấn đề: chuyện gì đã xảy ra? | Cố vấn chép nguyên lời khách lên phiếu, không hỏi thêm; có phiếu kết thúc bằng "không tìm thấy lỗi" |
| Workaround hiện tại | Đào tạo lại cố vấn cách đặt câu hỏi bổ sung |
| Mất bao lâu, bao lần? | Không có số liệu |
| Insight | Nguyên nhân nằm cả ở thói quen hỏi của cố vấn, không chỉ ở khách |

Tổng hợp:

| Nguồn | Số người / số mẫu | Tín hiệu xác nhận | Tín hiệu phản bác |
|---|---:|---|---|
| | | | |

**Nhóm đã sửa problem thế nào sau kiểm chứng:**

### 3.3. Research giải pháp đã có

| Công cụ / case / pattern | Link | Giải bước nào trong quy trình? | Điểm mạnh | Khoảng trống / rủi ro | Bài học cho nhóm |
|---|---|---|---|---|---|
| ASE C1 — hướng dẫn phỏng vấn khách khi tiếp nhận (luyện thi chứng chỉ cố vấn dịch vụ) | https://www.brakeandfrontend.com/ase-c1-test-prep-customer-interview-and-write-up/ | Lúc tiếp nhận: bộ câu hỏi chuẩn (lỗi là gì, khi nào xảy ra, liên tục hay thỉnh thoảng, điều kiện, lặp lại được không) | Không cần công nghệ; là chuẩn nghề, dùng làm danh sách câu hỏi bắt buộc được ngay | Phụ thuộc cố vấn có hỏi đủ hay không; không nói cách ghi phiếu theo mẫu | Là nền cho mức Rule: biến bộ câu hỏi này thành ô bắt buộc trong form đặt lịch |

---

## 4. Quy trình trước/sau (CP5)

### 4.1. Quy trình hiện tại

*Thời gian là ước lượng của nhóm, chưa bấm giờ thật.*

| # | Bước | Actor | Input | Output | Thời gian / tần suất |
|---|---|---|---|---|---|
| 1 | Đọc lịch đặt mới | Cố vấn dịch vụ | Lịch đặt từ app / web / hotline | Danh sách xe sắp tới | ~2 phút / lịch, mỗi ngày |
| 2 | Gọi lại khách hỏi thêm khi mô tả thiếu | Cố vấn dịch vụ | Mô tả tự do của khách | Mô tả bổ sung | ~5 phút / lần, có thể 2 đợt ← BOTTLENECK |
| 3 | Ghi phiếu tiếp nhận | Cố vấn dịch vụ | Mô tả đã bổ sung | Phiếu tiếp nhận | ~3 phút |
| 4 | Khách tới xưởng, hỏi lại tại quầy | Cố vấn dịch vụ, khách | Phiếu tiếp nhận | Phiếu đã xác nhận | ~5 phút |
| 5 | Tạo lệnh sửa chữa, nhập tay lại | Cố vấn dịch vụ | Phiếu đã xác nhận | Lệnh sửa chữa | ~3 phút |
| 6 | Bàn giao cho kỹ thuật viên | Cố vấn → kỹ thuật viên | Lệnh sửa chữa | Kỹ thuật viên bắt tay sửa | ~2 phút; nếu thiếu thì kỹ thuật viên hỏi lại cố vấn |

**Bottleneck chính:** Bước 2, gọi lại khách hỏi thêm vì mô tả lúc đặt lịch thiếu (khoảng 5–10 phút mỗi lịch, ước lượng). Tổng khoảng 20–25 phút mỗi lượt.

### 4.2. Quy trình tương lai

| # | Bước | Ai / cái gì làm | Ghi chú |
|---|---|---|---|
| 1 | Khách đặt lịch, điền các ô bắt buộc (loại lỗi, khi nào xảy ra, liên tục hay thỉnh thoảng, số km) + mô tả tự do | Rule (form đặt lịch) | Ô bắt buộc lấy từ bộ câu hỏi chuẩn ASE C1 |
| 2 | Đọc mô tả tự do, gợi ý 2–3 câu hỏi còn thiếu và soạn nháp phiếu tiếp nhận theo mẫu | AI hỗ trợ | Không chẩn đoán, không báo giá |
| 3 | Duyệt câu hỏi gợi ý, sửa, rồi gửi khách hoặc hỏi khi khách tới | Cố vấn dịch vụ (người kiểm tra) | Boundary: không câu hỏi nào gửi khách nếu cố vấn chưa duyệt |
| 4 | Xác nhận phiếu với khách tại quầy | Cố vấn dịch vụ | Ngắn hơn vì phiếu đã gần đủ |
| 5 | Tạo lệnh sửa chữa từ phiếu đã duyệt, bàn giao kỹ thuật viên | Cố vấn dịch vụ |  |

**Boundary:** AI không chẩn đoán lỗi, không báo giá, không kết luận bảo hành, không tự nhắn hay gọi khách, không sửa thông tin khách đã điền.

**Phương án quay về:** Gợi ý sai hoặc nháp kém → cố vấn bỏ qua, dùng danh sách câu hỏi cố định in sẵn (mức Rule), như quy trình hiện tại.

### 4.3. Before / after

| Chỉ số | Trước | Sau (kỳ vọng) | Ghi chú |
|---|---|---|---|
| Số bước | 6 | 5 |  |
| Tổng thời gian mỗi lượt | ~20–25 phút (ước lượng) | ~10–12 phút | Cần bấm giờ thật để có baseline |
| Bước thủ công | 6/6 | 3/5 | Cố vấn vẫn duyệt, xác nhận, bàn giao |
| Bottleneck | Gọi lại khách hỏi thêm | Cố vấn duyệt câu hỏi gợi ý | Chấp nhận được vì đây là điểm kiểm soát chất lượng |
| Rủi ro mới | — | AI gợi ý câu hỏi thừa, sai, hoặc tóm tắt sai lời khách | Xử lý bằng boundary và tiêu chí đánh giá ở mục 7 |

---

## 5. Problem Statement v0 (CP5)

| Trường | Nội dung |
|---|---|
| Actor | Cố vấn dịch vụ tiếp nhận lịch đặt bảo dưỡng, sửa chữa tại xưởng dịch vụ |
| Quy trình | Đọc lịch đặt → gọi lại khách hỏi thêm → ghi phiếu tiếp nhận → xác nhận tại quầy → tạo lệnh sửa chữa → bàn giao kỹ thuật viên |
| Bottleneck | Gọi lại khách hỏi thêm vì mô tả lúc đặt lịch thiếu, và cố vấn không có bộ câu hỏi bổ sung theo từng loại triệu chứng (~5–10 phút mỗi lịch, ước lượng) |
| Impact | Mất thời gian cố vấn; kỹ thuật viên đoán từ thông tin thiếu, có thể sửa sai, khách quay lại (theo tư liệu công khai ở mục 3.2) |
| Success Metric | Số lần gọi lại khách mỗi lịch: [đo 1 tuần] → tối đa 1; thời gian tiếp nhận mỗi lượt: [đo 1 tuần] → giảm 50%; đo bằng cố vấn tự ghi trong 2 tuần pilot |
| Boundary | Không tự nhắn khách, không chẩn đoán lỗi, không báo giá; cố vấn duyệt mọi thứ trước khi tới khách hoặc kỹ thuật viên |

**Phản biện nhận được:** Metric chỉ đo tốc độ, chưa đo chất lượng: tiếp nhận nhanh hơn mà phiếu vẫn thiếu thì kỹ thuật viên vẫn phải hỏi lại. Nhóm đồng ý, thêm metric chất lượng ở v1.

---

## 5. Problem Statement v0 (CP5)

| Trường | Nội dung |
|---|---|
| **Actor** | |
| **Quy trình** | |
| **Bottleneck** | |
| **Impact** | |
| **Success Metric** (baseline → target, cách đo) | |
| **Boundary** (AI không được làm gì; khi nào cần con người kiểm tra — HITL) | |

Phản biện nhận được (từ AI hoặc nhóm khác) và nhóm có đồng ý không:

-

---

## 6. Mức can thiệp AI (CP6)

### 6.1. Ma trận độ mơ hồ × độ phức tạp

Bài của nhóm nằm ở ô:

Vì sao:

### 6.2. So sánh 4 mức

| Mức | Phương án cho bài của nhóm | Đủ khi nào | Rủi ro | Chọn? |
|---|---|---|---|---|
| **No AI** (sửa quy trình) | | | | |
| **Rule** | | | | |
| **Workflow** | | | | |
| **Agent** | | | | |

**Mức chọn:**

**Vì sao không chọn mức đơn giản hơn:**

### 6.3. AI Canvas rút gọn

| Thành phần | Nội dung |
|---|---|
| **Prediction** — AI dự đoán / tạo ra gì? | |
| **Judgment** — con người cân nhắc, quyết định gì? | |
| **Action** — hành động cuối cùng là gì, ai làm? | |
| **Outcome** — đo kết quả bằng gì? | |
| **Input** — AI cần dữ liệu đầu vào gì mỗi lần chạy? Có sẵn không? | |
| **Feedback** — lấy phản hồi ở đâu để cải thiện? | |

### 6.4. Hai câu hỏi của Google PAIR

- Người dùng muốn **được hỗ trợ (augment)** hay **giao hẳn việc (automate)**? Bằng chứng:
- AI sai kiểu nào tệ hơn, **báo nhầm** hay **bỏ sót**? Vì sao, và thiết kế đã xử lý thế nào:

---

## 7. Problem Statement v1 + tiêu chí đánh giá (CP6)

| Trường | Nội dung |
|---|---|
| **Actor** | |
| **Quy trình** | |
| **Bottleneck** | |
| **Impact** | |
| **Success Metric** (baseline → target, cách đo) | |
| **Boundary** | |
| **AI intervention point** | |
| **Mức chọn** | No AI / Rule / Workflow / Agent |
| **Rủi ro & người kiểm tra** | |

**Thay đổi so với v0 và lý do:**

| Trường | v0 | v1 | Vì sao đổi |
|---|---|---|---|
| | | | |

**Tiêu chí đánh giá đầu ra của AI (3–5 tiêu chí):**

| # | Tiêu chí | Đạt khi | Không đạt khi |
|---:|---|---|---|
| 1 | | | |
| 2 | | | |
| 3 | | | |

---

## 8. Quyết định (CP6)

### 8.1. Bốn rủi ro

| Rủi ro | Câu hỏi | Mức độ rủi ro (Thấp = an toàn / TB / Cao = nguy hiểm) | Lý do / bằng chứng |
|---|---|---|---|
| **Value** | Người dùng có thật sự cần và sẽ dùng không? | | |
| **Usability** | Người dùng có dùng được, có hiểu và sửa được đầu ra của AI không? | | |
| **Feasibility** | Có đủ dữ liệu, công cụ, kỹ năng để làm không? | | |
| **Viability** | Có hợp chi phí, pháp lý, quy định tổ chức không? Ai vận hành? | | |

### 8.2. Kết luận

**Quyết định:** Go / Not Yet / No-Go

**Lý do:**

**Nếu Go — pilot nhỏ nhất:**

**Nếu Not Yet — cần kiểm chứng gì trước:**

**Nếu No-Go — nên làm gì thay AI:**

**Ngưỡng dừng** (nếu sau … mà … thì quay về …):

---

## 9. Hạn chế và hướng tiếp theo

-

## 10. Tài liệu tham khảo

-
