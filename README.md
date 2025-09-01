# Phân loại hoa Diên vĩ (Iris) với Machine Learning

## Giới thiệu

Dự án này nhằm mục đích xây dựng một mô hình Machine Learning để phân loại ba loài hoa diên vĩ khác nhau dựa trên các đặc trưng vật lý của chúng. Bộ dữ liệu Iris là một trong những bộ dữ liệu kinh điển và được sử dụng rộng rãi trong lĩnh vực Machine Learning để học tập và thực hành.

**Ba loài hoa diên vĩ cần phân loại:**
- **Setosa** (Iris setosa)
- **Versicolor** (Iris versicolor) 
- **Virginica** (Iris virginica)

**Các đặc trưng được sử dụng:**
- Chiều dài đài hoa (sepal length)
- Chiều rộng đài hoa (sepal width)
- Chiều dài cánh hoa (petal length)
- Chiều rộng cánh hoa (petal width)

## Cấu trúc dự án

```
Iris-flower-classification/
├── iris.csv                    # Bộ dữ liệu Iris (150 mẫu)
├── iris_classification.ipynb   # Jupyter Notebook chính
└── README.md                   # Tài liệu hướng dẫn (file này)
```

## Yêu cầu hệ thống

- **Python**: 3.9+ (khuyến nghị Python 3.9 trở lên)
- **Hệ điều hành**: Windows, macOS, hoặc Linux
- **RAM**: Tối thiểu 4GB
- **Dung lượng**: ~100MB cho môi trường và thư viện

## Cài đặt môi trường

### Bước 1: Tạo môi trường ảo
```bash
python -m venv .venv
```

### Bước 2: Kích hoạt môi trường ảo
**Trên Linux/macOS:**
```bash
source .venv/bin/activate
```

**Trên Windows:**
```cmd
.venv\Scripts\activate
```

### Bước 3: Cập nhật pip
```bash
pip install --upgrade pip
```

### Bước 4: Cài đặt các thư viện cần thiết
```bash
pip install jupyter scikit-learn pandas numpy matplotlib seaborn
```

## Cách chạy Notebook

### Bước 1: Khởi động Jupyter Notebook
```bash
jupyter notebook
```

### Bước 2: Mở file notebook
- Trình duyệt sẽ tự động mở tại `http://localhost:8888`
- Click vào file `iris_classification.ipynb`
- Chạy lần lượt các cell từ trên xuống dưới bằng cách nhấn `Shift + Enter`

## Nội dung Notebook

Notebook được chia thành các phần chính sau:

1. **Giới thiệu**: Mô tả mục tiêu và nội dung của notebook
2. **Import thư viện**: Tải các thư viện cần thiết (pandas, numpy, matplotlib, seaborn, scikit-learn)
3. **Tải dữ liệu**: Đọc và khám phá dữ liệu từ file `iris.csv`
4. **Khám phá dữ liệu (EDA)**: Phân tích và trực quan hóa dữ liệu
5. **Tiền xử lý dữ liệu**: Chuẩn bị dữ liệu cho việc huấn luyện
6. **Huấn luyện mô hình**: Thử nghiệm nhiều thuật toán khác nhau
7. **Tối ưu siêu tham số**: Tìm kiếm tham số tốt nhất cho mô hình
8. **Đánh giá mô hình**: Đánh giá chi tiết hiệu suất trên tập test
9. **Lưu mô hình**: Lưu mô hình tốt nhất và thực hiện suy luận
10. **Kết luận**: Tổng kết và hướng phát triển

## Kết quả mong đợi

- **Độ chính xác**: Thường đạt từ 0.9 đến 1.0 (90-100%)
- **Mô hình hiệu quả**: Support Vector Machine (SVC) và Random Forest thường cho kết quả tốt nhất
- **Thời gian huấn luyện**: Rất nhanh (< 1 giây) do kích thước dữ liệu nhỏ

## Nguồn dữ liệu và tham khảo

- **UCI Machine Learning Repository**: [Iris Data Set](https://archive.ics.uci.edu/ml/datasets/iris)
- **Scikit-learn**: [sklearn.datasets.load_iris](https://scikit-learn.org/stable/modules/generated/sklearn.datasets.load_iris.html)
- **Tác giả gốc**: Ronald Fisher (1936)

## Gợi ý mở rộng

1. **Thử nghiệm thêm mô hình**: Neural Networks, Gradient Boosting, XGBoost
2. **Tối ưu siêu tham số**: Sử dụng RandomizedSearchCV, Optuna
3. **Kỹ thuật tiền xử lý**: Feature scaling, PCA, feature selection
4. **Cross-validation**: K-fold, stratified K-fold
5. **Ensemble methods**: Voting classifier, stacking
6. **Triển khai mô hình**: Tạo API với Flask/FastAPI, containerize với Docker
7. **Theo dõi mô hình**: MLflow, Weights & Biases

## Giấy phép

Đây là một dự án ví dụ cho mục đích học tập. Bộ dữ liệu Iris là công khai và được sử dụng tự do cho nghiên cứu và giáo dục.

---

*Chúc bạn học tập hiệu quả với Machine Learning! 🌸*