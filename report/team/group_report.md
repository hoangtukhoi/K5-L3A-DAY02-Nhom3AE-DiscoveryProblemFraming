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

| #   | Người đưa ra     | Candidate (Job Story ngắn)                                                                                                                                                        | Actor                                                                     | Bottleneck                                                                                                                                 | Câu hỏi phản biện nhận được (ai hỏi)                                                                                                                                   |
| --- | ---------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| 1   | Nguyễn Đức Minh  | Khi nhận ca, muốn biết việc dở để không sót                                                                                                                                       | Nhân viên ca sau                                                          | Hỏi lại ca trước                                                                                                                           | Lần gần nhất việc bàn giao chỉ bằng hỏi lại ca trước khiến bạn bỏ sót công việc là khi nào, và hậu quả cụ thể là gì? (Nguyễn Minh Quân)                                |
| 2   | Nguyễn Đức Minh  | Khi hết ca, muốn báo cáo nhanh, để quản lý khỏi gọi hỏi                                                                                                                           | Trưởng ca                                                                 | Viết lại sự cố                                                                                                                             | Vì sao trưởng ca phải viết lại sự cố vào cuối ca, thông tin chưa được ghi nhận hay đã có nhưng nằm rải rác? (Nguyễn Minh Quân)                                         |
| 3   | Nguyễn Đức Minh  | Khi có người mới, muốn họ tự tra quy trình, để khỏi hỏi lại                                                                                                                       | Nhân viên mới                                                             | Hỏi lại người cũ                                                                                                                           | Người mới hỏi lại vì chưa có tài liệu, khó tìm tài liệu hay tài liệu có nhưng khó hiểu? (Nguyễn Minh Quân)                                                             |
| 4   | Phan Gia Bảo     | Khi chuẩn bị báo cáo tuần, muốn nhận biết những triệu chứng được khách phản ánh nhiều, để trưởng xưởng ưu tiên kiểm tra và theo dõi.                                              | Cố vấn dịch vụ                                                            | Phải đọc từng phiếu và gộp các mô tả cùng nghĩa nhưng khác câu chữ trước khi thống kê, dễ đếm trùng hoặc bỏ sót.                           | Tại sao không có 1 từ điển mã lỗi chung để dễ thống kê lỗi hơn, thay vì ghi các lỗi khác nhau làm loạn thống kê ? (Vũ Lê Hoàng)                                        |
| 5   | Phan Gia Bảo     | Khi tiếp nhận xe khách đã sửa chữa trước đó, muốn nắm nhanh lịch sử sự cố và cách xử lý, để tránh hỏi lại và cung cấp đủ thông tin cho kỹ thuật viên.                             | Cố vấn dịch vụ, khách hàng                                                | Phải đọc nhiều phiếu sửa chữa và ghi chú rời rạc để tìm thông tin liên quan đến triệu chứng hiện tại.                                      | Lịch sử này nằm ở đâu? Trên phần mềm quản lý xưởng, trên sổ bảo hành giấy của khách, hay lưu trong hệ thống FOTA (cập nhật phần mềm từ xa) của xe điện? (Vũ Lê Hoàng)  |
| 6   | Phan Gia Bảo     | Khi bàn giao xe sau sửa chữa, muốn giải thích dễ hiểu những hạng mục đã làm và lưu ý sử dụng, để khách hiểu và thực hiện đúng.                                                    | Cố vấn dịch vụ, nhân viên                                                 | Phiếu sửa chữa có thuật ngữ và ghi chú kỹ thuật; phải diễn giải lại theo tình trạng từng xe, dễ bỏ sót lưu ý.                              | Lần gần nhất khách hiểu sai hoặc không thực hiện đúng lưu ý sau sửa chữa là khi nào, và làm sao bạn biết nguyên nhân nằm ở cách giải thích lúc bàn giao? (Vũ Lê Hoàng) |
| 7   | Vũ Lê Hoàng      | Khi khách hàng gọi hotline hoặc đến xưởng hỏi giá, tôi muốn có ngay bảng báo giá sơ bộ cho các mốc bảo dưỡng tiêu chuẩn, để trả lời khách ngay lập tức.                           | Khách hàng, Cố vấn dịch vụ                                                | Chờ đợi người trả lời. Trường hợp hotline bận thì không thể gọi được trong khi thông tin này là cố định và có thể báo nhanh cho khách được | Nếu đã có bảng giá cố định, vì sao vẫn phải chờ người trả lời?<br>Giá sơ bộ có đủ để báo khách khi chưa kiểm tra xe không?<br>(Phan Gia Bảo)                           |
| 8   | Vũ Lê Hoàng      | Khi khách phàn nàn về lỗi pin hoặc linh kiện, tôi muốn trích xuất ngay điều khoản trong chính sách bảo hành mới nhất, để giải thích rõ ràng việc nào miễn phí, việc nào tính phí. | Cố vấn dịch vụ, khách hàng                                                | Phần này có trong chính sách của công ty, nhưng khách hàng thường không dành thời gian để đọc                                              | Chỉ dựa vào điều khoản bảo hành đã xác định được việc nào miễn phí chưa? (Phan Gia Bảo)                                                                                |
| 9   | Vũ Lê Hoàng      | Khi nhận xe tại xưởng, tôi muốn thông tin từ hệ thống booking đồng bộ ngay thành lệnh sửa chữa chi tiết, để KTV có thể bắt đầu làm việc lập tức mà không phải chờ đợi.            | Cố vấn dịch vụ, <br>Kĩ thuật viên                                         | Cố vấn dịch vụ phải nhập tay                                                                                                               | Thông tin đặt lịch đã đủ để kỹ thuật viên bắt đầu sửa chữa chưa? Cần kiểm tra những thông tin nào trước khi tạo lệnh sửa chữa? (Phan Gia Bảo)                          |
| 10  | Nguyễn Minh Quân | Làm rõ mô tả nhu cầu trước khi bàn giao                                                                                                                                           | An, cố vấn dịch vụ tiếp nhận và chuẩn bị mô tả nhu cầu cho kỹ thuật viên. | Phải hỏi bổ sung nhiều đợt                                                                                                                 | Thông tin hay thiếu nhất là gì: triệu chứng, đời xe hay số km? Nếu luôn thiếu đúng mấy mục đó thì thêm ô bắt buộc vào form đặt lịch đã đủ chưa? (Nguyễn Đức Minh)      |
| 11  | Nguyễn Minh Quân | Tra cứu câu trả lời dịch vụ đúng trường hợp                                                                                                                                       | An, cố vấn dịch vụ phụ trách phản hồi câu hỏi của khách.                  | Tìm đúng đoạn tài liệu                                                                                                                     | Khách hỏi lặp lại cùng các câu hay mỗi lần một khác? Tài liệu dịch vụ dài bao nhiêu trang mà phải mất công tìm? (Nguyễn Đức Minh)                                      |
| 12  | Nguyễn Minh Quân | Cập nhật bản chuẩn bị sau khi khách đổi lịch/nhu cầu                                                                                                                              | An, cố vấn dịch vụ cập nhật thông, kỹ thuật viên phụ trách lịch hẹn.      | Đối chiếu các phiên bản để tìm phần cần cập nhật                                                                                           | Khách đổi lịch hoặc đổi nhu cầu mấy lần một tuần? Nếu ít thì đối chiếu bằng tay có thật sự là vấn đề không? (Nguyễn Đức Minh)                                          |

