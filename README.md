learning-toeic

## Mentor TOEIC (Claude Code skill)

Project này dùng Claude Code skill `toeic-mentor` (định nghĩa ở
`.claude/skills/toeic-mentor/SKILL.md`) làm gia sư luyện thi TOEIC cá nhân. Toàn bộ tiến độ
học (lộ trình, thẻ ghi nhớ, error log, kiến thức đã học, lịch sử mock test) được lưu trong
thư mục `toeic-mentor/` và commit cùng repo — nên clone repo về máy nào, mở Claude Code ở đó
và học tiếp là đủ, không cần cấu hình thêm.

Cách dùng:
1. Mở Claude Code trong thư mục project này (`learning-toeic`).
2. Gõ một câu như "hôm nay học gì" hoặc "học toeic" — Claude sẽ tự nhận diện và chạy skill
   `toeic-mentor` (có thể gọi tường minh bằng `/toeic-mentor` nếu muốn chắc chắn).
3. Phiên đầu tiên: skill sẽ cho làm bài test chẩn đoán rồi đề xuất lộ trình 24 tuần — xác nhận
   hoặc chỉnh trước khi học chính thức.
4. Các phiên sau: skill tự đọc `toeic-mentor/PROGRESS.md` để biết hôm nay ôn gì/học gì, không
   cần bạn nhắc lại ngữ cảnh.
5. Sau mỗi phiên, nhớ `git add`/`commit` thư mục `toeic-mentor/` (file tiến độ thay đổi liên
   tục) rồi push, để máy khác clone xuống có đúng trạng thái học mới nhất.
