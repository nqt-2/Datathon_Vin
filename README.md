# DATATHON 2026: THE GRIDBREAKER - TEAM [DATATHỐN]

## 1. Giới thiệu dự án
[cite_start]Dự án này được thực hiện trong khuôn khổ vòng 1 cuộc thi **Datathon 2026: The Gridbreaker**[cite: 339, 443]. [cite_start]Mục tiêu chính là phân tích bộ dữ liệu mô phỏng hoạt động kinh doanh của một doanh nghiệp thương mại điện tử thời trang tại Việt Nam trong giai đoạn 2012-2022 để tìm ra các insight giá trị và xây dựng mô hình dự báo doanh thu cho giai đoạn 2023-2024[cite: 19, 222, 444].

## 2. Thành viên nhóm và Phân công nhiệm vụ
[cite_start]Để đảm bảo tính minh bạch và ghi nhận đóng góp, nhóm phân chia vai trò cụ thể như sau[cite: 413, 437, 445]:

| Thành viên | Vai trò | Nhiệm vụ chính |
| :--- | :--- | :--- |
| **Nguyễn Quốc Thái** | Trưởng nhóm | [cite_start]Thiết lập GitHub, Tiền xử lý dữ liệu (Cleaning), Xây dựng & Tối ưu Mô hình dự báo (Phần 3)[cite: 222, 345, 447]. |
| **Nguyễn Đình Sơn** | Coding Specialist | [cite_start]Giải quyết 10 câu hỏi trắc nghiệm (Phần 1), Phân tích EDA & Trực quan hóa dữ liệu (Phần 2)[cite: 139, 202, 448]. |
| **Nguyễn Duy Khang** | Business Analyst | [cite_start]Phân tích Insight kinh doanh (Prescriptive Analysis), Viết báo cáo PDF theo chuẩn NeurIPS[cite: 216, 318, 449]. |

## 3. Cấu trúc Repository
[cite_start]Repository được tổ chức khoa học để Ban giám khảo dễ dàng theo dõi và tái lập kết quả[cite: 326, 346, 451]:

* [cite_start]`**/data**`: Chứa 15 file dữ liệu CSV gốc tải từ Kaggle (products, orders, customers,...)[cite: 27, 343, 386].
* [cite_start]`**/notebooks**`: Chứa các file Jupyter Notebook (.ipynb) ghi lại toàn bộ quá trình xử lý, phân tích và huấn luyện mô hình[cite: 346, 387, 452].
* [cite_start]`**submission.csv**`: File kết quả dự báo doanh thu cuối cùng được định dạng theo yêu cầu để nộp lên Kaggle[cite: 243, 316, 388].
* [cite_start]`**Report.pdf**`: Báo cáo chi tiết (tối đa 4 trang) tóm tắt các phát hiện chính và phương pháp tiếp cận kỹ thuật[cite: 319, 366, 454].

## 4. Pipeline thực hiện
[cite_start]Quy trình làm việc của nhóm tuân thủ các giai đoạn chuẩn trong Khoa học dữ liệu[cite: 350, 455]:

1.  [cite_start]**Làm sạch dữ liệu:** Xử lý giá trị thiếu (null), chuẩn hóa kiểu dữ liệu và định dạng ngày tháng cho 15 bảng dữ liệu[cite: 351, 455].
2.  [cite_start]**Phân tích EDA:** Khám phá dữ liệu qua 4 cấp độ (Mô tả, Chẩn đoán, Dự đoán và Đề xuất) để đưa ra các kiến nghị kinh doanh thiết thực[cite: 216, 355, 456].
3.  [cite_start]**Xây dựng Mô hình:** Thực hiện Feature Engineering (tạo biến lag, mùa vụ) và áp dụng Cross-validation theo chuỗi thời gian để dự báo cột Revenue[cite: 227, 361, 362, 457].
4.  [cite_start]**Giải thích mô hình:** Sử dụng Feature Importance hoặc SHAP để xác định các yếu tố ảnh hưởng lớn nhất đến doanh thu[cite: 256, 364, 458].

## 5. Hướng dẫn cài đặt và Chạy code
### Yêu cầu hệ thống
* Python 3.8+
* [cite_start]Thư viện: `pandas`, `matplotlib`, `seaborn`, `scikit-learn`, `xgboost`[cite: 349, 459].

### Cách chạy
1. Clone repository về máy cá nhân.
2. Cài đặt các thư viện cần thiết: `pip install -r requirements.txt`.
3. [cite_start]Mở các file trong thư mục `/notebooks` bằng VS Code hoặc Jupyter Notebook và chạy theo thứ tự[cite: 346, 389, 459].

---
[cite_start]*Lưu ý: Repository này được để ở chế độ **Public** để phục vụ công tác chấm thi của Ban tổ chức Datathon 2026[cite: 325, 384, 414].*