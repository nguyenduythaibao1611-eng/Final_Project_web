# 🥗 PROJECT: VIECAL - VIETNAMESE NUTRITION TRACKER

## 1. Objective — Mục tiêu dự án
* **Số hóa dữ liệu:** Trích xuất và xây dựng cơ sở dữ liệu cho 100+ thực phẩm phổ biến từ sách "Bảng thành phần thực phẩm Việt Nam".
* **Tính toán chính xác:** Đo lường Kcal, Protein, Lipid, Glucid dựa trên định lượng thực tế của người Việt.
* **Cá nhân hóa:** Tự động tính toán nhu cầu năng lượng (TDEE) theo chỉ số cơ thể riêng biệt.
* **Minh bạch:** Mỗi thông tin thực phẩm đều đính kèm số trang tham chiếu từ nguồn sách gốc của Viện Dinh Dưỡng.

## 2. Target Users — Đối tượng người dùng
* **Weight Control:** Người theo dõi thâm hụt hoặc dư thừa Calo để tăng/giảm cân.
* **Gymers:** Tập trung vào chỉ số Protein và Lipid để tối ưu cơ bắp.
* **Nutrition Students:** Tra cứu số liệu y khoa chuẩn xác cho học tập và nghiên cứu.
* **Chronic Patients:** Kiểm soát lượng Đường/Béo nạp vào cơ thể hàng ngày.

## 3. Feature List (MoSCoW)
* **Must have:**
    - Tra cứu thực phẩm theo tên (Search).
    - Hiển thị chi tiết dinh dưỡng P-L-G (Details).
    - Tính toán năng lượng theo khẩu phần gram (Portion Calc).
    - Nhật ký ăn uống hàng ngày (Diary).
* **Should have:**
    - Thiết lập mục tiêu Calo cá nhân (Goal Setting).
    - Xem lại lịch sử ăn uống (History).
    - Đăng nhập tài khoản lưu trữ dữ liệu (Login).
* **Nice to have:**
    - Công cụ tính BMR/TDEE tự động.
    - Danh sách món ăn yêu thích (Favorites).
    - So sánh thành phần giữa 2 loại thực phẩm (Compare).

## 4. UI Design — Thiết kế giao diện
* **Mockup:** Dashboard trung tâm với vòng tròn Progress Bar (Glassmorphism), thanh tìm kiếm nhanh và các thẻ (Card) bữa ăn sáng/trưa/tối.
* **Color & Typography:** Mint Green (#E8F5E9) & White; Font: "Be Vietnam Pro".
* **User Flow:** Login -> Input Stats -> Search Food -> Add to Diary -> Track Progress.

## 5. ERD — Sơ đồ thực thể (5 Entities)
* **FOOD_GROUP:** Phân loại nhóm thực phẩm (1:N FOOD).
* **FOOD:** Dữ liệu thực phẩm từ sách (Name, Kcal, P, L, G, Reference_Page).
* **USER:** Thông tin cá nhân và chỉ số TDEE.
* **DIARY:** Nhật ký tổng hợp theo ngày của User (1:N DIARY_ENTRY).
* **DIARY_ENTRY:** Chi tiết món ăn và khối lượng trong một nhật ký.