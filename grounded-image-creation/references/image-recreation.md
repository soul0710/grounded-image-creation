# Tạo lại ảnh tham chiếu

## Mặc định cần giữ

“Tạo lại ảnh này” nghĩa là tái tạo trung thành ảnh gốc trong giới hạn công cụ. Nếu người dùng không yêu cầu thay đổi, giữ:

- bố cục, góc nhìn, tỉ lệ khung, vị trí và số lượng các chủ thể chính;
- hướng và cường độ tương đối của các nguồn sáng, phân bố bóng và phản chiếu;
- bảng màu và tone: cân bằng trắng, sắc nóng/lạnh, hue chủ đạo, độ bão hòa, độ sáng, tương phản, chiều sâu vùng tối và vùng sáng;
- chất liệu, bề mặt, mức độ chi tiết, cảm giác ảnh chụp/tranh/đồ họa.

Xem ảnh bằng `view_image` trước khi tạo. Dùng chính tệp ảnh làm đầu vào edit/reference cho công cụ ảnh khi có thể. Không chỉ chép lại ảnh bằng mô tả chữ. Trong prompt, nói rõ **preserve the original color palette, white balance, tonal range, saturation, contrast, exposure, and lighting ratios**; tránh tính từ như “rực rỡ hơn”, “điện ảnh hơn”, “ánh vàng ấm hơn”, “sắc nét hơn” khi người dùng không yêu cầu. Nếu yêu cầu đổi một phần (ví dụ đổi vật trên bàn), lặp lại các thuộc tính còn phải giữ trong mỗi lần sửa.

Áp dụng `visual-aesthetics` để nhận diện điểm nhấn, mảng sáng tối, quan hệ màu, đường dẫn mắt và chất liệu *đã hiện diện* trong ảnh. Kiến thức bổ sung hoặc nghiên cứu web giúp nhận ra vật thể/bối cảnh và tránh lỗi thực tế; không được dùng để âm thầm đổi phong cách, cảnh trí hay màu của ảnh tham chiếu. Nếu người dùng chỉ nói “tạo lại”, mặc định tái tạo cả chi tiết có vẻ phi thực tế như trong ảnh gốc; không tự hiệu chỉnh. Chỉ hỏi khi họ đồng thời yêu cầu ảnh đúng thực tế và hai mục tiêu xung đột đáng kể.

## So ảnh trước khi chấp nhận

Mở cả ảnh gốc và ảnh ứng viên ở kích thước dễ so. So toàn ảnh rồi so ít nhất các vùng chủ thể, nền và nguồn sáng. Trả lời rõ:

1. Ảnh mới có giữ cùng ấn tượng màu tổng thể, tỷ lệ nóng/lạnh và độ sáng không?
2. Các vùng sáng nhất, tối nhất, màu nổi bật nhất có nằm và mạnh tương đối như ảnh gốc không?
3. Có vùng nào bị cam/vàng/xanh hơn, bão hòa hơn, tương phản mạnh hơn hoặc sáng hơn đáng kể mà người dùng không yêu cầu không?
4. Bố cục, vật thể, tỉ lệ, văn bản và ánh sáng có dịch chuyển hoặc thay đổi đáng kể không?

Agent review phải **xem cả hai tệp**, trả lời riêng mục màu/tone: `giữ đạt` hoặc `lệch cần sửa`, nêu vùng và hướng lệch. Không cho qua lệch màu/tone đáng kể chỉ vì ảnh “đẹp hơn”. Nếu công cụ không đạt sau các lần sửa hợp lý, báo rõ giới hạn và không mô tả ảnh là bản tạo lại trung thành.
