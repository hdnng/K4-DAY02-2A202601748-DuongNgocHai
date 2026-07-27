
## Scan rộng
| # | Lăng kính | Problem quan sát được | Ai chịu ảnh hưởng? | Dấu hiệu thật |
|---|---|---|---|---|
| 1 | Tốn thời gian | Chưa kiểm soát được thời gian, thói quen hàng ngày | các bạn sinh viên, đại học từ 19 đến 24 tuổi | mỗi ngày trôi qua cảm tưởng như không đủ, có quá nhiều công việc bị dồn dập |
| 2 | Lặp lại| Ăn uống thiếu khoa học, thiếu ngủ| các bạn sinh viên đại học từ 19 đến 24 tuổi | người dễ mệt mỏi, buồn ngủ  |
| 3 | Lặp lại | chưa kiểm soát được dòng tiền | Các bạn sinh viên mới lên Đại học, xa gia đình | tiêu tiền không kiểm soát |
| 4 | Tốn thời gian | mất tập trung, hay quên mất điều cần làm khi thấy nội dung mới | giới trẻ dùng mạng xã hội | quên mất điều cần làm |
| 5 | AI có thể tốt hơn | Nhiều học sinh gian lận, coi cóp bài  | Giáo viên nhà trường | chất lượng học lực giảm mặc dù điểm số cao |
| 6 | Tốn thời gian | Tìm kiếm và tổng hợp tài liệu ôn thi rải rác trên nhiều nguồn | Sinh viên đại học | Mất hàng giờ trước kỳ thi để xin link tải, lọc tài liệu trùng hoặc cũ |
| 7 | AI có thể tốt hơn | Loay hoay lên ý tưởng và dàn ý cho bài thuyết trình nhóm | Nhóm sinh viên | Mất cả buổi họp đầu tiên chỉ để chốt dàn ý sơ sài |
| 8 | Lặp lại | Nhắc nhở và theo dõi tiến độ công việc của các thành viên trong nhóm | Trưởng nhóm / Sinh viên làm leader | Phải nhắn tin giục liên tục, thường xuyên trễ tiến độ chung |
| 9 | Pain từ người khác | Bỏ lỡ thông báo quan trọng từ trường/giảng viên do quá nhiều email/tin nhắn rác | Sinh viên | Đi học nhầm lịch  hoặc quên nộp bài |

## Top 3

| Rank | Problem | Vì sao chọn | Điều còn chưa chắc |
|---|---|---|---|
| 1 | Nhiều học sinh gian lận, coi cóp bài | Workflow rõ, mất nhiều thời gian, có metric tốt | Dữ liệu của học sinh, nhà trường chưa có AI |
| 2 | Chưa kiểm soát được dòng tiền | Pain phổ biến, có workflow (thu/chi) rõ, AI tự phân loại tốt từ ảnh/text | Dữ liệu cá nhân nhạy cảm, nhiều giao dịch tiền mặt khó tracking |
| 3 | Chưa kiểm soát được thời gian, thói quen hàng ngày | Rất nhiều sinh viên gặp phải, impact lớn nếu giải quyết được | Phụ thuộc vào kỷ luật bản thân, khó đo lường chính xác improvement |

## Problem Card #1 — Học sinh gian lận, coi cóp bài
 
**Problem 1 câu:**  
Giám thị phòng thi không thể bao quát toàn bộ lớp học cùng lúc bằng mắt thường, dẫn đến việc mất nhiều công sức quan sát nhưng vẫn bỏ lọt các hành vi gian lận (quay cóp, trao đổi tài liệu) trong giờ kiểm tra.

**Actor:**  
Giám thị phòng thi / Giáo viên coi thi.

**Thời điểm / bối cảnh:**  
Trực tiếp trong giờ thi / kiểm tra định kỳ tại lớp học.

**Current workflow:**

```text
1. Giám thị phát đề và bắt đầu tính giờ làm bài.
2. Giám thị liên tục đi lại hoặc ngồi trên bục giảng để quan sát học sinh.
3. Nếu phát hiện bằng mắt thường các hành vi khả nghi (nhìn bài bạn, cúi xuống ngăn bàn), giám thị tiến lại gần kiểm tra.
4. Thu giữ tài liệu hoặc lập biên bản nếu bắt quả tang gian lận.
5. Thu bài khi hết giờ.
```

**Bottleneck:**  
Bước 2 tốn rất nhiều năng lượng và sự tập trung của giám thị (không thể nhìn 30-40 học sinh cùng lúc). Học sinh thường canh lúc giám thị quay đi hoặc nhìn hướng khác để gian lận, khiến việc phát hiện rất khó khăn và dễ bị lọt.

