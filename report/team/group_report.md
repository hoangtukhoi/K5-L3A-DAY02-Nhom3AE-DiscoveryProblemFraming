# Báo cáo nhóm — Day 02 Discovery & Problem Framing

> Bản chung của nhóm, viết trên repo do nhóm trưởng fork. Không copy file này sang repo cá nhân.
> Template chi tiết và prompt mẫu: [docs/01-worksheet.md](../../docs/01-worksheet.md). Bài mẫu: [docs/02-deliverable-example.md](../../docs/02-deliverable-example.md).

## 1. Thông tin nhóm

- Tên nhóm:
- Thành viên: xem `TEAM.md`
- Candidate problem được chọn (1 câu):
- Quyết định cuối: Go / Not Yet / No-Go

---

## 2. Hội tụ nhóm (CP3)

### 2.1. Pitch

| # | Người đưa ra | Candidate (Job Story ngắn) | Actor | Bottleneck | Câu hỏi phản biện nhận được (ai hỏi) |
|---:|---|---|---|---|---|
| 1 | | | | | |
| 2 | | | | | |
| 3 | | | | | |
| 4 | | | | | |
| 5 | | | | | |
| 6 | | | | | |
| 7 | | | | | |
| 8 | | | | | |
| 9 | | | | | |
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
| 4 | | | | | |
| 5 | | | | | |
| 6 | | | | | |

*Điền 4–6 giả định; xóa dòng thừa.*

Giả định nhóm kiểm chứng trong buổi này:

### 3.2. Kiểm chứng

Cách đã dùng: Phỏng vấn / Survey / Log, ticket, review

Interview snapshot (mỗi buổi phỏng vấn một bảng, hoặc đặt file trong `report/assets/cp4-interview-snapshot-N.md`):

| Trường | Nội dung |
|---|---|
| Người được hỏi (vai trò, không ghi tên thật) | |
| Câu nói đáng nhớ nhất (nguyên văn) | |
| Lần gần nhất gặp vấn đề này: chuyện gì đã xảy ra? | |
| Hiện đang xử lý bằng cách nào (workaround)? | |
| Mất bao lâu, bao lần? | |
| Insight / opportunity rút ra | |

Tổng hợp:

| Nguồn | Số người / số mẫu | Tín hiệu xác nhận | Tín hiệu phản bác |
|---|---:|---|---|
| | | | |

**Nhóm đã sửa problem thế nào sau kiểm chứng:**

### 3.3. Research giải pháp đã có

| Công cụ / case / pattern | Link | Giải bước nào trong quy trình? | Điểm mạnh | Khoảng trống / rủi ro | Bài học cho nhóm |
|---|---|---|---|---|---|
| | | | | | |
| | | | | | |
| | | | | | |

---

## 4. Quy trình trước/sau (CP5)

### 4.1. Quy trình hiện tại

Sơ đồ (ASCII, Mermaid hoặc link ảnh trong `report/assets/`):

```text

```

| Bước | Actor | Input | Output | Thời gian / tần suất | Ghi chú |
|---:|---|---|---|---|---|
| 1 | | | | | |
| 2 | | | | | |
| 3 | | | | | |
| 4 | | | | | |
| 5 | | | | | |

**Bottleneck chính:**

### 4.2. Quy trình tương lai

Ghi rõ bước nào **Rule**, bước nào **AI**, bước nào **con người**, **boundary** ở đâu, **phương án quay về** khi AI sai.

```text

```

### 4.3. Before / after

| Chỉ số | Trước | Sau (kỳ vọng) | Ghi chú |
|---|---:|---:|---|
| Số bước | | | |
| Tổng thời gian | | | |
| Số bước thủ công | | | |
| Bottleneck chính | | | |
| Rủi ro mới phát sinh | | | |

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

*Người chính: Vũ Lê Hoàng · Hỗ trợ: Nguyễn Minh Quân, Nguyễn Đức Minh, Phan Gia Bảo*

**Ma trận:** Độ mơ hồ cao (khách mô tả bằng lời tự do: tiếng kêu, mùi, cảm giác lái; mỗi lần một kiểu). Độ phức tạp thấp–trung bình (các bước cố định, không rẽ nhánh). → Workflow có AI ở một bước.

