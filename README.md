# DATATHON 2026: THE GRIDBREAKER - TEAM DATATHỐN

## 1. Giới thiệu dự án
Dự án này được thực hiện trong khuôn khổ vòng 1 cuộc thi **Datathon 2026: The Gridbreaker**. Mục tiêu chính là phân tích bộ dữ liệu mô phỏng hoạt động kinh doanh của một doanh nghiệp thương mại điện tử thời trang tại Việt Nam trong giai đoạn 2012-2022 để tìm ra các insight giá trị và xây dựng mô hình dự báo doanh thu cho giai đoạn 2023-2024.

## 2. Thành viên nhóm và Phân công nhiệm vụ
Để đảm bảo tính minh bạch và ghi nhận đóng góp, nhóm phân chia vai trò cụ thể như sau:

| Thành viên | Vai trò | Nhiệm vụ chính |
| :--- | :--- | :--- |
| **Nguyễn Quốc Thái** | Trưởng nhóm | Thiết lập GitHub, Tiền xử lý dữ liệu (Cleaning), Xây dựng & Tối ưu Mô hình dự báo (Phần 3). |
| **Nguyễn Đình Sơn** | Coding Specialist | Giải quyết 10 câu hỏi trắc nghiệm (Phần 1), Phân tích EDA & Trực quan hóa dữ liệu (Phần 2). |
| **Nguyễn Phúc Duy Khang** | Business Analyst | Phân tích Insight kinh doanh (Prescriptive Analysis), Viết báo cáo PDF theo chuẩn NeurIPS. |

## 3. Cấu trúc Repository
Repository được tổ chức khoa học để Ban giám khảo dễ dàng theo dõi và tái lập kết quả:

* `**/data**`: Chứa 15 file dữ liệu CSV gốc tải từ Kaggle (products, orders, customers,...).
* `**/notebooks**`: Chứa các file Jupyter Notebook (.ipynb) ghi lại toàn bộ quá trình xử lý, phân tích và huấn luyện mô hình.
* `**submission.csv**`: File kết quả dự báo doanh thu cuối cùng được định dạng theo yêu cầu để nộp lên Kaggle.
* `**Report.pdf**`: Báo cáo chi tiết (tối đa 4 trang) tóm tắt các phát hiện chính và phương pháp tiếp cận kỹ thuật.

## 4. Pipeline thực hiện
Quy trình làm việc của nhóm tuân thủ các giai đoạn chuẩn trong Khoa học dữ liệu:

1.  **Làm sạch dữ liệu:** Xử lý giá trị thiếu (null), chuẩn hóa kiểu dữ liệu và định dạng ngày tháng cho 15 bảng dữ liệu.
2.  **Phân tích EDA:** Khám phá dữ liệu qua 4 cấp độ (Mô tả, Chẩn đoán, Dự đoán và Đề xuất) để đưa ra các kiến nghị kinh doanh thiết thực.
3.  **Xây dựng Mô hình:** Thực hiện Feature Engineering (tạo biến lag, mùa vụ) và áp dụng Cross-validation theo chuỗi thời gian để dự báo cột Revenue.
4.  **Giải thích mô hình:** Sử dụng Feature Importance hoặc SHAP để xác định các yếu tố ảnh hưởng lớn nhất đến doanh thu.

## 5. Hướng dẫn cài đặt và Chạy code
### Yêu cầu hệ thống
* Python 3.8+
* Thư viện: `pandas`, `matplotlib`, `seaborn`, `scikit-learn`, `xgboost`.

### Cách chạy
1. Clone repository này về máy cá nhân bằng lệnh:  
   `git clone [Link-Repo-Của-Bạn]`
2. Cài đặt các thư viện cần thiết:  
   `pip install pandas matplotlib seaborn scikit-learn xgboost`
3. Mở các file trong thư mục `/notebooks` bằng VS Code hoặc Jupyter Notebook và chạy các cell theo thứ tự từ trên xuống dưới.

---
*Lưu ý: Repository này được để ở chế độ **Public** để phục vụ công tác chấm thi của Ban tổ chức Datathon 2026.*