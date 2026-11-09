# Báo cáo cá nhân — 2A202603562_PhanGiaBao

## 1. Thông tin học viên

- Họ tên: Phan Gia Bảo
- MSSV: 2A202603562
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm: Nhom3AE 
- Link repo nhóm: https://github.com/hoangtukhoi/K5-L3A-DAY02-Nhom3AE-DiscoveryProblemFraming/tree/main

---

Cơ sở thực tế: VinFast có quy trình đặt lịch bảo dưỡng, sửa chữa qua website, ứng dụng và hotline. Tài liệu ứng dụng có bước chọn dịch vụ, địa điểm, thời gian và xác nhận; khách hàng có thể bổ sung mô tả nhu cầu. 

Nhân vật: An, cố vấn dịch vụ tại một xưởng dịch vụ VinFast. Hằng ngày, An tiếp nhận nhu cầu của khách, chuẩn bị thông tin cho kỹ thuật viên và phản hồi các câu hỏi liên quan đến dịch vụ.

---

## 2. Scan problem (CP1)

Lăng kính: **Lặp lại** · **Tốn thời gian** · **Cần đọc, tổng hợp nhiều thông tin** · **Pain từ người khác**.

| # | Lăng kính | Job Story: Khi… tôi muốn… để… | Ai chịu ảnh hưởng? | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng) |
|---:|---|---|---|---|
| 1 | Cần đọc, tổng hợp nhiều thông tin | Khi chuẩn bị báo cáo tuần, tôi muốn nhận biết những triệu chứng được khách phản ánh nhiều, để trưởng xưởng ưu tiên kiểm tra và theo dõi. | Cố vấn dịch vụ, trưởng xưởng | Phải đọc lại phần mô tả tự do trong các phiếu tiếp nhận của cả tuần, mỗi khách ghi một kiểu ("kêu lạch cạch", "có tiếng gõ gầm xe"...). Ước tính 1–2 giờ/tuần. Chưa có số liệu thật, cần hỏi người làm cố vấn dịch vụ. |
| 2 | Tốn thời gian | Khi tiếp nhận xe khách đã sửa chữa trước đó, tôi muốn nắm nhanh lịch sử sự cố và cách xử lý, để tránh hỏi lại và cung cấp đủ thông tin cho kỹ thuật viên. | Cố vấn dịch vụ, khách hàng, kỹ thuật viên | Lịch sử bảo dưỡng/sửa chữa được lưu trên hệ thống chung (có bài báo chủ xe nhắc tới điều này), nhưng ghi chú của các lần trước thường dài và rời rạc. Ước tính 3–5 phút/xe quay lại, xưởng đông có thể 10+ xe/ngày. |
| 3 | Pain từ người khác | Khi khách chỉ mô tả chung chung "xe có tiếng kêu" lúc tiếp nhận, tôi muốn hỏi đủ chi tiết ngay tại quầy (kêu ở đâu, khi nào, ở tốc độ bao nhiêu), để kỹ thuật viên không phải nhờ tôi gọi lại khách hoặc chạy thử mò. | Kỹ thuật viên, cố vấn dịch vụ, khách hàng | Ứng dụng có ô "mô tả nhu cầu" nhưng khách thường ghi rất ngắn hoặc bỏ trống. Ước tính khoảng 1/3 phiếu sửa chữa (không tính bảo dưỡng định kỳ) phải hỏi bổ sung, mỗi lần mất thêm 10–20 phút. Cần kiểm chứng. |
| 4 | Lặp lại | Khi khách gọi/nhắn hỏi "xe tôi xong chưa?", tôi muốn trả lời ngay tình trạng và thời gian dự kiến, để khách không phải gọi nhiều lần và tôi không phải chạy xuống xưởng hỏi kỹ thuật viên. | Cố vấn dịch vụ, khách hàng, kỹ thuật viên | Câu hỏi gần như giống nhau, lặp lại trong ngày. Ước tính 10–20 cuộc/ngày ở xưởng đông. |
| 5 | Lặp lại | Khi có lịch hẹn cho ngày hôm sau, tôi muốn xác nhận lại với khách và nhắc mang theo giấy tờ cần thiết, để giảm khách không đến hoặc đến trễ làm lệch lịch khoang sửa chữa. | Cố vấn dịch vụ, xưởng | Ứng dụng đã có xác nhận khi đặt lịch, nhưng vẫn có khách quên. Ước tính 15–20 lịch hẹn/ngày, mỗi cuộc gọi xác nhận 2–3 phút, tức khoảng 40–60 phút/ngày. Chưa biết tỷ lệ no-show thật. |
| 6 | Tốn thời gian | Khi báo giá phát sinh cho khách, tôi muốn giải thích được hạng mục nào trong bảo hành, hạng mục nào khách phải trả, để khách đồng ý nhanh và không thắc mắc lúc thanh toán. | Cố vấn dịch vụ, khách hàng | Phải tra chính sách bảo hành theo từng dòng xe và từng bộ phận (pin, động cơ, phụ tùng hao mòn). Khách hay hỏi đi hỏi lại khi hóa đơn khác báo giá ban đầu. Ước tính 5–8 lần báo giá phát sinh/ngày, mỗi lần mất 5–10 phút tra cứu và giải thích. |

