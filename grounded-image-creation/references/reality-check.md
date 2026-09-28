# Kiểm chứng thực tế và review ảnh cuối

## Chọn mức nghiên cứu

- **Cảnh hư cấu hoặc ảnh trừu tượng:** không cần nghiên cứu địa điểm; xác minh ràng buộc của người dùng và tính nhất quán bên trong ảnh.
- **Loại hình ngoài đời** (ví dụ nhà dân Mỹ, phố cổ, cây trồng bản địa): xác định vùng, thời kỳ, biến thể. Không xem một ảnh ví dụ là đại diện cho mọi nơi/mọi thời.
- **Địa danh/công trình định danh:** xác minh vị trí, dáng tổng thể, mặt nào đang thấy, công trình/cảnh quan kế cận, đường tiếp cận, địa hình, tỉ lệ, và các thay đổi theo thời gian hoặc mùa. Một danh thắng có thể không thể đứng cùng các công trình khác trong một góc nhìn như prompt mô tả.
- **Tái hiện lịch sử:** xác định năm hoặc khoảng thời gian; phân biệt hiện trạng, phục dựng, và chi tiết suy đoán. Dấu hiệu hiện đại không được lọt vào cảnh gắn niên đại nếu người dùng muốn chính xác lịch sử.

## Nguồn tham khảo đáng ưu tiên

1. Website chính thức của di tích, cơ quan quản lý, bảo tàng, cơ quan di sản, bản đồ/ảnh tư liệu có ngày và vị trí rõ. Với Di sản Thế giới, hồ sơ địa điểm của [UNESCO World Heritage Centre](https://whc.unesco.org/en/list/) giúp xác định khu vực và mô tả công trình; cần kiểm tra thêm nguồn địa phương để biết điểm nhìn cụ thể.
2. Với kiến trúc Mỹ, [Library of Congress HABS/HAER/HALS](https://www.loc.gov/pictures/collection/hh/) có ảnh, bản vẽ đo đạc và lịch sử; nếu kho này không truy cập được, tra qua [trang bộ sưu tập của National Park Service](https://www.nps.gov/subjects/heritagedocumentation/collection.htm). [National Park Service](https://www.nps.gov/articles/colonial-revival-architecture.htm) cũng có mô tả kiểu Colonial Revival. Các nguồn này cho thấy “nhà truyền thống Mỹ” gồm nhiều kiểu; ví dụ cụ thể phải gắn với vùng và thời kỳ.
3. Ảnh hiện trường có chú thích nguồn, ngày, góc chụp để so môi trường xung quanh. Kết quả tìm ảnh chung, ảnh stock, ảnh AI và blog không dẫn nguồn chỉ dùng để gợi ý, không để khẳng định một chi tiết khó xác minh.

Ghi ngắn gọn: **điều đã xác minh → nguồn → chi tiết đưa vào prompt → điều còn chưa chắc**. Nếu hai nguồn xung đột, xem ngày, vị trí và giai đoạn lịch sử; không ghép cả hai vào một hình.

## Ví dụ phân giải yêu cầu mơ hồ

“Một ngôi nhà truyền thống Mỹ” chưa đủ để khẳng định một mặt tiền chính xác. Có thể hỏi vùng/niên đại/phong cách. Nếu người dùng muốn làm ngay và không có ràng buộc, chọn một kiểu có tên như Colonial Revival, Craftsman bungalow hoặc ranch, nghiên cứu kiểu đó rồi mô tả mái, hiên, cửa sổ, vật liệu và cảnh quan hợp vùng. Tránh trộn mái, cột, hiên, cửa và chi tiết từ các kiểu/niên đại khác nhau chỉ vì chúng cùng mang cảm giác “Mỹ”.

## Gói giao cho agent review

- Prompt gốc và những yếu tố bắt buộc.
- Đường dẫn ảnh **cuối cùng mà agent mở xem được**; nếu có ảnh tham chiếu, ghi rõ vai trò của từng ảnh.
- Các phát hiện chính kèm URL nguồn; phân biệt điều chắc chắn và giả định.
- Các điểm dễ sai cần soi: không gian xung quanh địa danh, kiểu kiến trúc, niên đại, tỉ lệ, chữ, số lượng vật, ánh sáng/bóng, chi tiết người, viền ảnh sửa.

Yêu cầu agent trả lời: **đã xem ảnh hay chưa; đạt/chưa đạt; lỗi trọng yếu kèm vị trí trong ảnh và nguồn/quan sát; sửa tối thiểu cần làm; giới hạn chưa xác minh**. Reviewer không chỉ xét prompt. Không thay phán đoán bằng một điểm số chung. Nếu lỗi trọng yếu, sửa và gửi lại bản mới cho agent xem.
