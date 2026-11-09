# Báo cáo cá nhân — 2A202603510_NguyenMinhQuan

> File báo cáo: `2A202603510_NguyenMinhQuan.md`. Nội dung CP1, CP2 theo bối cảnh cố vấn dịch vụ An tại xưởng VinFast.
> Template chi tiết và prompt mẫu cho từng mục: [docs/01-worksheet.md](../../docs/01-worksheet.md).
> Mỗi thành viên một file trong `report/individual/` trên repo nhóm: copy template này thành file mới, điền, rồi commit bằng tài khoản GitHub của bạn. Không viết hộ người khác.

## 1. Thông tin học viên

- Họ tên: Nguyễn Minh Quân
- MSSV: 2A202603510
- Email trường (không bắt buộc, repo có thể để public):
- Tên nhóm: Nhom3AE
- Link repo nhóm: https://github.com/hoangtukhoi/K5-L3A-Day02-Nhom3AE-DiscoveryProblemFraming

---

## 2. Scan problem (CP1)

### Bối cảnh

**Nhân vật:** An, cố vấn dịch vụ tại một xưởng dịch vụ VinFast. Hằng ngày, An tiếp nhận nhu cầu của khách, chuẩn bị thông tin cho kỹ thuật viên và phản hồi các câu hỏi liên quan đến dịch vụ.

