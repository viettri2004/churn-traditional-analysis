# Dự án: Dự đoán Khả năng Rời bỏ của Khách hàng Viễn thông (Customer Churn Prediction)

## Mô tả
Đây là mã nguồn (source code) phục vụ cho báo cáo môn Khai phá Dữ liệu, áp dụng quy trình CRISP-DM để dự đoán khả năng khách hàng ngừng sử dụng dịch vụ dựa trên bộ dữ liệu Telco Customer Churn. Dự án huấn luyện và so sánh 5 mô hình học máy: Decision Tree, KNN, Naive Bayes, Random Forest, và Gradient Boosting.

## Cấu trúc thư mục (Folder Structure)
Mã nguồn được tổ chức theo tiêu chuẩn Data Science chuyên nghiệp:

```text
churn-traditional-analysis/
│
├── data/                                 # Chứa tập dữ liệu
│   └── WA_Fn-UseC_-Telco-Customer-Churn.csv
│
├── notebooks/                            # Chứa toàn bộ mã nguồn (.ipynb)
│   ├── 01_EDA_and_Preprocessing.ipynb    # Code EDA và Tiền xử lý (Data Understanding & Preparation)
│   ├── 02_Model_DecisionTree.ipynb       # Huấn luyện mô hình Decision Tree
│   ├── 02_Model_KNN.ipynb                # Huấn luyện mô hình K-Nearest Neighbors
│   ├── 02_Model_NaiveBayes.ipynb         # Huấn luyện mô hình Naive Bayes
│   ├── 03_Model_Evaluation.ipynb         # Đánh giá và so sánh toàn bộ 5 mô hình (Evaluation)
│   └── 04_Decision_Making.ipynb          # Phân tích Feature Importance và Đề xuất kinh doanh (Decision Making)
│
├── images/                               # Chứa các biểu đồ kết quả (.png)
│   ├── confusion_matrix_Comparison.png
│   ├── roc_curve_comparison.png
│   └── ...
│
├── README.md                             # Tài liệu giới thiệu dự án
└── requirements.txt                      # Các thư viện cần thiết
```

## Yêu cầu môi trường
Các thư viện cần thiết để chạy dự án được liệt kê trong tệp `requirements.txt`:
- Python 3.8+
- pandas
- numpy
- scikit-learn
- matplotlib
- seaborn
- jupyter

## Hướng dẫn cài đặt và chạy mã nguồn

**1. Tạo môi trường ảo (Khuyến nghị)**
```bash
python -m venv .venv
# Kích hoạt trên Windows:
.venv\Scripts\activate
# Kích hoạt trên MacOS/Linux:
source .venv/bin/activate
```

**2. Cài đặt các thư viện cần thiết**
```bash
pip install -r requirements.txt
```

**3. Khởi chạy Jupyter Notebook**
```bash
jupyter notebook
```
Sau đó, bạn có thể điều hướng vào thư mục `notebooks/` và mở chạy thử các file theo đúng **thứ tự từ 01 đến 04** để tái tạo toàn bộ kết quả phân tích.