| Mức | Phương án | Đủ khi nào | Rủi ro | Chọn? |
|---|---|---|---|---|
| No AI | Đào tạo cố vấn + danh sách câu hỏi in sẵn tại quầy | Cố vấn luôn hỏi đủ, khách tới trực tiếp | Không giảm số lần gọi lại trước khi xe tới | Dùng làm phương án quay về |
| Rule | Ô bắt buộc trong form đặt lịch theo bộ câu hỏi ASE C1 | Lỗi rơi vào vài loại cố định | Không đọc được mô tả tự do; khách có thể bỏ dở form dài | Dùng cho bước 1 |
| Workflow | Form bắt buộc → AI gợi ý câu hỏi còn thiếu + soạn nháp phiếu → cố vấn duyệt | Các bước cố định, AI chỉ làm phần đọc và viết | Gợi ý sai, tóm tắt sai lời khách | Chọn |
| Agent | AI tự nhắn khách, tự hỏi tiếp, tự tạo lệnh sửa chữa | Khi bước tiếp theo không đoán trước được | Tự liên hệ khách, khó kiểm soát, nhiều quyền truy cập | Không chọn |

**Vì sao không chọn mức đơn giản hơn:** Rule (ô bắt buộc) chỉ bắt được các mục cố định; mô tả tự do kiểu "xe kêu như tiếng tất khô" (ví dụ trên diễn đàn DealersEdge) không vào được ô nào, và đây chính là phần cố vấn phải gọi lại hỏi. Tuy vậy bằng chứng còn yếu: nếu khảo sát cho thấy thông tin thiếu chỉ là vài mục cố định (giả định #2) thì Rule là đủ và nhóm sẽ dừng ở Rule.

**AI Canvas rút gọn:**

| Thành phần | Nội dung |
|---|---|
| Prediction | 2–3 câu hỏi còn thiếu cho mô tả của khách; nháp phiếu tiếp nhận theo mẫu (triệu chứng, khi nào, điều kiện, số km) |
| Judgment | Cố vấn quyết định câu hỏi nào cần hỏi, mô tả nào đủ để giao kỹ thuật viên |
| Action | Cố vấn gửi câu hỏi đã duyệt cho khách hoặc hỏi khi khách tới; tạo lệnh sửa chữa |
| Outcome | Số lần gọi lại khách mỗi lịch; số lần kỹ thuật viên hỏi lại cố vấn; tỉ lệ câu hỏi gợi ý bị cố vấn bỏ |
| Input | Nội dung khách điền khi đặt lịch (ô bắt buộc + mô tả tự do), đời xe, số km |
| Feedback | Câu hỏi cố vấn sửa hoặc bỏ mỗi ngày; câu kỹ thuật viên hỏi lại |

**Câu hỏi PAIR:**

- Augment hay automate? Augment. Cố vấn vẫn là người hỏi khách và chịu trách nhiệm phiếu; không gửi gì cho khách nếu cố vấn chưa duyệt.
- Sai kiểu nào tệ hơn? Bỏ sót tệ hơn báo nhầm: thiếu một câu hỏi quan trọng thì kỹ thuật viên sửa sai; thừa một câu hỏi chỉ tốn thêm của khách vài giây. Tiêu chí đánh giá ưu tiên "không bỏ sót thông tin cần thiết".

---

## 7. Problem Statement v1 + tiêu chí đánh giá (CP6)

| Trường | Nội dung |
|---|---|
| Actor | Cố vấn dịch vụ tiếp nhận lịch đặt bảo dưỡng, sửa chữa, ở xưởng có cho khách mô tả nhu cầu bằng lời tự do khi đặt lịch |
| Quy trình | Đọc lịch đặt → gọi lại khách hỏi thêm → ghi phiếu tiếp nhận → xác nhận tại quầy → tạo lệnh sửa chữa → bàn giao kỹ thuật viên |
| Bottleneck | Gọi lại khách hỏi thêm vì mô tả lúc đặt lịch thiếu, và cố vấn không có bộ câu hỏi bổ sung theo từng loại triệu chứng (~5–10 phút mỗi lịch, ước lượng) |
| Impact | Mất thời gian cố vấn; kỹ thuật viên đoán từ thông tin thiếu, có thể sửa sai, khách quay lại (theo tư liệu công khai ở mục 3.2) |
| Success Metric | (1) Số lần gọi lại khách mỗi lịch: [đo] → tối đa 1; (2) số lần kỹ thuật viên hỏi lại cố vấn: [đo] → giảm 50%; (3) cố vấn bỏ dưới 30% câu hỏi AI gợi ý; đo trong 2 tuần pilot |
| Boundary | AI không chẩn đoán, không báo giá, không kết luận bảo hành, không tự liên hệ khách, không sửa thông tin khách đã điền |
| AI intervention point | Sau khi khách gửi form đặt lịch, trước bước cố vấn gọi lại khách |
| Mức chọn | Workflow (Rule ở bước form + AI ở bước gợi ý câu hỏi, soạn nháp phiếu) |
| Rủi ro & người kiểm tra | Gợi ý sai, bỏ sót, tóm tắt sai lời khách → cố vấn đối chiếu nháp với lời khách trước khi dùng |

| Trường | v0 | v1 | Vì sao đổi |
|---|---|---|---|
| Actor | Cố vấn dịch vụ tiếp nhận lịch đặt | Thêm: ở xưởng cho khách mô tả tự do khi đặt lịch | Nếu xưởng chỉ dùng ô chọn cố định thì Rule là đủ, không cần AI |
| Success Metric | Chỉ đo tốc độ | Thêm số lần kỹ thuật viên hỏi lại và tỉ lệ câu hỏi bị bỏ | Phản biện: nhanh hơn mà phiếu vẫn thiếu thì không đạt |
| Boundary | Không tự nhắn khách, không chẩn đoán, không báo giá | Thêm: không kết luận bảo hành, không sửa thông tin khách điền | Tư liệu DealerELITE: ghi sai mô tả có thể làm mất bảo hành |

**Tiêu chí đánh giá:**

| # | Tiêu chí | Đạt khi | Không đạt khi |
|---|---|---|---|
| 1 | Không bỏ sót | Hỏi đủ các mục còn thiếu: triệu chứng, khi nào xảy ra, liên tục hay thỉnh thoảng, điều kiện | Bỏ qua mục còn thiếu mà kỹ thuật viên cần |
| 2 | Không hỏi lại điều khách đã nói | Mọi câu hỏi đều về thông tin chưa có | Hỏi lại điều khách đã ghi trong form |
| 3 | Không bịa, không chẩn đoán | Nháp phiếu chỉ chứa thông tin khách đã đưa | Có nguyên nhân lỗi, giá hoặc kết luận bảo hành |
| 4 | Ngắn, dễ trả lời | Tối đa 3 câu, mỗi câu khách trả lời được trong 1 dòng | Câu dài, dùng thuật ngữ kỹ thuật |

---

## 8. Quyết định (CP6)

| Rủi ro | Mức | Lý do |
|---|---|---|
| Value | Trung bình | Tư liệu công khai xác nhận pain, nhưng cả 3 nguồn ở Mỹ; chưa có số liệu Việt Nam hay VinFast (giả định #1, #2) |
| Usability | Thấp | Cố vấn chỉ duyệt và sửa vài câu hỏi; có phương án quay về là danh sách câu hỏi cố định |
| Feasibility | Trung bình | Đã có công cụ làm gần đúng việc này (myKaarma Service Pre-Diag), nhưng nhóm chưa biết lấy được nội dung đặt lịch từ hệ thống của xưởng không |
| Viability | Cao | Dữ liệu khách hàng; chưa biết quy định nội bộ có cho đưa vào công cụ bên ngoài (giả định #4) |

**Quyết định:** Not Yet. Viability ở mức Cao nhưng kiểm chứng nhanh được bằng cách hỏi người làm ở xưởng; Value cần số liệu Việt Nam trước khi làm.

**Ngưỡng dừng:** Nếu khảo sát 10 người từng đặt lịch cho thấy dưới 30% bị gọi lại hỏi thêm → No-Go. Nếu thông tin thiếu chỉ là vài mục cố định → dừng ở Rule (form bắt buộc). Nếu pilot 2 tuần mà cố vấn bỏ quá 50% câu hỏi AI gợi ý → quay về danh sách câu hỏi cố định.

**Bước tiếp theo:** (1) Khảo sát 10 người từng đặt lịch bảo dưỡng; (2) hỏi một cố vấn dịch vụ thật về số lần gọi lại và quy định dữ liệu; (3) thử form bắt buộc trước, chỉ thêm AI nếu form không đủ.

**Nguồn**

- [KTAR — Ever have your auto shop fix the wrong noise](https://ktar.com/uncategorized/ever-have-your-auto-shop-fix-the-wrong-noise)
- [DealersEdge forum — Terminology](https://forums.dealersedge.com/viewtopic.php?p=48481)
- [DealerELITE — The 3 C's: Customer concern](https://www.dealerelite.net/profiles/blogs/the-3c-s-customer-concern)
- [myKaarma — Service Pre-Diag AI Overview](https://support.mykaarma.com/hc/en-us/articles/45647747400211-Service-Pre-Diag-AI-Overview-Smarter-Service-Conversations-Before-Check-In)
- [Brake & Front End — ASE C1 Test Prep, Customer Interview and Write Up](https://www.brakeandfrontend.com/ase-c1-test-prep-customer-interview-and-write-up/)
- [Motor Magazine — Make Your Initial Assessment Count (2012)](https://www.motor.com/wp-content/uploads/MakeYourInitialAssessmentCount-Feb-2012.pdf)
