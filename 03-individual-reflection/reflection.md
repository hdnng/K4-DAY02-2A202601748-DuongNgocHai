## Đóng góp của Hải (Dương Ngọc Hải) trong nhóm

| Hoạt động | Hải đã làm gì? | Kết quả |
|---|---|---|
| Scan cá nhân | Đưa ra 9 problems từ báo cáo cá nhân, trong đó nổi bật là bài toán phát hiện gian lận thi cử | Nhóm có nhiều candidate về reporting/workflow |
| Pitch | Đề xuất bài toán "Camera CV phát hiện gian lận thi cử" | Bài toán được đưa vào danh sách đánh giá chung (Candidate 3) |
| Đánh giá & Challenge | Đánh giá chéo các bài toán, tự nhận thấy rủi ro của bài CV | Cùng nhóm đi đến quyết định loại bài toán CV do vấn đề quyền riêng tư và thiếu dữ liệu test trong lab |
| Đề xuất giải pháp (Role) | Đảm nhận vai trò "Đề xuất giải pháp", cùng nhóm xây dựng Workflow cho bài toán Ngân hàng đề thi | Góp phần định hình cách dùng AI để đọc giáo trình, phác thảo đề và giảng viên review |
| Rule / Workflow / Agent | Tham gia lập luận để chọn mức Workflow thay vì Agent cho bài toán Ngân hàng đề | Nhóm chốt được boundary an toàn: AI chỉ phác thảo, không tự đẩy đề vào hệ thống CSDL |

## Bảng dùng AI trong quá trình làm bài

| Phase | Tôi dùng AI để làm gì? | AI hữu ích ở đâu? | AI sai/hời hợt ở đâu? | Tôi sửa gì |
|---|---|---|---|---|
| Scan (Cá nhân) | Nhờ AI hoàn thiện Problem Card và vẽ luồng xử lý (Before/After) | Giúp định hình cấu trúc văn bản nhanh chóng, logic | Ban đầu AI gợi ý hướng check đạo văn bằng text sau giờ thi | Chủ động prompt yêu cầu AI viết lại theo hướng xử lý realtime bằng Camera CV |
| Đánh giá nhóm | Nhờ AI phân tích rủi ro của việc dùng Camera giám sát trong trường học | Nêu bật được rủi ro quyền riêng tư và khả năng khả thi | Gợi ý xử lý bằng các giải pháp kỹ thuật quá phức tạp | Chỉ lấy ý "rủi ro quyền riêng tư" làm luận điểm để loại bài toán cá nhân |
| Problem Statement | Dùng AI hỗ trợ viết phần "Workflow Before/After" cho báo cáo chung của nhóm | Chuyển luồng suy nghĩ thành các bước rõ ràng, có time estimate | Đôi khi gộp các bước review của con người vào chung với bước xử lý của AI | Tách bạch rõ ranh giới (Human boundary) ở bước giảng viên kiểm duyệt và quyết định |

## Bài học của Hải

- Ý tưởng hay (như Camera AI phát hiện gian lận) chưa chắc đã là bài toán tốt nhất để thực thi. Một problem tốt phải xét đến tính khả thi về dữ liệu (Data access) và thời gian thực hiện (Làm được trong lab). Bài toán Ngân hàng đề thi đáp ứng tốt điều này.
- Không phải lúc nào cũng cần đến agent. Đôi khi áp dụng AI ở mức Workflow (Rule kết hợp GenAI) như nhóm đã chọn đã mang lại impact rất lớn.

Nếu làm lại:

```text
Trong phần Scan cá nhân, tôi sẽ ưu tiên tìm kiếm các vấn đề liên quan đến quy trình xử lý văn bản/thông tin (Text/Data Workflow) thay vì các hệ thống phần cứng (Camera/CV) để tăng tính ứng dụng và khả năng được nhóm chọn làm bài tập chung.
```