### 2.2. Cluster

| Cluster                                                    | Các candidate                                                                                                                                                                                     | Pattern chung                                                                                                                                                                                                          |
| ---------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| A - Chuẩn hóa và cập nhật thông tin bàn giao               | Bàn giao ca bị sót việc dở; Nhập tay thông tin đặt lịch thành lệnh sửa chữa; Làm rõ mô tả nhu cầu trước khi bàn giao cho kỹ thuật viên; Cập nhật bản chuẩn bị khi khách đổi lịch hoặc đổi nhu cầu | Thông tin chuyển từ người này sang người kia (ca trước → ca sau, khách → cố vấn → kỹ thuật viên) bị thiếu, thay đổi giữa chừng hoặc phải nhập tay lại, nên người nhận phải hỏi bổ sung nhiều đợt trước khi bắt tay làm |
| B - Tra cứu và diễn giải thông tin dịch vụ đúng trường hợp | Nhân viên mới hỏi lại quy trình; Giải thích hạng mục đã sửa cho khách; Báo giá các mốc bảo dưỡng; Giải thích điều khoản bảo hành; Tra cứu câu trả lời dịch vụ đúng trường hợp                     | Thông tin đã có sẵn (bảng giá, chính sách bảo hành, quy trình, phiếu sửa chữa) nhưng khó tìm đúng đoạn hoặc khó hiểu, nên người hỏi phải chờ, phải hỏi người khác hoặc cố vấn phải diễn giải lại từng trường hợp       |
| C - Tổng hợp lịch sử sự cố để hỗ trợ xử lý                 | Báo cáo sự cố cuối ca; Thống kê triệu chứng khách phản ánh nhiều; Nắm lịch sử sửa chữa của xe                                                                                                     | Ghi chép sự cố nằm rải rác ở nhiều phiếu, mỗi người mô tả một kiểu, nên muốn báo cáo, thống kê hay xem lịch sử xe đều phải đọc lại từng phiếu và gộp bằng tay, dễ trùng hoặc sót                                       |

