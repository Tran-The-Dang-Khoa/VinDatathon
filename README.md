#VinDatathon 2026 - THE GRIDBREAKER 
### Team: CUTIE KT 
**Thành viên:** Trần Thế Đăng Khoa & Hoàng Bảo Trân 

Dự án tập trung giải quyết bài toán tối ưu hóa vận hành và dự báo doanh thu dựa trên bộ dữ liệu thương mại điện tử gồm 13 bảng liên kết.

---

## 🏗️ Cấu trúc Repository

### 1. Khám phá & Giải đố
* **`EDA_narrative.ipynb`**: Thực hiện phân tích đa tầng để tìm ra các "nút thắt" kinh doanh. 
    * Xác định lỗi `wrong_size` chiếm ~50% đơn hoàn trong nhóm Outdoor & Streetwear.
    * Phân tích áp lực nhu cầu vùng miền, phát hiện sự lệch pha cung cầu tại vùng East.
* **`MCQ.ipynb`**: Chứa lời giải chi tiết cho các câu hỏi trắc nghiệm dựa trên dữ liệu thực tế của cuộc thi.

### 2. Xử lý Dữ liệu (Preprocessing)
* **`reEDA`**: Quy trình làm sạch và chuẩn bị dữ liệu.
    * Loại bỏ các chỉ số ảo như `avg_rating`, thay thế bằng `defect_rate` để phản ánh đúng chất lượng.
    * Tạo các đặc trưng (Feature Engineering) cần thiết cho mô hình dự báo.
    * **Output:** `out.csv` – Bộ dữ liệu sạch, sẵn sàng cho training.

### 3. Dự báo Doanh thu (Modeling)
* **`revenue_forecast`**: Xây dựng và triển khai mô hình dự báo. 
    * Sử dụng các phát hiện từ EDA (như lịch áp lực nhu cầu) để tinh chỉnh mô hình.
    * **Output:** `sales_test.csv` – Kết quả dự báo doanh thu cuối cùng.

---

## 💡 Đề xuất Hành động nổi bật
* **Số hóa Size Guide:** Dự kiến giảm 30% đơn hoàn do sai size, tiết kiệm ~232.5 triệu VND/năm.
* **Điều phối Tồn kho:** Tăng buffer stock cho vùng East vào tháng 4 và tháng 12 để giải quyết triệt để tình trạng fill_rate âm.
* **Tối ưu Freeship:** Nâng ngưỡng từ 300k lên 500k để cải thiện ROI nhanh chóng.