**Nếu có dùng AI để gợi ý thêm:** ý nào AI gợi ý mà bạn giữ lại, ý nào bỏ và vì sao.

- Mình tự scan trước được 5 ý (số 1, 2, 3, 5, 6), sau đó mới nhờ AI gợi ý thêm theo lăng kính "Lặp lại". Mình giữ lại ý số 4 (khách gọi hỏi "xe xong chưa?") vì đây là việc An gặp nhiều lần mỗi ngày và dễ đo bằng số cuộc gọi. Mình bỏ ý AI gợi ý "dự đoán xe sắp hỏng để chủ động gọi khách", vì đó là việc của hệ thống chẩn đoán trên xe chứ không phải pain của An, và mình cũng không có dữ liệu để kiểm chứng.

---

## 3. Top 3 Problem Cards + quy trình nháp (CP2)

### Bảng chọn top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---:|---|---|---|
| 1 | Phiếu tiếp nhận thiếu thông tin triệu chứng, kỹ thuật viên phải hỏi lại (#3) | Actor rõ (An tại quầy tiếp nhận). Bottleneck cụ thể là bước gọi lại khách/chạy thử. Impact đo được bằng % phiếu phải hỏi lại. Vừa sức một buổi lab vì chỉ xoay quanh một bước tiếp nhận. | Tỷ lệ phiếu thiếu thông tin thực tế là bao nhiêu. Có thể xưởng đã có checklist rồi mà mình không biết. |
| 2 | Nắm nhanh lịch sử sửa chữa khi xe quay lại (#2) | Actor rõ, quy trình tra cứu vẽ được 6 bước, bottleneck là bước đọc lệnh cũ (đo được bằng phút). Liên quan tới card 1 vì lỗi lặp lại thì lịch sử rất quan trọng. | Hệ thống hiện tại tra lịch sử dễ hay khó. Nếu đã có màn hình tóm tắt thì problem này yếu. |
| 3 | Khách hỏi tiến độ sửa xe lặp lại nhiều lần (#4) | Tần suất cao, impact dễ đo (đếm số cuộc gọi/ngày), quy trình ngắn nên dễ vẽ và vừa sức một buổi lab. | Có thể giải bằng cập nhật trạng thái trên app, không cần AI. Không chắc app VinFast đã có tính năng này chưa. |

### Problem Card #1

| Trường | Nội dung |
|---|---|
| Job Story | Khi khách mang xe đến sửa với mô tả triệu chứng chung chung, tôi muốn hỏi đúng và đủ các câu cần thiết ngay lúc tiếp nhận, để kỹ thuật viên có đủ thông tin chẩn đoán mà không phải gọi lại khách. |
| Actor | An (cố vấn dịch vụ). Người hưởng lợi: kỹ thuật viên, khách hàng. |
| Thời điểm / bối cảnh | Lúc khách đặt lịch sửa chữa qua app/hotline (ô mô tả nhu cầu) và lúc khách đến quầy tiếp nhận, đặc biệt giờ cao điểm buổi sáng khi nhiều xe vào cùng lúc. |
| Quy trình hiện tại (3–7 bước) | 1. An tiếp nhận, hỏi miệng khách (5'). 2. Ghi phiếu (5'). 3. Chuyển phiếu cho kỹ thuật viên (2'). 4. Kỹ thuật viên đọc phiếu, thấy thiếu thông tin (3'). 5. Nhờ An gọi lại khách hoặc tự chạy thử để tìm lỗi (15'). 6. Chẩn đoán (20'). 7. Báo giá cho khách (10'). |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 5: gọi lại khách / chạy thử, khoảng 15 phút mỗi phiếu thiếu thông tin (dao động 10–20 phút nếu khách không nghe máy). Số liệu là giả định, cần hỏi kỹ thuật viên thật. |
| Impact (nếu không giải thì sao) | Xe nằm xưởng lâu hơn, khoang sửa bị chiếm; khách bị gọi nhiều lần và có cảm giác xưởng không chuyên nghiệp; có rủi ro sửa không đúng lỗi khách phản ánh, khách phải quay lại. |
| Success metric (baseline → target) | % phiếu sửa chữa kỹ thuật viên phải hỏi bổ sung: giả định ~30% → dưới 10%. Phụ: thời gian từ lúc nhận xe đến lúc có chẩn đoán giảm khoảng 15 phút/xe. |
| Phương án không dùng AI | Làm checklist câu hỏi cố định theo nhóm triệu chứng (tiếng kêu, rung, cảnh báo trên màn hình, sạc/pin...), in lên phiếu hoặc thành form bắt buộc trên app khi chọn "sửa chữa". |
| Giả thuyết về AI (nếu có) | Khách mô tả bằng lời tự nhiên rất đa dạng, checklist cứng khó bao hết. AI có thể đọc mô tả, xếp vào nhóm triệu chứng và gợi ý cho An 3–5 câu hỏi còn thiếu. An vẫn là người hỏi và quyết định, AI chỉ gợi ý. |
| Cảm nhận nhanh | Rule / Workflow (nghiêng về thử checklist trước, AI chỉ là bước sau nếu checklist không đủ) |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — 60 phút (với phiếu thiếu thông tin)

[1 Tiếp nhận, hỏi miệng: 5'] → [2 Ghi phiếu: 5'] → [3 Chuyển KTV: 2']
→ [4 KTV đọc phiếu: 3'] → [5 Gọi lại khách / chạy thử: 15'] ← BOTTLENECK
→ [6 Chẩn đoán: 20'] → [7 Báo giá cho khách: 10']
```

### Problem Card #2

| Trường | Nội dung |
|---|---|
| Job Story | Khi tiếp nhận xe của khách đã từng sửa chữa trước đó, tôi muốn nắm nhanh lịch sử sự cố và cách đã xử lý, để không hỏi lại khách và báo cho kỹ thuật viên biết lỗi có lặp lại hay không. |
| Actor | An (cố vấn dịch vụ) |
| Thời điểm / bối cảnh | Lúc khách vừa tới quầy, khách đang đứng chờ nên An cần thông tin trong vài phút. |
| Quy trình hiện tại (3–7 bước) | 1. Nhập biển số/số VIN để tìm xe (1'). 2. Mở danh sách các lần vào xưởng (1'). 3. Mở từng lệnh sửa chữa cũ để đọc ghi chú (4'). 4. Tự tóm tắt những lần liên quan (1'). 5. Hỏi lại khách để xác nhận (2'). 6. Ghi chú vào phiếu mới cho kỹ thuật viên (2'). |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3: đọc từng lệnh sửa chữa cũ, khoảng 4 phút/xe (3–5 phút), vì ghi chú do nhiều người viết, khác cách diễn đạt. Lâu hơn với xe chạy dịch vụ vào xưởng nhiều lần. |
| Impact (nếu không giải thì sao) | Bỏ sót lỗi lặp lại (ví dụ đã thay một chi tiết 2 lần mà vẫn hỏng) nên kỹ thuật viên xử lý lại theo cách cũ; khách bực vì phải kể lại; khách chờ ở quầy lâu. |
| Success metric (baseline → target) | Thời gian An nắm được lịch sử liên quan: ~4 phút → dưới 1 phút. Số lần phải hỏi lại khách thông tin đã có trên hệ thống: giảm rõ rệt (cần đo baseline). |
| Phương án không dùng AI | Thêm ô "tóm tắt cho lần sau" bắt buộc khi đóng lệnh sửa chữa; màn hình lịch sử lọc theo bộ phận (phanh, pin, treo...). |
| Giả thuyết về AI (nếu có) | AI đọc các lệnh sửa chữa cũ và tóm tắt theo bộ phận, đánh dấu những lần cùng triệu chứng với lần này. Cần có trích dẫn lệnh gốc để An kiểm tra lại, tránh AI tóm sai. |
| Cảm nhận nhanh | Workflow |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — 11 phút / xe quay lại

[1 Tra biển số/VIN: 1'] → [2 Mở danh sách lần vào xưởng: 1']
→ [3 Đọc từng lệnh sửa chữa cũ: 4'] ← BOTTLENECK
→ [4 Tự tóm tắt: 1'] → [5 Hỏi lại khách xác nhận: 2'] → [6 Ghi phiếu mới cho KTV: 2']
```

### Problem Card #3

| Trường | Nội dung |
|---|---|
| Job Story | Khi khách gọi hoặc nhắn hỏi xe đã sửa xong chưa, tôi muốn trả lời ngay tình trạng và giờ nhận xe dự kiến, để khách yên tâm và không phải gọi thêm lần nữa. |
| Actor | An (cố vấn dịch vụ). Người hưởng lợi: khách hàng. |
| Thời điểm / bối cảnh | Rải rác cả ngày, dày hơn vào buổi chiều khi khách muốn biết có lấy xe trong ngày được không. |
| Quy trình hiện tại (3–7 bước) | 1. Nhận cuộc gọi/tin nhắn của khách (1'). 2. An tìm phiếu của xe (2'). 3. An hỏi kỹ thuật viên (gọi nội bộ hoặc đi xuống khoang) và chờ trả lời (7'). 4. Kỹ thuật viên ước lượng tiến độ (1'). 5. An gọi/nhắn lại cho khách (2'). |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 3: chờ kỹ thuật viên rảnh tay để trả lời, khoảng 7 phút/lượt (3–10 phút), còn làm gián đoạn kỹ thuật viên đang sửa xe. |
| Impact (nếu không giải thì sao) | An bị ngắt việc liên tục; kỹ thuật viên bị hỏi trong lúc đang sửa; khách không được trả lời kịp thì gọi lại hoặc đánh giá dịch vụ thấp. |
| Success metric (baseline → target) | Số cuộc gọi hỏi tiến độ/ngày: ước tính 15 → dưới 5. Thời gian trả lời khách: ~10 phút → dưới 2 phút. |
| Phương án không dùng AI | Kỹ thuật viên bấm cập nhật trạng thái theo bước (đang chẩn đoán / chờ phụ tùng / đang sửa / rửa xe / sẵn sàng giao), hệ thống tự gửi thông báo cho khách. |
| Giả thuyết về AI (nếu có) | Có thể không cần AI. Nếu có thì chỉ để trả lời các câu hỏi phụ của khách bằng ngôn ngữ tự nhiên dựa trên trạng thái đã có. |
| Cảm nhận nhanh | No AI / Rule |

Quy trình nháp hiện tại:

```text
HIỆN TẠI — 13 phút / lượt hỏi (khoảng 15 lượt/ngày)

[1 Nhận cuộc gọi/tin nhắn: 1'] → [2 Tìm phiếu của xe: 2']
→ [3 Hỏi KTV, chờ trả lời: 7'] ← BOTTLENECK
→ [4 KTV ước lượng tiến độ: 1'] → [5 Báo lại khách: 2']
```

### Card muốn pitch nhất

- Card số: 1
- Vì sao: Đây là lỗi ở "đầu nguồn" — thông tin thiếu ngay từ lúc tiếp nhận thì mọi bước sau đều chậm theo. Card 2 và 3 có thể đã có giải pháp sẵn trong hệ thống hoặc giải được bằng tính năng đơn giản, còn card 1 liên quan tới cách khách mô tả bằng lời nên khó làm checklist bao hết, đáng để thảo luận xem có cần AI hay không.
- Câu hỏi muốn nhóm phản biện: Con số "khoảng 30% phiếu phải hỏi lại" có hợp lý không, và nhóm có cách nào kiểm chứng (hỏi người làm ở xưởng, hay tìm review của khách) không? Nếu checklist đơn giản đã giải được 80% thì có nên bỏ hẳn hướng AI không?

### AI đã phản biện card thế nào

Mình đưa 3 card cho AI với yêu cầu đóng vai "PM hoài nghi", soi kỹ số liệu và hỏi vì sao problem này đáng làm.

| Điểm yếu AI chỉ ra | Đồng ý? | Đã sửa gì |
|---|---|---|
| Các con số baseline (30%, 10–20 phút) đều là giả định, không có nguồn. | Đồng ý | Ghi rõ "giả định, cần kiểm chứng" trong card và đưa vào câu hỏi muốn nhóm phản biện. |
| Card 1 ban đầu viết giải pháp AI ngay trong Job Story ("muốn AI gợi ý câu hỏi") — bị solution-first. | Đồng ý | Viết lại Job Story chỉ nói nhu cầu (hỏi đủ thông tin), tách phần AI ra ô "Giả thuyết về AI". |
| Card 3 gần như không cần AI, nên cân nhắc có giữ trong top 3 không. | Đồng ý một phần | Vẫn giữ vì tần suất cao và dễ đo, nhưng để cảm nhận là No AI / Rule cho trung thực. |
| Card 2 có rủi ro AI tóm tắt sai lịch sử sửa chữa, ảnh hưởng tới kỹ thuật viên. | Đồng ý | Thêm yêu cầu tóm tắt phải kèm trích dẫn lệnh sửa chữa gốc để An tự kiểm tra. |

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động | Tôi đã làm gì? | Kết quả / ảnh hưởng tới bài nhóm |
|---|---|---|
| Pitch Problem Card | Pitch 3 candidate (#4, #5, #6 trong bảng pitch nhóm): (1) thống kê triệu chứng khách phản ánh nhiều cho báo cáo tuần; (2) nắm nhanh lịch sử sửa chữa khi xe quay lại; (3) giải thích dễ hiểu hạng mục đã sửa và lưu ý sử dụng khi bàn giao xe. | Candidate (1) và (2) được gom vào cluster C "Tổng hợp lịch sử sự cố"; candidate (3) vào cluster B "Tra cứu và diễn giải thông tin dịch vụ". Cả hai cluster đều không được chọn (cluster C 20 điểm, cluster B 18 điểm, so với 26 điểm của candidate được chọn). |
| Phản biện bài của bạn khác | Câu hỏi tôi đã đặt (cho các candidate của Vũ Lê Hoàng): <br>• #7 báo giá sơ bộ: "Nếu đã có bảng giá cố định, vì sao vẫn phải chờ người trả lời?" và "Giá sơ bộ có đủ để báo khách khi chưa kiểm tra xe không?" <br>• #8 điều khoản bảo hành: "Chỉ dựa vào điều khoản bảo hành đã xác định được việc nào miễn phí chưa?" <br>• #9 đồng bộ booking: "Thông tin đặt lịch đã đủ để kỹ thuật viên bắt đầu sửa chữa chưa? Cần kiểm tra những thông tin nào trước khi tạo lệnh sửa chữa?" | Câu hỏi cho #7 và #8 được nhóm dùng làm lý do loại cluster B: giá và chính sách bảo hành là thông tin cố định, đăng sẵn hoặc làm FAQ là đủ, ít chỗ để bàn về AI. Câu hỏi cho #9 chỉ ra "đồng bộ booking" là giải pháp, nhóm gạch khỏi OST, và gắn với nhánh A (thông tin đặt lịch thiếu), cũng là nhánh được chọn. |
| Nhận phản biện | Câu hỏi tôi nhận được (từ Vũ Lê Hoàng): <br>• Candidate thống kê triệu chứng: "Tại sao không có 1 từ điển mã lỗi chung để dễ thống kê lỗi hơn?" <br>• Candidate lịch sử sửa chữa: "Lịch sử này nằm ở đâu? Trên phần mềm quản lý xưởng, sổ bảo hành giấy hay hệ thống FOTA?" | Tôi đã sửa gì: "Từ điển mã lỗi chung" được nhóm xác định là giải pháp đội lốt opportunity nên gạch khỏi OST, giữ lại opportunity C ở dạng vấn đề (ghi chép rải rác, mỗi người viết một kiểu). Câu hỏi về nơi lưu lịch sử cho thấy tôi chưa rõ hệ thống thật của xưởng, góp phần vào lý do loại cluster C (thiếu dữ liệu phiếu sửa chữa, domain 1/5). |
| Gom cluster / cây OST | Hỗ trợ CP3 (người chính: Nguyễn Minh Quân): đưa 3 candidate của mình vào cluster B và C. | Opportunity C trong OST ("ghi chép sự cố rải rác, muốn xem lịch sử xe hay thống kê phải đọc lại từng phiếu") hình thành chủ yếu từ 2 candidate của tôi. |
| Chọn candidate problem | Tham gia chấm điểm shortlist; câu phản biện của tôi cho candidate báo giá và bảo hành được ghi làm lý do loại cluster B. | Nhóm chọn: "Cố vấn dịch vụ muốn có mô tả nhu cầu đủ rõ khi nhận lịch đặt, để không phải hỏi lại khách nhiều đợt". Hướng này trùng với Problem Card #1 tôi đã viết ở CP2 (phiếu tiếp nhận thiếu thông tin triệu chứng). |
| Kiểm chứng / research | Hỗ trợ CP4 (người chính: Nguyễn Đức Minh): <br>• Làm Snapshot 2 — diễn đàn quản lý xưởng DealersEdge. <br>• Research ASE C1 — hướng dẫn phỏng vấn khách khi tiếp nhận (Brake & Front End). <br>• Phụ trách giả định #4 (Viability: công ty có cho đưa nội dung đặt lịch vào công cụ bên ngoài không), kiểm chứng sau lab. | Snapshot 2 cho tín hiệu phản bác quan trọng: lỗi nằm cả ở thói quen hỏi của cố vấn, không chỉ ở khách → nhóm thu hẹp problem thành "cố vấn không có bộ câu hỏi bổ sung theo từng loại triệu chứng" và thêm phương án không dùng AI. ASE C1 trở thành nền cho mức Rule (ô bắt buộc trong form đặt lịch). |
| Quy trình nhóm | Người chính CP5 — Quy trình trước/sau (mục 4 bài nhóm): vẽ quy trình hiện tại 6 bước, xác định bottleneck ở bước gọi lại khách hỏi thêm; vẽ quy trình tương lai 5 bước, boundary, phương án quay về và bảng before/after. | Bottleneck và quy trình này được dùng nguyên cho trường "Quy trình" và "Bottleneck" của Problem Statement v0 và v1. Ô bắt buộc ở bước 1 lấy từ bộ câu hỏi ASE C1 tôi tìm. |
| Problem Statement | Hỗ trợ: phần quy trình, bottleneck và boundary của Problem Statement lấy từ quy trình trước/sau tôi làm. | Problem Statement v1 thêm metric chất lượng (số lần kỹ thuật viên hỏi lại, tỉ lệ câu hỏi AI gợi ý bị bỏ) sau phản biện "metric chỉ đo tốc độ". |
| Mức can thiệp AI | Hỗ trợ CP6 (người chính: Vũ Lê Hoàng). | Ví dụ "xe kêu như tiếng tất khô" từ nguồn DealersEdge (Snapshot 2 của tôi) được dùng để giải thích vì sao Rule không đủ và chọn Workflow. |
| Quyết định | Tham gia đánh giá rủi ro; giả định #4 (Viability) do tôi phụ trách. | Quyết định Not Yet, trong đó Viability ở mức Cao chính là giả định #4 chưa kiểm chứng. Bước tiếp theo (2) — hỏi một cố vấn dịch vụ thật về quy định dữ liệu — là phần việc gắn với tôi. |

---

## 5. Dùng AI

| Checkpoint | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai hoặc hời hợt ở đâu? | Tôi sửa gì bằng nhận định của mình? |
|---|---|---|---|---|
| CP1 Scan | Nhờ AI gợi ý thêm problem theo lăng kính "Lặp lại", sau khi đã tự scan được 5 ý. | Gợi ý được ý khách gọi hỏi tiến độ, việc lặp lại mình chưa nghĩ tới. | Có ý lệch khỏi nhân vật An (dự đoán xe sắp hỏng). Con số tần suất AI đưa ra không có nguồn. | Bỏ ý không thuộc công việc của An; ghi rõ số liệu là ước tính. |
| CP2 Problem Card | Nhờ AI đóng vai "PM hoài nghi" phản biện 3 card. | Phát hiện Job Story card 1 bị solution-first; nhắc rủi ro AI tóm tắt sai ở card 2. | Phần quy trình hiện tại AI viết khá chung, không chắc đúng với quy trình xưởng thật. | Viết lại Job Story, thêm điều kiện kiểm tra lại cho card 2, để card 3 ở mức No AI / Rule. |
| CP4 Research | | | | |
| CP5 Quy trình | | | | |
| CP5–6 Problem Statement | | | | |
| CP6 Mức can thiệp / quyết định | | | | |

---

## 6. Reflection (CP7)

Trả lời bằng trải nghiệm thật của bạn, tối thiểu 200 từ cho các câu 6.1–6.6 (không tính 6.7, câu này được chấm riêng ở tiêu chí C5). **Không dùng AI để viết thay.**

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**

Lúc nghe pitch, mình thấy các bạn tự nghĩ ra những problem khác nhau, nhưng gom lại thì đều nói về chuyện thông tin chuyển từ người này sang người kia bị thiếu, phải hỏi lại. Trước đó mình nghĩ problem của mình chỉ là ý riêng. Thấy người khác cũng gặp thì mình tin hơn đây là pain thật chứ không phải mình tự tưởng tượng ra. Mình cũng nhận ra nhiều candidate, kể cả của mình, thật ra là giải pháp được viết thành problem, ví dụ “đồng bộ booking” hay “bảng báo giá sơ bộ”. Nghe người khác mắc lỗi này thì mình dễ thấy hơn là tự soi bài mình.

**6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?**

Có, và mình bị trước. Job Story 1 lúc đầu mình viết là “muốn AI gợi ý câu hỏi”, tức là đã chọn AI trước khi hiểu vấn đề. Khi nhờ AI phản biện thì mình mới thấy, rồi viết lại thành “muốn hỏi đủ thông tin”, còn phần AI để sang ô giả thuyết. Ở nhóm cũng vậy, mấy ý như “từ điển mã lỗi chung”, “đồng bộ booking”, “trích xuất điều khoản bảo hành” đều là giải pháp. Lúc vẽ OST, nhóm gạch các ý này ra và chỉ giữ opportunity ở dạng vấn đề. Ngoài ra nhóm cũng hơi có xu hướng muốn dùng AI ngay, may là có Snapshot 2 nên mới thêm phương án không dùng AI để so sánh.

**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**

Có. Hoàng hỏi mình “lịch sử sửa chữa này nằm ở đâu, phần mềm xưởng, sổ bảo hành giấy hay hệ thống FOTA?”. Mình không trả lời được, vì thật ra mình không biết hệ thống thật của xưởng VinFast lưu thế nào, mới chỉ đọc một bài báo có nhắc qua. Lúc đầu mình khá thích candidate này, nhưng sau câu hỏi đó mình đồng ý với nhóm là cluster C nên bỏ. Nhóm không có dữ liệu phiếu sửa chữa, và hiểu domain gần như bằng 0, nên làm tiếp thì chỉ toàn đoán.

**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?**

Có hai điều làm mình bất ngờ. Thứ nhất là trên diễn đàn DealersEdge, nhiều cố vấn chép nguyên lời khách lên phiếu, kiểu “Customer states there is a problem with the brakes”, rồi không hỏi thêm gì. Trước đó mình luôn nghĩ lỗi là do khách mô tả kém, hóa ra một phần do thói quen hỏi của cố vấn. Nhờ vậy nhóm thu hẹp problem lại. Thứ hai là myKaarma đã có công cụ làm gần y hệt ý tưởng của nhóm. Lúc đầu mình hơi hụt hẫng, sau mới nghĩ lại thì đây là dấu hiệu tốt vì problem có thật, và nhóm không cần tự xây từ đầu.

**6.5. Điều khó nhất khi viết Problem Statement là gì?**

Khó nhất là phần metric, vì nhóm không có số liệu thật nào. Thời gian trong quy trình mình vẽ đều là ước lượng, chưa ai bấm giờ. Cuối cùng phải để baseline là “[đo]”, nhìn hơi thiếu nhưng vẫn trung thực hơn là bịa một con số. Ngoài ra v0 chỉ đo tốc độ, bị phản biện mới thấy nếu tiếp nhận nhanh mà phiếu vẫn thiếu thì cũng như không, nên phải thêm metric chất lượng. Viết boundary cũng mất thời gian, vì phải nghĩ kỹ AI không được làm những gì.

**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**

Mình sẽ phỏng vấn người thật ngay từ đầu (thành viên nhóm khác), hoặc là đổi bối cảnh chủ đề. Mình sẽ phản biện mạnh hơn ở phần rủi ro Usability. Nhóm chấm Thấp vì chỉ nghĩ tới cố vấn, quên mất khách hàng. Giải pháp thêm ô bắt buộc vào form, nhưng giả định 3 (khách chịu trả lời thêm câu hỏi) thì chưa kiểm chứng. Nếu form dài làm khách bỏ không đặt lịch nữa thì giải pháp hỏng ngay bước đầu. Lúc đó mình thấy hơi lạ nhưng không nói. Giờ nghĩ lại, mình thấy nên để mức Trung bình.

**6.7. Hiểu bài:** giải thích bằng 5–8 câu, không nhìn tài liệu, chuỗi *problem → quy trình → metric → boundary → mức can thiệp AI → quyết định* của bài nhóm mình.

Problem của nhóm là cố vấn dịch vụ nhận lịch đặt có mô tả nhu cầu thiếu, nên phải gọi lại khách hỏi thêm, có khi tới 2 đợt, trước khi giao cho kỹ thuật viên. Quy trình hiện tại có 6 bước, bottleneck là bước gọi lại khách, khoảng 5–10 phút mỗi lịch (đây là ước lượng). Metric gồm số lần gọi lại khách mỗi lịch, số lần kỹ thuật viên hỏi lại cố vấn và tỉ lệ câu hỏi AI gợi ý bị cố vấn bỏ. Boundary là AI không chẩn đoán, không báo giá, không kết luận bảo hành, không tự liên hệ khách, và mọi câu hỏi phải qua cố vấn duyệt. Nhóm chọn Workflow: form có ô bắt buộc theo bộ câu hỏi ASE C1, sau đó AI đọc mô tả tự do để gợi ý câu hỏi còn thiếu, vì lời mô tả tự do không ô nào bắt được hết. Quyết định là Not Yet, vì chưa có số liệu Việt Nam về Value và chưa biết công ty có cho đưa dữ liệu khách ra công cụ bên ngoài không (Viability). Bước tiếp theo là khảo sát người từng đặt lịch, hỏi một cố vấn thật, và thử form bắt buộc trước khi thêm AI.

---

## 7. Tài liệu tham khảo

- Worksheet môn học: [docs/01-worksheet.md](../../docs/01-worksheet.md)
- Báo Thanh tra — "Thay đổi thói quen sử dụng ô tô với ứng dụng quản lý xe thông minh" (30/06/2022): đặt lịch bảo dưỡng, sửa chữa theo khung giờ trống trên ứng dụng VinFast. https://thanhtra.com.vn/thong-tin-doanh-nghiep/thay-doi-thoi-quen-su-dung-o-to-voi-ung-dung-quan-ly-xe-thong-minh-198884.html
- Tiền Phong — "Đi xa bằng VF 8, chủ xe nhẹ cả đầu lẫn ví nhờ hệ sinh thái hậu mãi toàn diện của VinFast": đặt lịch qua màn hình trung tâm, ứng dụng và tổng đài. https://tienphong.vn/di-xa-bang-vf-8-chu-xe-nhe-ca-dau-lan-vi-nho-he-sinh-thai-hau-mai-toan-dien-cua-vinfast-post1865193.tpo
- VnReview — bài về xưởng dịch vụ VinFast: chủ xe nhắc lịch sử bảo dưỡng, sửa chữa được quản lý đồng bộ trên hệ thống. https://vnreview.vn/threads/sau-ha-tang-sac-vinfast-hoa-giai-tiep-noi-lo-xuong-dich-vu-cua-chu-xe-dien.87895/
- Green SM — "Hướng dẫn đặt lịch bảo dưỡng/sửa chữa xe qua ứng dụng Green SM Driver": tài xế có thể đặt lịch kiểm tra sự cố kỹ thuật, hư hỏng tại xưởng VinFast. https://www.greensm.com/vn-vi/news/huong-dan-dat-lich-bao-duong-sua-chua-xe-qua-ung-dung-green-sm-driver