**Impact:**  
Tỷ lệ bỏ lọt gian lận cao gây bất công về điểm số. Giám thị chịu áp lực tâm lý và mệt mỏi vì phải căng thẳng quan sát liên tục trong suốt 45-90 phút.

**Success metric:**  
Giảm 80% thời gian giám thị phải đi lại quan sát thủ công; cảnh báo ngay lập tức (dưới 3 giây) khi có các tư thế bất thường xảy ra.

**Non-AI alternative:**  
Tăng cường số lượng giám thị lên 3-4 người/phòng thi (tốn chi phí nhân sự), hoặc lắp camera thông thường (nhưng giám thị vẫn phải tự nhìn chằm chằm vào màn hình rất mỏi mắt).

**AI hypothesis:**  
Sử dụng hệ thống Computer Vision (AI Camera) phân tích luồng video phòng thi theo thời gian thực (real-time) để nhận diện các tư thế/hành động bất thường (quay ngang dọc, che bài, trao đổi vật thể), từ đó khoanh vùng (red box) và gửi cảnh báo (alert) lên màn hình giám thị ngay lập tức.

**Quick gut:**  
Workflow / Rule. (AI đóng vai trò cảnh báo như một sensor tự động, giám thị đưa ra quyết định cuối cùng).

### Draft current workflow

```text
CURRENT STATE — 90 phút (suốt giờ thi)

[1 Phát đề và tính giờ: 5']
→ [2 Liên tục đi lại và quan sát lớp học bằng mắt: 80'] <-- bottleneck (không bao quát hết, mệt mỏi)
→ [3 Thấy hành vi khả nghi và đến tận nơi kiểm tra: 2']
→ [4 Lập biên bản nếu bắt quả tang: 3']
```

### Draft future workflow

```text
FUTURE STATE — 90 phút (Bao quát 100%, giám thị nhàn hơn)

[1 Phát đề và bật hệ thống Camera AI giám sát: 5']
→ [2 Giám thị ngồi xem màn hình trung tâm, làm việc khác: 80']
→ [3 AI Camera phát hiện hành vi lạ và bắn cảnh báo đỏ trên màn hình: 0']
→ [4 Giám thị xem màn hình, quyết định đi xuống đúng vị trí đó để kiểm tra: 2'] <-- human boundary
→ [5 Lập biên bản nếu đúng là có gian lận: 3']
```

---

## Problem Card #2 — Chưa kiểm soát được dòng tiền

**Problem 1 câu:**  
Sinh viên đại học xa nhà thường tiêu tiền không kiểm soát và lười ghi chép chi tiêu nhỏ lẻ hàng ngày, dẫn đến việc thiếu hụt ngân sách vào cuối tháng mà không rõ lý do.

**Actor:**  
Sinh viên đại học mới xa gia đình, có ngân sách giới hạn.

**Thời điểm / bối cảnh:**  
Mỗi lần phát sinh giao dịch mua sắm, ăn uống (cả tiền mặt lẫn chuyển khoản) và thời điểm đối chiếu tài chính cuối tháng.

**Current workflow:**

```text
1. Phát sinh giao dịch (mua đồ ăn, trả tiền nước...).
2. Quên ghi chép lại hoặc lưu trữ hóa đơn rời rạc.
3. Cuối tháng kiểm tra số dư thẻ hoặc ví thì thấy hết tiền.
4. Cố gắng nhớ lại đã tiêu gì nhưng không thể.
5. Cảm thấy hoang mang và phải xin thêm tiền gia đình.
```

**Bottleneck:**  
Bước 2. Việc mở app quản lý chi tiêu và nhập liệu thủ công cho từng cốc trà đá/bát phở tốn thời gian, dễ gây chán nản và từ bỏ thói quen ghi chép.

**Impact:**  
Thâm hụt ngân sách hàng tháng, tạo thói quen tài chính xấu. Mất nhiều thời gian suy nghĩ/nhớ lại nhưng không ra kết quả.

**Success metric:**  
Giảm thời gian ghi chép mỗi giao dịch xuống dưới 10 giây; đảm bảo track được >90% chi phí thực tế hàng tháng.

**Non-AI alternative:**  
Chỉ thanh toán qua ngân hàng (dùng lịch sử giao dịch ngân hàng làm sao kê), bỏ qua các khoản tiền mặt, lập file Excel cuối tháng copy vào.