**Cơ sở thực tế theo đề bài:** VinFast tiếp nhận đặt lịch bảo dưỡng, sửa chữa qua website, ứng dụng và hotline. Luồng ứng dụng có chọn dịch vụ, địa điểm, thời gian và xác nhận; khách có thể bổ sung mô tả nhu cầu. Hướng dẫn công khai cũng mô tả việc xem tiến độ, báo giá và đổi/hủy lịch trên ứng dụng. [Nguồn: hướng dẫn VinFast, mục 7.1–7.2](https://vinfastauto.com/vn_vi/huong-dan-su-dung-ung-dung-vinfast).

**Phạm vi:** tìm vấn đề trong công việc tiếp nhận, chuẩn bị và trao đổi thông tin của An. Không giả định VinFast thiếu hệ thống đặt lịch hoặc các kênh đang không đồng bộ.

**Mức độ xác thực:** Các số liệu về thời gian, tần suất và dấu hiệu trong bảng dưới đây là **số liệu giả định minh họa** được ước tính sát với bối cảnh vận hành thực tế tại xưởng của An, nhằm lượng hóa quy mô vấn đề và xác định bottleneck cho từng candidate trước khi bước vào đo đạc thực tế.

### Bảng scan 10 problem theo 4 lăng kính

|   # | Lăng kính                         | Problem                                                                             | Job Story: Khi… tôi muốn… để…                                                                                                                                                                          | Ai chịu ảnh hưởng?                             | Dấu hiệu thật (thời gian, tần suất, số người, bằng chứng giả định)                                                                                                                      |
| --: | --------------------------------- | ----------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------------------------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
|   1 | Lặp lại                           | Mô tả ban đầu quá chung, An phải hỏi bổ sung nhiều lượt.                            | Khi nhận lịch sửa chữa chỉ ghi “xe có tiếng kêu”, tôi muốn làm rõ vị trí và điều kiện xuất hiện tiếng kêu, để kỹ thuật viên có thông tin cụ thể trước khi kiểm tra.                                    | An, khách hàng, kỹ thuật viên                  | ~12–15 ca/tuần chỉ ghi lỗi chung chung; An mất 2–3 lượt hỏi (12–15 phút/ca, ~3 giờ/tuần); KTV thường xuyên phản ánh thiếu chi tiết trước khi kiểm tra xe.                               |
|   2 | Tốn thời gian                     | Phải đối chiếu các lần sửa trước khi khách báo triệu chứng tái diễn.                | Khi khách nói xe gặp lại hiện tượng từng sửa, tôi muốn biết nội dung phản ánh và cách xử lý lần trước, để bàn giao đủ lịch sử liên quan cho kỹ thuật viên.                                             | An, kỹ thuật viên, khách quay lại              | ~5–7 ca/tuần xe báo lỗi tái diễn; An mất 10–15 phút/ca tìm và đối chiếu các phiếu sửa cũ; KTV phải chờ 15 phút mới có đủ lịch sử xử lý trước đó.                                        |
|   3 | Cần đọc, tổng hợp nhiều thông tin | Chưa rõ khi nào cần chuyển mô tả bất thường cho người phụ trách kỹ thuật.           | Khi yêu cầu đặt lịch có mô tả cảnh báo bất thường, tôi muốn xác định thông tin cần chuyển người có chuyên môn theo quy trình của xưởng, để khách được hướng dẫn phù hợp trước lịch hẹn.                | An, người phụ trách kỹ thuật, khách hàng       | ~3–4 ca/tuần có cảnh báo bất thường (lỗi pin, hệ thống lái); An mất 15–20 phút/ca đọc và phân vân thẩm quyền; chuyển muộn 30–45 phút khiến KTV trưởng bị động xếp khoang kỹ thuật cao.  |
|   4 | Cần đọc, tổng hợp nhiều thông tin | Dễ bỏ sót một nhu cầu khi khách nêu nhiều việc trong cùng lần đến xưởng.            | Khi khách vừa đặt bảo dưỡng vừa nhờ kiểm tra điều hòa và tiếng ồn, tôi muốn ghi nhận đầy đủ từng yêu cầu đã thống nhất, để kỹ thuật viên không bỏ sót hạng mục.                                        | An, kỹ thuật viên, khách hàng                  | ~6–8 ca/tuần khách nêu ≥3 hạng mục; An mất 8–10 phút/ca rà soát tổng hợp; ghi nhận 2–3 phiếu/tuần bị thiếu hạng mục phụ, KTV phải gọi hỏi lại khi đang làm xe.                          |
|   5 | Lặp lại                           | Tốn công xác định liên hệ trên nhiều kênh là lịch cũ hay nhu cầu mới.               | Khi khách đã đặt trên ứng dụng rồi gọi hotline để xác nhận, tôi muốn đối chiếu được với lịch hẹn tương ứng, để không ghi nhận nhầm một nhu cầu thành hai lượt dịch vụ.                                 | An, bộ phận tiếp nhận, khách hàng              | ~10–12 lượt liên hệ chéo/tuần (đặt app rồi gọi hotline xác nhận); An mất 5–7 phút/lượt tra cứu đối chiếu số điện thoại/biển số; tốn ~1 giờ/tuần chỉ để lọc trùng lịch hẹn.              |
|   6 | Pain từ người khác                | Bản chuẩn bị cho kỹ thuật viên có thể chưa phản ánh thay đổi sau xác nhận lịch.     | Khi khách đổi giờ hoặc bổ sung dịch vụ sau khi xưởng đã chuẩn bị thông tin, tôi muốn biết bản yêu cầu mới nhất và phần thay đổi, để người điều phối và kỹ thuật viên chuẩn bị đúng nội dung cuối cùng. | An, người điều phối, kỹ thuật viên, khách hàng | ~5–6 ca/tuần đổi giờ hoặc thêm hạng mục sát giờ hẹn; An mất 10–12 phút/ca tìm bản cũ để sửa; 2 ca/tuần KTV chuẩn bị nhầm vật tư theo bản chuẩn bị ban đầu.                              |
|   7 | Pain từ người khác                | Khách có thể hiểu giờ hẹn tiếp nhận là giờ hoàn thành dịch vụ.                      | Khi khách cần lấy xe trước một giờ cụ thể, tôi muốn thống nhất rõ giờ tiếp nhận và giờ trả xe dự kiến do xưởng xác nhận, để khách chủ động sắp xếp việc đi lại.                                        | Khách hàng, An, người điều phối                | ~8–10 lượt khách/tuần nhầm giờ tiếp nhận là giờ lấy xe; An mất 5–7 phút/khách giải thích và hẹn lại giờ trả xe; 3–4 phản ánh/tuần từ khách khó chịu vì trễ việc riêng 1–2 tiếng.        |
|   8 | Cần đọc, tổng hợp nhiều thông tin | Tra cứu câu trả lời dịch vụ đúng dòng xe và trường hợp áp dụng mất nhiều bước.      | Khi khách hỏi hạng mục bảo dưỡng hoặc điều kiện áp dụng dịch vụ cho xe của mình, tôi muốn tìm đúng tài liệu còn hiệu lực và phần liên quan, để trả lời có căn cứ và nhất quán.                         | An, khách hàng, người phụ trách dịch vụ        | ~12–15 câu hỏi/tuần về chính sách bảo hành/bảo dưỡng pin xe điện; An phải mở 3–4 file PDF/thông báo, tốn 8–10 phút/câu trả lời; khách phải chờ trên điện thoại hoặc tại quầy.           |
|   9 | Tốn thời gian                     | Phải xác minh thêm khi khách cần giải thích tiến độ ngoài trạng thái đang hiển thị. | Khi khách đã xem trạng thái nhưng vẫn hỏi vì sao giờ trả xe chưa được cập nhật, tôi muốn có thông tin được người phụ trách xác nhận, để phản hồi rõ ràng và không hứa sai thời điểm.                   | An, kỹ thuật viên/người điều phối, khách hàng  | ~8–10 lượt khách hỏi tiến độ/tuần khi xe quá giờ hẹn dự kiến; An mất 8–12 phút/lượt vào xưởng hỏi KTV/điều phối để xác minh lý do trước khi trả lời khách.                              |
|  10 | Pain từ người khác                | Khách chưa hiểu phần thay đổi khi có báo giá bổ sung.                               | Khi phát sinh hạng mục cần khách phê duyệt thêm, tôi muốn giải thích rõ phần việc và chi phí thay đổi so với bản đã thống nhất, để khách có đủ thông tin trước khi quyết định.                         | Khách hàng, An, kỹ thuật viên                  | ~6–8 ca/tuần phát sinh báo giá bổ sung; An mất 12–15 phút/ca gọi điện giải thích lý do thay đổi và chênh lệch chi phí; thời gian chờ khách duyệt kéo dài 30–60 phút làm nghẽn cầu nâng. |

### Ghi nhận ý do AI gợi ý

Sau khi tự scan 7 problem đầu (#1 đến #7) theo bối cảnh công việc của An, tôi dùng AI để gợi ý thêm nhằm mở rộng góc nhìn theo 4 lăng kính:

- **Ý AI gợi ý được giữ lại (3 problem cuối: #8, #9, #10):**
  - **Problem #8 (Cần đọc, tổng hợp nhiều thông tin):** _Tra cứu câu trả lời dịch vụ đúng dòng xe và trường hợp áp dụng mất nhiều bước._ Giữ lại vì phản ánh đúng khó khăn khi tra cứu tài liệu/chính sách áp dụng cho xe điện VinFast, có thể kiểm chứng qua số tài liệu cần mở và thời gian tra cứu.
  - **Problem #9 (Tốn thời gian):** _Phải xác minh thêm khi khách cần giải thích tiến độ ngoài trạng thái đang hiển thị._ Giữ lại vì dù ứng dụng đã có hiển thị trạng thái cơ bản, khách vẫn cần giải thích khi phát sinh độ trễ; đo được thời gian phối hợp nội bộ với kỹ thuật viên/người điều phối.
  - **Problem #10 (Pain từ người khác):** _Khách chưa hiểu phần thay đổi khi có báo giá bổ sung._ Giữ lại vì các hạng mục phát sinh là điểm nhạy cảm dễ gây thắc mắc, đo được qua số lượt giải thích lại và thời gian chờ khách duyệt.
  - _Lý do chung:_ Cả 3 ý đều có tình huống, actor, đầu ra và cách quan sát cụ thể để đưa vào danh sách kiểm chứng thực tế.

- **Ý AI gợi ý bị loại bỏ:**
  - Bỏ hướng _“trợ lý quản lý toàn bộ xưởng”_ vì phạm vi quá rộng, thiếu trọng tâm, không giải quyết đúng điểm nghẽn cụ thể của cố vấn dịch vụ.
  - Bỏ ý _“chưa có chức năng theo dõi tiến độ”_ vì tài liệu VinFast đã mô tả rõ ứng dụng đã có sẵn chức năng này.
  - Bỏ ý _“tự động chẩn đoán kỹ thuật”_ vì chẩn đoán lỗi kỹ thuật thuộc thẩm quyền của kỹ thuật viên/người phụ trách kỹ thuật, không phải nhiệm vụ tự quyết của An.

---

## 3. Top 3 Problem Cards (CP2)

### Bảng chọn top 3

| Rank | Problem                                                   | Vì sao chọn                                                                                                                         | Điều còn chưa chắc                                                                 |
| ---: | --------------------------------------------------------- | ----------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------- |
|    1 | Làm rõ mô tả nhu cầu trước khi bàn giao (#1)              | Gắn trực tiếp việc tiếp nhận của An; đầu ra có thể đối chiếu với nhu cầu khách; thử được checklist trong phạm vi nhỏ.               | Có bao nhiêu ca thực sự thiếu mô tả? Thời gian mất ở hỏi bổ sung hay ở chờ khách?  |
|    2 | Tra cứu câu trả lời dịch vụ đúng trường hợp (#8)          | Đại diện cho việc đọc và tổng hợp; đo được thời gian tìm nguồn và độ đúng câu trả lời; có phương án FAQ/tìm kiếm sẵn có để so sánh. | Tài liệu hiện có đã dễ tìm chưa? Khó tìm nguồn hay khó xác định điều kiện áp dụng? |
|    3 | Cập nhật bản chuẩn bị sau khi khách đổi lịch/nhu cầu (#6) | Thể hiện pain của kỹ thuật viên và điều phối; có thể đối chiếu hai phiên bản; phù hợp để đánh giá giải pháp quy trình hoặc rule.    | Hệ thống hiện có đã tự cập nhật đầy đủ chưa? Sai lệch có thật hay chỉ là giả định? |

**Nguyên tắc lựa chọn:** đây là thứ tự ưu tiên khảo sát dựa trên độ rõ và khả năng kiểm chứng, chưa phải xếp hạng impact thực tế. Chọn ba vấn đề ở ba khâu: làm rõ đầu vào, tra cứu khi tư vấn và cập nhật thay đổi trước bàn giao.

**Quy ước thời gian và metric:** tất cả số phút trong các sơ đồ dưới đây là **giả định minh họa**, không phải số liệu đo tại VinFast. Quy trình cũng là bản nháp cần An xác nhận. Baseline thực tế chưa có. Đề xuất lấy 20 ca phù hợp trước và 20 ca tương đương sau thử nghiệm cho từng card; so sánh trung vị thời gian An chủ động xử lý, đồng thời kiểm chất lượng đầu ra. Đo thời gian chờ khách hoặc người khác riêng. Các mục tiêu dưới đây cần được xem lại sau khi có baseline.

### Problem Card #1 — Làm rõ mô tả nhu cầu trước khi bàn giao

| Trường                                    | Nội dung                                                                                                                                                                                                                                                                                             |
| ----------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Job Story                                 | Khi nhận lịch sửa chữa chỉ ghi “xe có tiếng kêu”, tôi muốn làm rõ vị trí và điều kiện xuất hiện tiếng kêu, để kỹ thuật viên có thông tin cụ thể trước khi kiểm tra.                                                                                                                                  |
| Actor                                     | An, cố vấn dịch vụ tiếp nhận và chuẩn bị mô tả nhu cầu cho kỹ thuật viên.                                                                                                                                                                                                                            |
| Thời điểm / bối cảnh                      | Sau khi nhận lịch sửa chữa và trước bàn giao; chỉ xét các yêu cầu có mô tả ban đầu chưa rõ.                                                                                                                                                                                                          |
| Quy trình hiện tại (3–7 bước)             | 1. Đọc yêu cầu → 2. Xác định phần thiếu → 3. Hỏi khách bổ sung → 4. Ghi lại mô tả → 5. Xác nhận và bàn giao.                                                                                                                                                                                         |
| Bottleneck (bước nào, mất bao nhiêu phút) | Giả thuyết: bước 3, hỏi bổ sung nhiều lượt. Minh họa 5/12 phút xử lý chủ động mỗi ca; thời gian chờ khách chưa biết.                                                                                                                                                                                 |
| Impact (nếu không giải thì sao)           | Khách phải kể lại; An liên hệ nhiều lần; kỹ thuật viên có thể phải hỏi lại trước khi kiểm tra. Đo số lượt hỏi/ca, phút xử lý và tỷ lệ phiếu bị yêu cầu bổ sung. Chưa đủ dữ liệu tính tổng thiệt hại/ngày.                                                                                            |
| Success metric (baseline → target)        | Baseline: chưa đo. Target đề xuất: trung vị thời gian xử lý còn ≤ 50% baseline, minh họa 12 → 6 phút/ca; tỷ lệ phiếu cần bổ sung sau bàn giao không tăng. Kiểm các mục áp dụng: hiện tượng, vị trí, điều kiện xuất hiện, thời điểm bắt đầu, tần suất; phần khách chưa biết phải ghi “chưa xác định”. |
| Phương án không dùng AI                   | Checklist hỏi theo nhóm nhu cầu và mẫu ghi nhận thống nhất; xác nhận lại mô tả với khách trước bàn giao.                                                                                                                                                                                             |
| Giả thuyết về AI (nếu có)                 | Nếu checklist chưa đủ, thử hỗ trợ xác định thông tin còn thiếu và nháp câu hỏi từ mô tả tự do. An chọn câu hỏi và kiểm nội dung; không tự suy diễn triệu chứng hoặc chẩn đoán lỗi.                                                                                                                   |
| Cảm nhận nhanh                            | **No AI trước**. Cân nhắc Workflow có một bước AI hỗ trợ nếu dữ liệu thử cho thấy cách diễn đạt đa dạng vẫn gây nhiều công xử lý. Chưa có cơ sở cần Agent.                                                                                                                                           |

Quy trình nháp hiện tại:

```text
GIẢ ĐỊNH MINH HỌA — 12 phút xử lý chủ động/ca

[1. An đọc yêu cầu: 1 phút]
→ [2. An xác định phần thiếu: 2 phút]
→ [3. An hỏi khách bổ sung: 5 phút] ← BOTTLENECK GIẢ ĐỊNH
→ [4. An ghi mô tả: 2 phút]
→ [5. An xác nhận với khách và bàn giao: 2 phút]

Chờ khách phản hồi: chưa đo, ghi riêng.
```

### Problem Card #2 — Tra cứu câu trả lời dịch vụ đúng trường hợp

| Trường                                    | Nội dung                                                                                                                                                                                                                                                                 |
| ----------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| Job Story                                 | Khi khách hỏi hạng mục bảo dưỡng hoặc điều kiện áp dụng dịch vụ cho xe của mình, tôi muốn tìm đúng tài liệu còn hiệu lực và phần liên quan, để trả lời có căn cứ và nhất quán.                                                                                           |
| Actor                                     | An, cố vấn dịch vụ phụ trách phản hồi câu hỏi của khách.                                                                                                                                                                                                                 |
| Thời điểm / bối cảnh                      | Khách hỏi trước hoặc trong lần làm dịch vụ; chỉ xét câu hỏi có thể trả lời từ tài liệu được duyệt, không gộp ca phải kiểm tra xe hay phê duyệt ngoại lệ.                                                                                                                 |
| Quy trình hiện tại (3–7 bước)             | 1. Làm rõ câu hỏi và thông tin xe → 2. Tìm tài liệu → 3. Đối chiếu phiên bản và điều kiện áp dụng → 4. Soạn câu trả lời kèm căn cứ → 5. Kiểm tra và phản hồi.                                                                                                            |
| Bottleneck (bước nào, mất bao nhiêu phút) | Bước 2, tìm đúng đoạn tài liệu. Minh họa 4/10 phút mỗi câu.                                                                                                                                                                                                              |
| Impact (nếu không giải thì sao)           | Khách chờ; An tra đi tra lại hoặc phải đính chính; câu trả lời thiếu điều kiện có thể khiến khách hiểu sai quyền lợi hoặc phạm vi dịch vụ. Đo phút tra cứu và tỷ lệ trả lời phải sửa.                                                                                    |
| Success metric (baseline → target)        | Baseline: chưa đo. Target đề xuất: trung vị thời gian xử lý còn ≤ 50% baseline, minh họa 10 → 5 phút/câu; 100% câu trả lời trong mẫu thử có nguồn và phiên bản; tỷ lệ sai điều kiện áp dụng không tăng. Người phụ trách dịch vụ kiểm đáp án theo nguồn đang có hiệu lực. |
| Phương án không dùng AI                   | Kho tài liệu được duyệt, mục lục theo dòng xe/chủ đề, FAQ gắn nguồn và người cập nhật; dùng chức năng tìm kiếm sẵn có trước.                                                                                                                                             |
| Giả thuyết về AI (nếu có)                 | Hỗ trợ tìm đoạn liên quan và nháp câu trả lời có dẫn nguồn trong kho được phép dùng. An kiểm nguồn và điều kiện trước khi phản hồi. Không tìm thấy căn cứ thì chuyển người phụ trách xác nhận.                                                                           |
| Cảm nhận nhanh                            | **No AI/Rule trước** để tổ chức và lọc nguồn. Chỉ thử Workflow có hỗ trợ ngôn ngữ nếu cách đơn giản chưa đạt metric; không cần Agent tự đưa cam kết với khách.                                                                                                           |

Quy trình nháp hiện tại:

```text
GIẢ ĐỊNH MINH HỌA — 10 phút xử lý chủ động/câu

[1. An làm rõ câu hỏi và thông tin xe: 1 phút]
→ [2. An tìm tài liệu: 4 phút] ← BOTTLENECK GIẢ ĐỊNH
→ [3. An đối chiếu hiệu lực và điều kiện: 2 phút]
→ [4. An soạn câu trả lời kèm căn cứ: 2 phút]
→ [5. An kiểm tra và phản hồi: 1 phút]

Ca cần người có thẩm quyền xác nhận: theo dõi riêng.
```

### Problem Card #3 — Cập nhật bản chuẩn bị sau khi khách đổi lịch/nhu cầu

| Trường                                    | Nội dung                                                                                                                                                                                                                                                       |
| ----------------------------------------- | -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Job Story                                 | Khi khách đổi giờ hoặc bổ sung dịch vụ sau khi xưởng đã chuẩn bị thông tin, tôi muốn biết bản yêu cầu mới nhất và phần thay đổi, để người điều phối và kỹ thuật viên chuẩn bị đúng nội dung cuối cùng.                                                         |
| Actor                                     | An, cố vấn dịch vụ cập nhật thông tin cho người điều phối và kỹ thuật viên phụ trách lịch hẹn.                                                                                                                                                                 |
| Thời điểm / bối cảnh                      | Sau lần xác nhận đầu và trước tiếp nhận xe; chỉ xét ca có thay đổi ảnh hưởng bản chuẩn bị đã lập. Không giả định dữ liệu gốc chưa đồng bộ.                                                                                                                     |
| Quy trình hiện tại (3–7 bước)             | 1. Nhận thay đổi và xác định đúng lịch hẹn → 2. Đối chiếu yêu cầu mới với bản chuẩn bị → 3. Xác nhận phần thay đổi với khách/người điều phối → 4. Cập nhật bản chuẩn bị → 5. Bàn giao thay đổi và kiểm người phụ trách đã nhận.                                |
| Bottleneck (bước nào, mất bao nhiêu phút) | Giả thuyết: bước 2, đối chiếu các phiên bản để tìm phần phải cập nhật. Minh họa 4/10 phút xử lý chủ động mỗi ca; thời gian chờ điều phối xác nhận tính riêng.                                                                                                  |
| Impact (nếu không giải thì sao)           | Kỹ thuật viên hoặc điều phối có thể chuẩn bị theo giờ/hạng mục cũ; An phải sửa và bàn giao lại; khách phải nhắc lại yêu cầu đã bổ sung. Đo số bản chuẩn bị lệch với xác nhận cuối và số lần phải làm lại.                                                      |
| Success metric (baseline → target)        | Baseline: chưa đo. Target đề xuất: trung vị thời gian cập nhật còn ≤ 50% baseline, minh họa 10 → 5 phút/ca; 100% bản chuẩn bị trong mẫu thử khớp giờ hẹn và hạng mục đã xác nhận cuối cùng trước bàn giao. Kiểm thêm số lần phải sửa lại, không chỉ đo tốc độ. |
| Phương án không dùng AI                   | Một nguồn ghi nhận chính thức cho mỗi lịch hẹn; mẫu cập nhật ghi rõ trước/sau, thời điểm và người xác nhận; checklist báo thay đổi cho người phụ trách. Tận dụng lịch sử sửa đổi và thông báo sẵn có nếu có.                                                   |
| Giả thuyết về AI (nếu có)                 | Chỉ cân nhắc hỗ trợ trích phần thay đổi khi khách bổ sung bằng văn bản dài. An xác nhận trước khi sửa hồ sơ; không tự đổi giờ, thêm hạng mục hoặc hứa khả năng đáp ứng của xưởng.                                                                              |
| Cảm nhận nhanh                            | **Rule**, nếu dữ liệu thay đổi có cấu trúc và hệ thống cho phép; **No AI** với quy trình đối chiếu/checklist nếu số ca ít. Nếu hệ thống hiện có đã xử lý đủ thì không xây thêm. Chưa có lý do cần Agent.                                                       |

Quy trình nháp hiện tại:

```text
GIẢ ĐỊNH MINH HỌA — 10 phút xử lý chủ động/ca thay đổi

[1. An nhận thay đổi và xác định lịch hẹn: 1 phút]
→ [2. An đối chiếu với bản chuẩn bị: 4 phút] ← BOTTLENECK GIẢ ĐỊNH
→ [3. An xác nhận phần thay đổi: 2 phút]
→ [4. An cập nhật bản chuẩn bị: 2 phút]
→ [5. An bàn giao và kiểm đã nhận: 1 phút]

Chờ khách/người điều phối xác nhận: chưa đo, ghi riêng.
```

### Card đề xuất để pitch

- **Card số 1:** làm rõ mô tả nhu cầu trước bàn giao.
- **Lý do:** sát công việc tiếp nhận của An; có đầu ra để kiểm tra; phạm vi nhỏ; thử checklist trước khi cân nhắc công cụ phức tạp.
- **Câu hỏi muốn nhóm phản biện:** Nếu dùng checklist mà kỹ thuật viên vẫn phải hỏi lại, vấn đề nằm ở dữ kiện khách chưa cung cấp hay cách An bàn giao chưa rõ?

### AI tự phản biện và điều chỉnh bản nháp

| Điểm yếu AI chỉ ra                                                          | Đánh giá trong bản nháp           | Đã sửa gì                                                                                                        |
| --------------------------------------------------------------------------- | --------------------------------- | ---------------------------------------------------------------------------------------------------------------- |
| Bối cảnh đặt lịch chưa chứng minh các pain thực sự xảy ra tại xưởng của An. | Có cơ sở.                         | Ghi cả 10 ý là candidate; thêm hồ sơ cần đối chiếu và phép đo; không tạo kết quả khảo sát.                       |
| Số phút có thể bị hiểu nhầm là số đo thực tế.                               | Có cơ sở.                         | Gắn nhãn giả định ở cả 3 sơ đồ; baseline để “chưa đo”; tách thời gian xử lý và chờ.                              |
| Card #1 có thể chỉ cần checklist; card #2 có thể chỉ cần mục lục tài liệu.  | Cần thử phương án đơn giản trước. | Đưa No AI/Rule làm bước thử đầu; AI chỉ là giả thuyết khi cách đơn giản chưa đạt metric.                         |
| Card #3 có thể đã được hệ thống sẵn có xử lý đầy đủ.                        | Chưa biết, phải kiểm tra.         | Thêm điều kiện loại candidate nếu bản chuẩn bị đã được cập nhật đầy đủ; không khẳng định các kênh không đồng bộ. |
| Làm nhanh hơn nhưng bàn giao thiếu hoặc tư vấn sai thì chưa thành công.     | Metric tốc độ chưa đủ.            | Thêm kiểm chất lượng cho cả 3 card: mức đầy đủ, căn cứ trả lời và khớp phiên bản xác nhận cuối.                  |

_Đây là AI tự rà soát nội dung, không phải kết quả phản biện của nhóm hoặc xác nhận từ An. Học viên cần tự kiểm tra, chọn lại và bổ sung bằng chứng thực tế._

---

## 4. Tôi đã tham gia phần nào (CP3 → CP7)

| Hoạt động                  | Tôi đã làm gì?                                                                                                                                                                                                                                                                                                                                                                                                                             | Kết quả / ảnh hưởng tới bài nhóm                                                                                                                         |
| -------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | -------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Pitch Problem Card         | Trình bày 3 candidate: làm rõ mô tả nhu cầu trước khi bàn giao; tra cứu câu trả lời dịch vụ đúng trường hợp; cập nhật bản chuẩn bị sau khi khách đổi lịch/nhu cầu.                                                                                                                                                                                                                                                                         | Đóng góp 3 candidate để nhóm so sánh. Candidate làm rõ mô tả nhu cầu trước khi bàn giao được nhóm lựa chọn để đào sâu.                                   |
| Phản biện bài của bạn khác | **Các câu hỏi tôi đặt cho Nguyễn Đức Minh:**<br>1. Lần gần nhất việc bàn giao chỉ bằng hỏi lại ca trước khiến bạn bỏ sót công việc là khi nào, và hậu quả cụ thể là gì?<br>2. Vì sao trưởng ca phải viết lại sự cố vào cuối ca, thông tin chưa được ghi nhận hay đã có nhưng nằm rải rác?<br>3. Người mới hỏi lại vì chưa có tài liệu, khó tìm tài liệu hay tài liệu có nhưng khó hiểu?                                                    | Giúp xác định bottleneck rõ ràng hơn và hiểu rõ Job Story của các candidate được trình bày.                                                              |
| Nhận phản biện             | **Các câu hỏi tôi nhận từ Nguyễn Đức Minh:**<br>1. Thông tin hay thiếu nhất là gì: triệu chứng, đời xe hay số km? Nếu luôn thiếu đúng mấy mục đó thì thêm ô bắt buộc vào form đặt lịch đã đủ chưa?<br>2. Khách hỏi lặp lại cùng các câu hay mỗi lần một khác? Tài liệu dịch vụ dài bao nhiêu trang mà phải mất công tìm?<br>3. Khách đổi lịch hoặc đổi nhu cầu mấy lần một tuần? Nếu ít thì đối chiếu bằng tay có thật sự là vấn đề không? | Tôi xác định bottleneck rõ ràng hơn, hiểu rõ nhu cầu trong từng Job Story và những điểm còn cần kiểm chứng.                                              |
| Gom cluster / cây OST      | Gom 12 candidate thành 3 cụm; xây cây OST với outcome giảm thời gian tiếp nhận và số lần hỏi lại; tách các ý tưởng giải pháp khỏi tầng opportunity.                                                                                                                                                                                                                                                                                        | Giúp nhóm nhìn ra pattern chung, phân biệt vấn đề với giải pháp và thu hẹp phạm vi thảo luận.                                                            |
| Chọn candidate problem     | Tham gia chấm điểm shortlist theo 7 tiêu chí, thảo luận lựa chọn candidate và lý do loại các candidate còn lại.                                                                                                                                                                                                                                                                                                                            | Nhóm chọn bài toán cố vấn phải hỏi lại khách nhiều đợt vì mô tả nhu cầu lúc đặt lịch chưa đủ rõ.                                                         |
| Kiểm chứng / research      | Thu thập tư liệu công khai trên DealerELITE về việc ghi nhận mô tả nhu cầu của khách; tổng hợp thành snapshot 3 trong phần kiểm chứng.                                                                                                                                                                                                                                                                                                     | Bổ sung ví dụ về mô tả mơ hồ khiến KTV phải kiểm tra thêm để hiểu đúng vấn đề; cung cấp tư liệu cho nhóm xem xét cách hỏi bổ sung và ghi nhận thông tin. |
| Quy trình nhóm             | Cùng đọc quy trình hiện tại, quy trình tương lai và đóng góp ý kiến trong thảo luận.                                                                                                                                                                                                                                                                                                                                                       | Góp phần rà soát quy trình và thống nhất cách mô tả các bước trong bài nhóm.                                                                             |
| Problem Statement          | Cùng đọc Problem Statement v0, v1 và đóng góp ý kiến cho nội dung mô tả bài toán.                                                                                                                                                                                                                                                                                                                                                          | Góp phần rà soát và thống nhất cách trình bày Problem Statement của nhóm.                                                                                |
| Mức can thiệp AI           | Cùng đọc, thảo luận và góp ý về các phương án No AI, Rule, Workflow và Agent.                                                                                                                                                                                                                                                                                                                                                              | Cùng nhóm thống nhất hướng Workflow có cố vấn kiểm tra đầu ra, đồng thời thử Rule trước khi thêm AI.                                                     |
| Quyết định                 | Tham gia thảo luận và cùng nhóm quyết định lựa chọn **Not Yet**.                                                                                                                                                                                                                                                                                                                                                                           | Nhóm thống nhất chưa triển khai ngay; cần bổ sung bằng chứng tại Việt Nam, xác minh quyền xử lý dữ liệu và thử phương án Rule trước khi thêm AI.         |

---

## 5. Dùng AI

| Checkpoint                     | Tôi dùng AI để làm gì?                                                                                                                              | AI hữu ích ở đâu?                                                                                                              | AI sai hoặc hời hợt ở đâu?                                                                                              | Tôi sửa gì bằng nhận định của mình?                                                                                                            |
| ------------------------------ | --------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------ | ----------------------------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------- |
| CP1 Scan                       | Sau khi tự scan 7 problem đầu, dùng AI gợi ý thêm mở rộng 4 lăng kính; chọn giữ lại 3 problem cuối (#8, #9, #10).                                   | Bổ sung góc nhìn về tra cứu chính sách, giải thích tiến độ và báo giá bổ sung; gắn với cách đo cụ thể.                         | Đề xuất một số ý quá rộng (quản lý toàn xưởng) hoặc không đúng thực tế (tự chẩn đoán kỹ thuật, thiếu theo dõi tiến độ). | Lọc bỏ các ý sai thẩm quyền hoặc hệ thống đã có; chỉ giữ lại 3 problem (#8, #9, #10) để đưa vào kiểm chứng thực tế.                            |
| CP2 Problem Card               | AI soạn bản nháp 3 card và tự rà soát điểm yếu.                                                                                                     | Cụ thể hóa bước nghẽn, metric, quy trình và phương án không dùng AI.                                                           | Quy trình và thời gian chỉ là giả định; chưa biết hệ thống nội bộ đang hỗ trợ đến đâu.                                  | Chưa có sửa đổi của học viên; cần xác nhận từng bước và thay số minh họa bằng số đo.                                                           |
| CP4 Research                   | Dùng AI hỗ trợ tìm nguồn công khai về vấn đề tiếp nhận nhu cầu khách và các giải pháp liên quan; rà soát bằng chứng có phù hợp với giả định không.  | Hỗ trợ tìm tư liệu DealerELITE và nhận diện thông tin liên quan đến mô tả nhu cầu mơ hồ, cách hỏi bổ sung và bàn giao cho KTV. | Nguồn công khai ở nước ngoài chưa đủ để xác nhận tỷ lệ lịch đặt thiếu thông tin tại Việt Nam.                           | Phân biệt tư liệu công khai với phỏng vấn trực tiếp; giữ trạng thái chưa xác nhận cho giả định về tỷ lệ lịch đặt thiếu thông tin tại Việt Nam. |
| CP5 Quy trình                  | Tìm thông tin tham khảo về tiếp nhận xe; dùng AI kiểm tra tính nhất quán giữa quy trình hiện tại, quy trình tương lai và bottleneck.                | Hỗ trợ rà soát vị trí bước nghẽn, bước cố vấn kiểm tra và phương án quay về khi đầu ra AI không phù hợp.                       | Chưa ghi nhận lỗi cụ thể; AI không có dữ liệu thực tế để xác nhận thời gian hoặc cách vận hành của xưởng.               | Cùng nhóm đọc và góp ý quy trình; giữ rõ thời gian là ước lượng, chưa xem mức giảm thời gian kỳ vọng là kết quả đã đạt.                        |
| CP5–6 Problem Statement        | Dùng AI kiểm tra các điểm xung đột giữa Problem Statement v0, v1 với quy trình, metric và boundary.                                                 | Hỗ trợ đối chiếu xem actor, bottleneck, chỉ số và giới hạn của AI có thống nhất giữa các CP không.                             | Chưa ghi nhận lỗi cụ thể; việc rà soát bằng AI chưa xác nhận được baseline và mức khả thi của target.                   | Cùng nhóm đọc, góp ý và thống nhất nội dung; phân biệt số liệu cần đo với mục tiêu dự kiến, giữ vai trò kiểm tra của cố vấn.                   |
| CP6 Mức can thiệp / quyết định | Tìm thông tin liên quan đến No AI, Rule, Workflow và Agent; dùng AI kiểm tra mức can thiệp, rủi ro và quyết định có nhất quán với bằng chứng không. | Hỗ trợ rà soát lý do chọn Workflow, điều kiện dừng ở Rule và sự phù hợp của quyết định Not Yet.                                | Chưa ghi nhận lỗi cụ thể; AI không thể xác nhận thay nhóm về quy định dữ liệu nội bộ hoặc hiệu quả triển khai thực tế.  | Tham gia thảo luận và cùng nhóm chọn Not Yet; thống nhất cần bổ sung bằng chứng, xác minh quyền xử lý dữ liệu và thử Rule trước khi thêm AI.   |

---

## 6. Reflection (CP7)

Trả lời bằng trải nghiệm thật của bạn, tối thiểu 200 từ cho các câu 6.1–6.6 (không tính 6.7, câu này được chấm riêng ở tiêu chí C5). **Không dùng AI để viết thay.**

**6.1. Tôi học được gì khi nghe top 3 problems của các bạn khác?**

Khi nghe 3 problem của các bạn khác, có bài toán ứng với từng vấn đề rất rời rạc, rất khó để giải quyết nó. Khi gom cụm tìm các pattern chung giúp việc tìm giải phát rõ ràng hơn khi có nhiều bài toán

**6.2. Nhóm có lúc nào bị "solution-first" (nghĩ giải pháp trước khi hiểu vấn đề) không? Lúc đó nhóm nhận ra và xử lý thế nào?**

Nhóm em nhận ra “đồng bộ booking thành lệnh sửa chữa”, “trích xuất điều khoản bảo hành” đã chứa cách giải. Lúc đó cần đi từ pain thực tế của người dùng trước khi nghĩ đến giải pháp.

**6.3. Tôi có đổi ý sau khi bị phản biện không? Kể một lần cụ thể.**

Có.Khi Minh hỏi: "Người mới hỏi lại vì chưa có tài liệu, khó tìm tài liệu hay tài liệu có nhưng khó hiểu?"
Tôi đã xác định vấn đề rõ ràng hơn, nắm được rõ hơn bottleneck nằm ở bước nào, pain ở đâu.

**6.4. Kết quả kiểm chứng (phỏng vấn/survey/research) có làm tôi bất ngờ không? Điều gì?**

Kết quả research về tài liệu của DealerELITE làm em bất ngờ vì vấn đề thật sự là do cách mà 1 người hỏi và ghi phiếu báo cáo

**6.5. Điều khó nhất khi viết Problem Statement là gì?**

Điều khó nhất là xác định metrics khi viết Problem Statement

**6.6. Nếu làm lại, tôi sẽ đổi gì? Tôi sẽ phản biện nhóm mạnh hơn ở điểm nào?**

Nếu làm lại, em sẽ tìm người từng đặt lịch sửa xe hoặc cố vấn dịch vụ để hỏi sớm hơn. Lần này, nhóm chủ yếu dựa vào tư liệu công khai ở nước ngoài nên vẫn chưa biết vấn đề xảy ra thường xuyên đến đâu tại Việt Nam. Tôi cũng sẽ hỏi kỹ hơn: nếu thêm vài ô bắt buộc vào form đã đủ thì vì sao cần AI? Ngoài ra, tôi muốn nhóm làm rõ nguồn của các con số về thời gian, phân biệt số ước lượng với số đã đo để tránh đặt mục tiêu thiếu cơ sở.

**6.7. Hiểu bài:** giải thích bằng 5–8 câu, không nhìn tài liệu, chuỗi _problem → quy trình → metric → boundary → mức can thiệp AI → quyết định_ của bài nhóm mình.

Bài toán nhóm chọn là cố vấn dịch vụ phải hỏi lại khách nhiều đợt vì mô tả nhu cầu lúc đặt lịch chưa đủ rõ để bàn giao cho kỹ thuật viên. Quy trình hiện tại đi từ đọc lịch đặt, hỏi bổ sung, ghi phiếu, xác nhận với khách đến tạo lệnh sửa chữa và bàn giao. Bước nghẽn nằm ở việc hỏi bổ sung, nhưng thời gian nhóm đưa ra vẫn là ước lượng, cần đo thực tế để có baseline. Nhóm dự kiến đo số lần gọi lại, số lần kỹ thuật viên hỏi lại cố vấn và tỷ lệ câu hỏi AI bị bỏ, với mục tiêu như tối đa một lần gọi bổ sung mỗi lịch và giảm 50% số lần kỹ thuật viên hỏi lại. AI chỉ được gợi ý câu hỏi và soạn nháp để cố vấn duyệt, không tự liên hệ khách, chẩn đoán, báo giá, kết luận bảo hành hoặc sửa thông tin khách đã điền. Hướng dự kiến là Workflow vì các bước đã cố định, nhưng nhóm sẽ thử Rule trước và chỉ thêm AI nếu cách đơn giản hơn chưa đủ. Nhóm quyết định Not Yet vì còn thiếu bằng chứng tại Việt Nam và chưa xác nhận công ty có cho phép xử lý dữ liệu khách bằng công cụ bên ngoài hay không.

---
