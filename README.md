<a id="top"></a>

<!-- Banner -->
<p align="center">
  <a href="https://www.uit.edu.vn/" title="Trường Đại học Công nghệ Thông tin" style="border: none;">
    <img src="https://i.imgur.com/WmMnSRt.png" alt="Trường Đại học Công nghệ Thông tin | University of Information Technology">
  </a>
</p>

<h1 align="center"><b>DATA SCIENCE SALARY PREDICTION<br></b></h>

## [BẢNG MỤC LỤC](#top)
* [Giới thiệu môn học](#giới-thiệu-môn-học)
* [Thông tin các thành viên](#thông-tin-về-các-thành-viên-nhóm)
* [Giới thiệu dự án](#giới-thiệu-dự-án)
* [Mô tả bộ dữ liệu](#mô-tả-bộ-dữ-liệu)
* [Phương pháp phân tích](#phương-pháp-phân-tích)
* [Kết quả phân tích](#kết-quả-phân-tích)
* [Kết quả mô hình](#kết-quả-mô-hình)

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
Dưới đây là tóm tắt thông tin về các thuộc tính trong bảng dữ liệu công việc:

| Tên thuộc tính      | Kiểu dữ liệu   | Mô tả                                                                        | Khoảng giá trị                           |
|---------------------|----------------|------------------------------------------------------------------------------|------------------------------------------|
| Job Title           | object (string)| Tên công việc                                                                | “Data Scientist”, “Healthcare Data Scientist”, ... |
| Salary Estimate     | object (string)| Khoảng lương, đi kèm là ghi chú về cách tính lương hoặc thông tin này do ai cung cấp | “$53K-$91K (Glassdoor est.)”, “$21-$34 Per Hour (Glassdoor est.)”, ... |
| Job Description     | object (string)| Mô tả công việc, có chứa các kỹ năng yêu cầu (chuỗi rất dài)                 | “KnowBe4, Inc. is a high growth information sec...”, ... |
| Rating              | float64        | Điểm số đánh giá về công ty                                                  | [-1.0, 5.0]                              |
| Company Name        | object (string)| Tên công ty, kèm với điểm đánh giá                                           | “KnowBe4\n4.8”, “PNNL\n3.8”, ...          |
| Location            | object (string)| Địa điểm làm việc                                                            | “Linthicum, MD”, “Clearwater, FL”, ...    |
| Headquarters        | object (string)| Địa điểm trụ sở chính                                                        | “Baltimore, MD”, “Clearwater, FL”, ...    |
| Size                | object (string)| Quy mô công ty                                                               | “1 to 50 employees”, “51 to 200 employees”, ... |
| Founded             | int64          | Năm thành lập                                                                | [-1, 2019]                               |
| Type of ownership   | object (string)| Loại hình sở hữu công ty                                                     | “Company - Private”, “Government”, ...    |
| Industry            | object (string)| Ngành công nghiệp                                                            | “Energy”, “Security Services”, ...        |
| Sector              | object (string)| Lĩnh vực                                                                     | “Health Care”, “Business Services”, ...   |
| Revenue             | object (string)| Doanh thu công ty                                                            | “$2 to $5 billion (USD)”, “$50 to $100 million (USD)”, ... |
| Competitors         | object (string)| Tên các công ty đối thủ                                                      | -1 hoặc “Novartis, Baxter, Pfizer”, “Travelers, Allstate, State Farm”, ... |


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

### Thăm dò bằng PowerBI
![image](https://github.com/user-attachments/assets/7bfd8126-53d5-48f4-91d5-30a63730a578)

### Thông tin về công việc
<img width="400" alt="overall_distribution" src=https://github.com/user-attachments/assets/8a722aa4-91d8-48f8-830a-46a796d4cb1b>

### Kỹ năng cần thiết
<img width="500" alt="overall_distribution" src=https://github.com/user-attachments/assets/819f6551-c923-4ca4-9a60-ca3663773995>
<img width="400" alt="overall_distribution" src=https://github.com/user-attachments/assets/5d6d06bd-3f44-4d63-ac3a-1c2b513a90bf>

### Thông tin về công ty
<img width="500" alt="overall_distribution" src=https://github.com/user-attachments/assets/5bac85bd-63c4-4982-821d-1fbb63accfec>

### Thông tin về mức lương trên thị trường

- Ảnh hưởng của kinh nghiệm làm việc
<img width="500" alt="overall_distribution" src=https://github.com/user-attachments/assets/80b83ebe-5d0e-4ff0-a104-92200c6c3eca>

- Ảnh hưởng của vị trí địa lý
<img width="500" alt="overall_distribution" src=https://github.com/user-attachments/assets/a3d841ad-9ecc-45ce-b7b5-7fa1fee4dac2>

![image](https://github.com/user-attachments/assets/78b68e93-0da0-416f-91c8-034a1e11cc00)

➡️**Insight:**
- **Thông tin về công việc:** Thị trường việc làm khoa học dữ liệu đa dạng, chủ yếu tuyển dụng nhân lực có kinh nghiệm với các vị trí Senior/Principal chiếm đa số.

- **Kỹ năng cần thiết:** Python và SQL là hai kỹ năng quan trọng nhất. AWS và Spark được yêu cầu nhiều hơn cho các vị trí kỹ thuật.

- **Thông tin về công ty:** Trang tuyển dụng tiếp cận hơn 400 công ty, chủ yếu là công ty tư nhân với quy mô từ trung bình đến lớn. Các công ty này có mức uy tín và chất lượng cao.

- **Thông tin về địa điểm và khu vực:** Công việc tập trung tại các bang như California, Massachusetts, và New York. Các thành phố lớn mang lại nhiều cơ hội nhưng cũng đi kèm thách thức về chi phí sinh hoạt cao.

- **Mức lương trên thị trường:** Mức lương trung bình dao động từ $74,700 đến $128,200, với Data Scientist có mức lương cao nhất. Kinh nghiệm làm việc ảnh hưởng đáng kể đến mức lương, với Entry-level nhận lương thấp hơn so với Senior hoặc Manager/Director.
## [KẾT QUẢ MÔ HÌNH](#top)


| **STT** | **Mô hình**                    | **MSE**        | **MAE**        | **R2**         |
|---------|--------------------------------|----------------|----------------|----------------|
| 0       | XGBoost                        | 2.687e+08      | 1.065e+04      | 8.286e-01      |
| 1       | RandomForest                   | 2.936e+08      | 1.127e+04      | 8.127e-01      |
| 2       | HistogramGradientBoosting      | 4.009e+08      | 1.456e+04      | 7.443e-01      |
| 3       | DecisionTree                   | 4.605e+08      | 1.024e+04      | 7.062e-01      |
| 4       | KNeighbors                     | 8.300e+08      | 2.173e+04      | 4.706e-01      |
| 5       | SVR                            | 1.616e+09      | 3.117e+04      | -3.078e-02     |
| 6       | LinearRegression               | 2.511e+33      | 1.946e+16      | -1.602e+24     |

![image](https://github.com/user-attachments/assets/556a15f7-6d36-4d84-bf5e-8422a76d602c)
