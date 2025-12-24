📘 LESSON 1 (OFFICIAL)
Business → Data (Từ nghiệp vụ đến dữ liệu)

Domain: E-commerce

1️⃣ Mục tiêu của Lesson 1

Sau bài này, bạn sẽ:

Hiểu Business requirement là gì (đúng nghĩa, không mơ hồ)

Biết cách tìm Entity từ mô tả nghiệp vụ

Phân biệt rõ:

Entity

Attribute

Relationship
→ Đây là nền móng, nếu sai ở đây thì các bài sau sẽ rất khó.

2️⃣ Thuật ngữ cốt lõi (giải thích kỹ)
🔹 Business Requirement

Tiếng Anh: Business Requirement
Nghĩa: Yêu cầu nghiệp vụ
Là gì?
→ Những gì business muốn hệ thống làm được

Ví dụ E-commerce:

Khách hàng mua hàng

Khách hàng thanh toán

Theo dõi trạng thái đơn hàng

👉 Lưu ý quan trọng:
❌ Business requirement KHÔNG phải là bảng database
❌ Business requirement KHÔNG phải là API

🔹 Entity

Tiếng Anh: Entity
Nghĩa: Thực thể (đối tượng dữ liệu)

Entity là gì?
→ Một đối tượng:

Có ý nghĩa trong business

Cần lưu dữ liệu lâu dài

Có nhiều thuộc tính

Dấu hiệu nhận biết Entity (rất quan trọng):

Thường là danh từ

Có vòng đời riêng (lifecycle)

Không phụ thuộc hoàn toàn vào đối tượng khác

Ví dụ Entity trong E-commerce:

Customer (khách hàng)

Order (đơn hàng)

Product (sản phẩm)

Payment (thanh toán)

❌ Không phải Entity:

“Mua hàng”

“Thanh toán thành công”

“Xem sản phẩm”

👉 Vì đây là hành động, không phải đối tượng lưu trữ lâu dài.

🔹 Attribute

Tiếng Anh: Attribute
Nghĩa: Thuộc tính

Attribute là gì?
→ Thông tin mô tả cho Entity

Ví dụ:

Customer:

name (tên)

email

phone

Product:

name

price

status

👉 Attribute luôn thuộc về Entity, không tồn tại độc lập.

🔹 Relationship

Tiếng Anh: Relationship
Nghĩa: Mối quan hệ

Relationship là gì?
→ Cách các Entity liên kết với nhau trong nghiệp vụ

Đặc điểm:

Thường là động từ

Mô tả luồng business

Ví dụ:

Customer places Order
(Khách hàng đặt đơn hàng)

Order contains Product
(Đơn hàng chứa sản phẩm)

Order is paid by Payment
(Đơn hàng được thanh toán bằng payment)

3️⃣ Ví dụ E-commerce (từng bước, rất chậm)
Mô tả nghiệp vụ:

“Một khách hàng có thể đặt nhiều đơn hàng.
Mỗi đơn hàng gồm nhiều sản phẩm.
Mỗi đơn hàng có thể được thanh toán.”

🔹 Bước 1: Tìm danh từ (Candidate Entities)

khách hàng → Customer

đơn hàng → Order

sản phẩm → Product

thanh toán → Payment

👉 Tạm thời có 4 candidate entity

🔹 Bước 2: Tìm động từ (Relationships)

khách hàng đặt đơn hàng

đơn hàng gồm sản phẩm

đơn hàng được thanh toán bằng payment

🔹 Bước 3: Hỏi câu hỏi “senior”

Trước khi chốt entity, hỏi:

Đối tượng này có cần lưu lâu dài không?

Có thay đổi theo thời gian không?

Có cần truy vết lịch sử không?

👉 Nếu có → rất nên là entity

➡️ Với Customer / Order / Product / Payment → đều có
→ Chốt 4 entity chính.

4️⃣ Insight từ Senior (kinh nghiệm thực tế)
❌ Lỗi junior rất hay gặp

Biến mọi thứ thành entity

Hoặc gom hết vào 1–2 bảng lớn

✅ Senior luôn nghĩ:

“Nếu business đổi yêu cầu sau 6 tháng, model này có chịu được không?”

👉 Data modeling không phải chỉ để chạy, mà để chịu được thay đổi.

5️⃣ Câu hỏi thực tế (kèm dịch)
❓ Question 1

English:

Is “Cart” an entity in an e-commerce system?

Tiếng Việt:

“Giỏ hàng (Cart) có phải là entity trong hệ thống e-commerce không?”

👉 Gợi ý suy nghĩ:

Cart có tồn tại lâu dài không?

Có cần lưu lịch sử không?

❓ Interview Question

English:

How do you identify entities when modeling a system?

Tiếng Việt:

“Bạn xác định entity như thế nào khi thiết kế data model cho một hệ thống?”

👉 Câu trả lời tốt:

Nói về business

Không nói về bảng hay database ngay

6️⃣ Mini Test – tự kiểm tra (rất quan trọng)

Bạn hãy tự trả lời bằng lời của bạn:

1️⃣ Entity là gì?
2️⃣ Attribute khác Entity ở điểm nào?
3️⃣ Vì sao “mua hàng” không phải entity?
4️⃣ Payment có phải entity không? Vì sao?

👉 Không cần đúng hết, mục tiêu là hiểu.

7️⃣ Tóm tắt Lesson 1

Data modeling bắt đầu từ business

Entity = danh từ + có vòng đời

Relationship = động từ

Làm đúng Lesson 1 → các lesson sau sẽ dễ hơn rất nhiều

🔜 Lesson tiếp theo
Lesson 2 – ERD & Cardinality

1–1, 1–N, N–N là gì?

Quan hệ nào nguy hiểm trong thực tế

Ví dụ E-commerce chi tiết

👉 Sau Lesson 2 sẽ có Quiz 1.