### 2.3. Opportunity Solution Tree rút gọn

```text
OUTCOME: Cố vấn dịch vụ xử lý một lượt khách nhanh hơn và ít phải hỏi lại
         (đo bằng: số phút mỗi lượt tiếp nhận, số lần hỏi lại khách hoặc kỹ thuật viên mỗi lượt)
├── Opportunity A: Thông tin khách đưa vào thiếu hoặc đổi giữa chừng, cố vấn phải hỏi lại
│                   nhiều đợt và nhập tay lại trước khi giao cho kỹ thuật viên
├── Opportunity B: Thông tin dịch vụ có sẵn nhưng khó tìm đúng đoạn, khó hiểu, khách phải chờ
│                   hoặc cố vấn phải diễn giải lại từng trường hợp
└── Opportunity C: Ghi chép sự cố rải rác, mỗi người viết một kiểu, muốn xem lịch sử xe
                    hay thống kê phải đọc lại từng phiếu
```

**Những ý đã gạch bỏ vì là solution đội lốt opportunity:**

- "Có bảng báo giá sơ bộ cho các mốc bảo dưỡng": là cách giải cho nhánh B.
- "Đồng bộ booking thành lệnh sửa chữa": là cách giải cho nhánh A.
- "Trích xuất điều khoản bảo hành": là cách giải cho nhánh B.
- "Từ điển mã lỗi chung" (câu hỏi phản biện cho candidate thống kê triệu chứng): là cách giải cho nhánh C.

### 2.4. Chấm điểm shortlist (1–5)

| Candidate                                                                       | Actor rõ | Quy trình rõ | Pain có bằng chứng | Impact đo được | Vừa sức lab | So sánh được No AI/Rule/Workflow/Agent | Nhóm hiểu domain | Tổng |
| ------------------------------------------------------------------------------- | -------- | ------------ | ------------------ | -------------- | ----------- | -------------------------------------- | ---------------- | ---- |
| Cố vấn phải hỏi lại khách nhiều đợt vì mô tả nhu cầu lúc đặt lịch thiếu         | 5        | 4            | 2                  | 4              | 4           | 5                                      | 2                | 26   |
| Khách và cố vấn mất công tìm, hiểu thông tin dịch vụ (giá, bảo hành, quy trình) | 3        | 3            | 2                  | 3              | 3           | 2                                      | 2                | 18   |
| Ghi chép sự cố rải rác, khó xem lịch sử xe và thống kê lỗi                      | 4        | 3            | 2                  | 3              | 3           | 4                                      | 1                | 20   |

**Candidate được chọn:** Khi nhận yêu cầu đặt lịch, cố vấn dịch vụ muốn có mô tả nhu cầu đủ rõ, để chuyển cho kỹ thuật viên mà không phải hỏi lại khách nhiều đợt.

**Vì sao chọn:** Actor rõ (cố vấn dịch vụ tiếp nhận lịch); 3 thành viên cùng đưa ra một nỗi khó (Nguyễn Đức Minh, Vũ Lê Hoàng, Nguyễn Minh Quân); quy trình vẽ được từ đặt lịch đến bàn giao cho kỹ thuật viên; có chỗ để so sánh giữa thêm ô bắt buộc vào form (Rule) với các mức dùng AI.