**AI hypothesis:**  
Sử dụng AI OCR kết hợp NLP để đọc hình ảnh (hóa đơn, ảnh chụp) hoặc text (tin nhắn OTP, sao kê), tự động trích xuất số tiền, nội dung và tự động phân loại (categorize) vào các nhóm (Ăn uống, Giải trí) trên hệ thống quản lý.

**Quick gut:**  
Workflow / Rule.

### Draft current workflow

```text
CURRENT STATE — Nhiều giờ/tháng (nhưng thường bị skip)

[1 Phát sinh chi tiêu]
→ [2 Nhớ mở app và gõ từng mục: 2'] <-- bottleneck
→ [3 Phân loại hạng mục thủ công: 1']
→ [4 Tổng hợp cuối tháng (nhớ lại các khoản sót): 30']
```

### Draft future workflow

```text
FUTURE STATE — Dưới 1 phút/giao dịch

[1 Chụp ảnh hóa đơn hoặc forward tin nhắn OTP/chuyển khoản cho AI Bot: 10s]
→ [2 AI tự động extract số tiền và phân loại hạng mục: 0']
→ [3 User mở Dashboard xem báo cáo tự động cuối tháng: 5'] <-- human boundary (chỉ cần review)
```

---

## Problem Card #3 — Chưa kiểm soát được thời gian, thói quen hàng ngày

**Problem 1 câu:**  
Sinh viên đại học thường xuyên bị xao nhãng bởi mạng xã hội và thiếu kỹ năng lập kế hoạch, dẫn đến việc thời gian trôi qua không hiệu quả và công việc bị dồn ứ sát deadline.

**Actor:**  
Sinh viên đại học từ 19-24 tuổi.

**Thời điểm / bối cảnh:**  
Mỗi ngày khi bắt đầu lên kế hoạch làm việc/học tập hoặc khi đang thực hiện một task dài.

**Current workflow:**

```text
1. Nhận các deadline bài tập/hoạt động ngoại khóa.
2. Nghĩ trong đầu hoặc ghi chú sơ sài các việc cần làm.
3. Bắt đầu làm nhưng có thông báo điện thoại nên mở ra xem.
4. Lướt mạng xã hội quên thời gian (vài tiếng).
5. Cuối ngày hối hiện vì chưa làm được gì, công việc dồn sang ngày mai.
```

**Bottleneck:**  
Bước 3 và 4. Việc không có người nhắc nhở/không có kế hoạch block thời gian cụ thể khiến người dùng dễ dàng bị cuốn vào các xao nhãng.

**Impact:**  
Công việc luôn trong tình trạng gấp gáp, mệt mỏi, thiếu ngủ vì chạy deadline sát giờ, kết quả học tập không như ý.

**Success metric:**  
Tăng số giờ làm việc tập trung không ngắt quãng (Deep work) lên 2-3h/ngày. Hoàn thành >80% to-do list đặt ra mỗi ngày.

**Non-AI alternative:**  
Sử dụng phương pháp Pomodoro truyền thống, dùng app block các trang web mạng xã hội, lên lịch chi tiết bằng sổ tay.

**AI hypothesis:**  
AI đóng vai trò như một trợ lý cá nhân (Agent), trò chuyện vào mỗi sáng để cùng user lên lịch (Time-blocking), theo dõi tiến độ qua đoạn chat, và có thể gửi tin nhắn "thúc giục/nhắc nhở" khi thấy user có dấu hiệu lười biếng hoặc không check-in đúng hẹn.

**Quick gut:**  
Agent (trợ lý cá nhân tương tác linh hoạt theo context và phản hồi của người dùng).

### Draft current workflow

```text
CURRENT STATE — Hàng giờ lãng phí mỗi ngày

[1 Lên list việc cần làm trong đầu: 5']
→ [2 Ngồi vào bàn học: 5']
→ [3 Lướt điện thoại khi gặp bài khó: 120'] <-- bottleneck
→ [4 Chạy deadline trong lo âu: 60']
```

### Draft future workflow

```text
FUTURE STATE — Giảm xao nhãng, tăng tập trung

[1 Chat với AI Agent để lên lịch các block thời gian trong ngày: 5']
→ [2 AI tự động nhắc nhở khi đến giờ học: 0']
→ [3 User làm bài (Deep work) và báo cáo hoàn thành cho AI: 90']
→ [4 Nếu user không báo cáo, AI gửi tin nhắn nhắc nhở/thúc giục: 0'] <-- Agent action
```
