# Grounded Image Creation

Bộ hai Codex skills để tạo/chỉnh sửa ảnh bitmap theo ý định người dùng, kiểm chứng chi tiết đời thực khi cần và bắt buộc agent độc lập xem ảnh cuối trước câu trả lời cuối.

- [`grounded-image-creation/`](grounded-image-creation/SKILL.md): quy trình tạo ảnh, nghiên cứu địa danh/kiến trúc, tạo lại ảnh tham chiếu, và review.
- [`visual-aesthetics/`](visual-aesthetics/SKILL.md): kiến thức thực hành về bố cục, ánh sáng, màu, nhiếp ảnh và hội họa có liên kết nguồn.

Khi người dùng chỉ yêu cầu **tạo lại ảnh**, skill mặc định giữ bố cục, ánh sáng, màu sắc và tone của ảnh gốc. Agent review phải mở cả ảnh gốc lẫn ảnh mới, báo riêng nếu màu hoặc tone bị lệch. Nghiên cứu web giúp kiểm tra chi tiết có thật; nó không tự cho phép đổi màu hoặc sửa cảnh của ảnh tham chiếu.

## Cài đặt

Skill có [checklist 8 nhóm lỗi hình ảnh](grounded-image-creation/references/image-quality-checklist.md) cho tạo và sửa ảnh: tính hợp lý, kết cấu/không gian, điểm nhấn, mật độ/lặp, ánh sáng, màu/chất liệu, phối cảnh/chiều sâu, chi tiết/độ trung thành. Khi sửa ảnh, bắt buộc kiểm tra trước sửa và sau mỗi lần sửa, gồm cả vùng cần giữ; agent độc lập kiểm tra đúng bản cuối. Checklist tôn trọng phạm vi yêu cầu và phong cách, không mặc định mọi khác biệt thẩm mỹ là lỗi.

Sao chép **cả hai thư mục** `grounded-image-creation` và `visual-aesthetics` vào thư mục Codex skills của bạn (thường là `~/.codex/skills/`) để chúng nằm cạnh nhau. Skill tạo ảnh dùng skill `imagegen` có sẵn trong Codex và yêu cầu môi trường hỗ trợ agent độc lập để hoàn tất bước review.

Các tài liệu tham chiếu nằm trong `references/` của từng skill. Tài liệu liên kết trực tiếp tới nguồn gốc chuyên môn; không sao chép ảnh nguồn vào repository.
