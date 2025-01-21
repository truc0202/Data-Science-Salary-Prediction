<a id="top"></a>

<!-- Banner -->
<p align="center">
  <a href="https://www.uit.edu.vn/" title="Trường Đại học Công nghệ Thông tin" style="border: none;">
    <img src="https://i.imgur.com/WmMnSRt.png" alt="Trường Đại học Công nghệ Thông tin | University of Information Technology">
  </a>
</p>

<h1 align="center"><b>PHÂN TÍCH DỮ LIỆU<br></b></h>

## [BẢNG MỤC LỤC](#top)
* [GIỚI THIỆU MÔN HỌC]()
* [Thông tin các thành viên](#thông-tin-về-các-thành-viên-nhóm)

## [GIỚI THIỆU MÔN HỌC](#top)
* **Tên môn học:** Phân tích Dữ liệu - Data Analysis
* **Mã môn học:** IE224
* **Mã lớp:** IE224.P11
* **Năm học:** HK1 (2024 - 2025)
* **Giảng viên:** ThS. Phạm Thế Sơn

## [THÔNG TIN VỀ CÁC THÀNH VIÊN NHÓM](#top)

| STT    | MSSV          | Họ và Tên                |Vai trò    | Github                                          | Email                   |
| :----: |:-------------:| :-----------------------:|:---------:|:-----------------------------------------------:|:-------------------------:
| 1      | 22521550      | Nguyễn Công Trúc            |Trưởng nhóm| [truc0202](https://github.com/truc0202)           | 22521550@gm.uit.edu.vn   |
| 2      | 22521280      | Nguyễn Phú Tài          | Thành viên|            | 22521280@gm.uit.edu.vn   |
| 3      | 22521301      | Mai Văn Tân         | Thành viên| [tanmaivan](https://github.com/tanmaivan)             | 22521301@gm.uit.edu.vn   |
| 2      | 22521568      | Trần Lê Nguyên Trung          | Thành viên| [Trần Trung](https://github.com/Fat-ctrl)             | 22521568@gm.uit.edu.vn   |

## [GIỚI THIỆU DỰ ÁN](#top)

- Bối cảnh: Ngành Khoa học Dữ liệu phát triển, ảnh hưởng đến nhiều lĩnh vực.
- Nhu cầu: Hiểu rõ yếu tố ảnh hưởng đến mức lương trong ngành này.
- Mục tiêu: Phân tích và dự đoán mức lương các vị trí trong ngành Khoa học Dữ liệu.
- Dữ liệu: Sử dụng bộ dữ liệu [Data Science Jobs & Salaries 2024](https://www.kaggle.com/datasets/fahadrehman07/data-science-jobs-and-salary-glassdoor/data) trên Kaggle.
- Công cụ và thư viện:
<a href="#"><img alt="Python" src= "https://img.shields.io/badge/PowerBI-FFFF00.svg?logo=powerbi&logoColor=white"></a>
<a href="#"><img alt="Python" src="https://img.shields.io/badge/Python-003F5D.svg?logo=python&logoColor=white"></a>
<a href="#"><img alt="Pandas" src="https://img.shields.io/badge/Pandas-00527C.svg?logo=pandas&logoColor=white"></a>
<a href="#"><img alt="NumPy" src="https://img.shields.io/badge/Numpy-00609C.svg?logo=numpy&logoColor=white"></a>
<a href="#"><img alt="SciPy" src="https://img.shields.io/badge/SciPy-1560bd.svg?logo=scipy&logoColor=white"></a>
<a href="#"><img alt="Matplotlib" src="https://img.shields.io/badge/Matplotlib-006DB2.svg?logo=python-matplotlib&logoColor=white"></a>
<a href="#"><img alt="Selenium" src="https://img.shields.io/badge/Selenium-1faecf.svg?logo=selenium&logoColor=white"></a>
<a href="#"><img alt="seaborn" src="https://img.shields.io/badge/seaborn-4E97D1.svg?logo=pandas&logoColor=white"></a>
<a href="#"><img alt="plotly" src="https://img.shields.io/badge/plotly-7BB4E3.svg?logo=plotly&logoColor=white"></a>
<a href="#"><img alt="sklearn" src="https://img.shields.io/badge/sklearn-A3CEEF.svg?logo=scikitlearn&logoColor=white"></a>
<a href="#"><img alt="NLTK" src="https://img.shields.io/badge/NLTK-C5D4EB.svg?logo=python-nltk&logoColor=white"></a>
- Mô hình hồi quy:
  + Random Forest
  + SVR
  + XGBoost
  + Linear Regression (thư viện scikit-learn)
## [MÔ TẢ BỘ DỮ LIỆU](#top)



## [PHƯƠNG PHÁP PHÂN TÍCH](#top)

![image](https://github.com/user-attachments/assets/24d38ad3-9056-4bcf-92e5-577e5d01c7de)
1️⃣ Định nghĩa vấn đề
Xác định lĩnh vực và chủ đề phân tích. Đặt câu hỏi về đầu ra và kĩ năng học được từ dự án.

2️⃣ Thu thập dữ liệu
Mỗi thành viên tìm kiếm bộ dữ liệu phù hợp, hầu hết chọn trên Kaggle. Thảo luận và chọn dữ liệu phù hợp nhất.

3️⃣ Tiền xử lý dữ liệu

Kiểm tra dữ liệu:
+ Missing values, Duplicates, Data Types, Unique Values, Statistics, Categories.

Làm sạch dữ liệu:
- Loại bỏ cột không cần thiết, xử lý cột Job Title, Salary Estimate, Job Description, Rating, Size, Revenue, Company Name, Competitors, Founded, Type of Ownership.

Lưu dữ liệu đã làm sạch:
- Lưu dưới dạng file CSV

4️⃣ Phân tích thăm dò dữ liệu (EDA)

- **Phân tích đơn biến:** Phân phối lương, đánh giá, tuổi, biến phân loại nhị phân.

- **Phân tích hai biến:** Lương theo chức danh, ngành nghề, công ty, kỹ năng, vị trí.

- **Phân tích sâu hơn:** Lương theo doanh thu, độ tuổi và quy mô công ty, loại hình sở hữu.

- **Trích xuất biến quan trọng:** Ma trận tương quan, phân tích ANOVA.
  
5️⃣ Huấn luyện mô hình

- Đọc và kiểm tra dữ liệu.

- Chia dữ liệu thành tập huấn luyện và kiểm tra.

- Xây dựng đường ống dữ liệu.

- Lựa chọn và tinh chỉnh mô hình.

6️⃣ Đánh giá hiệu suất

- Đánh giá mô hình bằng MSE, MAE, R2.

- Kiểm tra chéo K-Fold.

- Trực quan hóa kết quả.
## [KẾT QUẢ PHÂN TÍCH](#top)

![image](https://github.com/user-attachments/assets/7bfd8126-53d5-48f4-91d5-30a63730a578)