**Vì sao loại các candidate còn lại:** Loại "khó tìm, khó hiểu thông tin dịch vụ": giá mốc bảo dưỡng và chính sách bảo hành là thông tin cố định, đăng sẵn hoặc làm câu hỏi thường gặp là đủ, ít chỗ để bàn về AI (đúng câu phản biện Phan Gia Bảo đặt cho candidate báo giá và bảo hành). Loại "ghi chép sự cố rải rác": cần dữ liệu phiếu sửa chữa nhiều tháng mà nhóm không có, và nhóm không ai hiểu nghiệp vụ xưởng (domain 1/5).

**Xử lý bất đồng (nếu có):** Không có bất đồng

---

## 3. Kiểm chứng + research giải pháp đã có (CP4)

### 3.1. Assumption Map

|   # | Giả định | Loại (Value / Usability / Feasibility / Viability) | Quan trọng (1–5) | Đã có bằng chứng (1–5) | Kiểm chứng trước? |
| --: | -------- | -------------------------------------------------- | ---------------: | ---------------------: | ----------------- |
|   1 |          |                                                    |                  |                        |                   |
|   2 |          |                                                    |                  |                        |                   |
|   3 |          |                                                    |                  |                        |                   |
|   4 |          |                                                    |                  |                        |                   |
|   5 |          |                                                    |                  |                        |                   |
|   6 |          |                                                    |                  |                        |                   |

_Điền 4–6 giả định; xóa dòng thừa._

Giả định nhóm kiểm chứng trong buổi này:

### 3.2. Kiểm chứng

Cách đã dùng: Phỏng vấn / Survey / Log, ticket, review

Interview snapshot (mỗi buổi phỏng vấn một bảng, hoặc đặt file trong `report/assets/cp4-interview-snapshot-N.md`):

| Trường                                            | Nội dung |
| ------------------------------------------------- | -------- |
| Người được hỏi (vai trò, không ghi tên thật)      |          |
| Câu nói đáng nhớ nhất (nguyên văn)                |          |
| Lần gần nhất gặp vấn đề này: chuyện gì đã xảy ra? |          |
| Hiện đang xử lý bằng cách nào (workaround)?       |          |
| Mất bao lâu, bao lần?                             |          |
| Insight / opportunity rút ra                      |          |

Tổng hợp:

| Nguồn | Số người / số mẫu | Tín hiệu xác nhận | Tín hiệu phản bác |
| ----- | ----------------: | ----------------- | ----------------- |
|       |                   |                   |                   |

**Nhóm đã sửa problem thế nào sau kiểm chứng:**

### 3.3. Research giải pháp đã có

| Công cụ / case / pattern | Link | Giải bước nào trong quy trình? | Điểm mạnh | Khoảng trống / rủi ro | Bài học cho nhóm |
| ------------------------ | ---- | ------------------------------ | --------- | --------------------- | ---------------- |
|                          |      |                                |           |                       |                  |
|                          |      |                                |           |                       |                  |
|                          |      |                                |           |                       |                  |

---

## 4. Quy trình trước/sau (CP5)

### 4.1. Quy trình hiện tại

Sơ đồ (ASCII, Mermaid hoặc link ảnh trong `report/assets/`):

```text

```

| Bước | Actor | Input | Output | Thời gian / tần suất | Ghi chú |
| ---: | ----- | ----- | ------ | -------------------- | ------- |
|    1 |       |       |        |                      |         |
|    2 |       |       |        |                      |         |
|    3 |       |       |        |                      |         |
|    4 |       |       |        |                      |         |
|    5 |       |       |        |                      |         |

**Bottleneck chính:**

### 4.2. Quy trình tương lai

Ghi rõ bước nào **Rule**, bước nào **AI**, bước nào **con người**, **boundary** ở đâu, **phương án quay về** khi AI sai.

```text

```

### 4.3. Before / after

| Chỉ số               | Trước | Sau (kỳ vọng) | Ghi chú |
| -------------------- | ----: | ------------: | ------- |
| Số bước              |       |               |         |
| Tổng thời gian       |       |               |         |
| Số bước thủ công     |       |               |         |
| Bottleneck chính     |       |               |         |
| Rủi ro mới phát sinh |       |               |         |

---

## 5. Problem Statement v0 (CP5)

| Trường                                                                     | Nội dung |
| -------------------------------------------------------------------------- | -------- |
| **Actor**                                                                  |          |
| **Quy trình**                                                              |          |
| **Bottleneck**                                                             |          |
| **Impact**                                                                 |          |
| **Success Metric** (baseline → target, cách đo)                            |          |
| **Boundary** (AI không được làm gì; khi nào cần con người kiểm tra — HITL) |          |

Phản biện nhận được (từ AI hoặc nhóm khác) và nhóm có đồng ý không:

- ***

## 6. Mức can thiệp AI (CP6)

### 6.1. Ma trận độ mơ hồ × độ phức tạp

Bài của nhóm nằm ở ô:

Vì sao:

### 6.2. So sánh 4 mức

| Mức                       | Phương án cho bài của nhóm | Đủ khi nào | Rủi ro | Chọn? |
| ------------------------- | -------------------------- | ---------- | ------ | ----- |
| **No AI** (sửa quy trình) |                            |            |        |       |
| **Rule**                  |                            |            |        |       |
| **Workflow**              |                            |            |        |       |
| **Agent**                 |                            |            |        |       |

**Mức chọn:**

**Vì sao không chọn mức đơn giản hơn:**

### 6.3. AI Canvas rút gọn

| Thành phần                                                        | Nội dung |
| ----------------------------------------------------------------- | -------- |
| **Prediction** — AI dự đoán / tạo ra gì?                          |          |
| **Judgment** — con người cân nhắc, quyết định gì?                 |          |
| **Action** — hành động cuối cùng là gì, ai làm?                   |          |
| **Outcome** — đo kết quả bằng gì?                                 |          |
| **Input** — AI cần dữ liệu đầu vào gì mỗi lần chạy? Có sẵn không? |          |
| **Feedback** — lấy phản hồi ở đâu để cải thiện?                   |          |

### 6.4. Hai câu hỏi của Google PAIR

- Người dùng muốn **được hỗ trợ (augment)** hay **giao hẳn việc (automate)**? Bằng chứng:
- AI sai kiểu nào tệ hơn, **báo nhầm** hay **bỏ sót**? Vì sao, và thiết kế đã xử lý thế nào:

---

## 7. Problem Statement v1 + tiêu chí đánh giá (CP6)

| Trường                                          | Nội dung                        |
| ----------------------------------------------- | ------------------------------- |
| **Actor**                                       |                                 |
| **Quy trình**                                   |                                 |
| **Bottleneck**                                  |                                 |
| **Impact**                                      |                                 |
| **Success Metric** (baseline → target, cách đo) |                                 |
| **Boundary**                                    |                                 |
| **AI intervention point**                       |                                 |
| **Mức chọn**                                    | No AI / Rule / Workflow / Agent |
| **Rủi ro & người kiểm tra**                     |                                 |

**Thay đổi so với v0 và lý do:**

| Trường | v0  | v1  | Vì sao đổi |
| ------ | --- | --- | ---------- |
|        |     |     |            |

**Tiêu chí đánh giá đầu ra của AI (3–5 tiêu chí):**

|   # | Tiêu chí | Đạt khi | Không đạt khi |
| --: | -------- | ------- | ------------- |
|   1 |          |         |               |
|   2 |          |         |               |
|   3 |          |         |               |

---

## 8. Quyết định (CP6)

### 8.1. Bốn rủi ro

| Rủi ro          | Câu hỏi                                                           | Mức độ rủi ro (Thấp = an toàn / TB / Cao = nguy hiểm) | Lý do / bằng chứng |
| --------------- | ----------------------------------------------------------------- | ----------------------------------------------------- | ------------------ |
| **Value**       | Người dùng có thật sự cần và sẽ dùng không?                       |                                                       |                    |
| **Usability**   | Người dùng có dùng được, có hiểu và sửa được đầu ra của AI không? |                                                       |                    |
| **Feasibility** | Có đủ dữ liệu, công cụ, kỹ năng để làm không?                     |                                                       |                    |
| **Viability**   | Có hợp chi phí, pháp lý, quy định tổ chức không? Ai vận hành?     |                                                       |                    |

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
