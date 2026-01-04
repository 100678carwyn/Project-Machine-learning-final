# DỰ ĐOÁN NGUY CƠ MẮC BỆNH TIM MẠCH DỰA TRÊN CÁC CHỈ SỐ SỨC KHỎE CÁ NHÂN
### (Cardiovascular Disease Prediction based on Personal Health Indicators)

## 👥 Thành viên nhóm thực hiện
| STT | Họ và tên | Mã số sinh viên |
|:---:|:---|:---:|
| 1 | **Nguyễn Thảo Quyên** | 2351060031 |
| 2 | **Nguyễn Phạm Triệu Vỹ** | 2351060042 |

---

## 📖 Giới thiệu (Introduction)
Dự án xây dựng mô hình Học máy để dự đoán nguy cơ mắc bệnh tim mạch. Hệ thống bao gồm quy trình phân tích dữ liệu (EDA), tiền xử lý (Preprocessing) và so sánh hiệu quả giữa hai mô hình chính: **Random Forest** và **XGBoost**.

---

## 📂 Cấu trúc dự án (Project Structure)

Dưới đây là danh sách chi tiết toàn bộ các file trong dự án:

```text
📁 Project-Machine-learning-final
│
├── 📁 RF                               # Thư mục chứa mô hình Random Forest
│   ├── X_test_cardio.csv               # Dữ liệu đặc trưng dùng để test (Input)
│   ├── feature_importance.csv          # File lưu mức độ quan trọng của các đặc trưng
│   ├── loaded_model_rf_final.py        # Code Python để load và chạy model RF
│   ├── predictions_cardio.csv          # Kết quả dự đoán xuất ra từ model
│   ├── preprocessor.pkl                # File pipeline tiền xử lý đã lưu
│   ├── rf_model_thresh0.35.zip         # File model RF đã huấn luyện (nén)
│   └── y_test_cardio.csv               # Nhãn thực tế dùng để đối chiếu (Ground Truth)
│
├── 📁 xgboost                          # Thư mục chứa mô hình XGBoost
│   ├── X_test_fe (1).csv               # Dữ liệu đặc trưng dùng để test (đã Feature Engineering)
│   ├── feature_importance_loaded.png   # Ảnh biểu đồ mức độ quan trọng của đặc trưng
│   ├── loaded_model_xgboost (1).py     # Code Python để load và chạy model XGBoost
│   ├── predictions.csv                 # Kết quả dự đoán xuất ra từ model
│   ├── xgb_model_thresh0.35.pkl        # File model XGBoost đã huấn luyện
│   └── y_test (1).csv                  # Nhãn thực tế dùng để đối chiếu
├── 📂 Logistic Regression/
│   ├── X_train_logistic.xlsx
│   ├── X_test_logistic.xlsx
│   ├── y_train_logistic.xlsx
│   ├── y_test_logistic.xlsx
│   ├── bang_predict (1).xlsx
│   ├── predictions_logistic.csv
│   ├── logistic_model_thresh0.35.pkl
│   ├── load_and_predict.py
│   └── threshold_model.py
├── EDA (1).ipynb                       # Notebook Phân tích dữ liệu khám phá (EDA)
├── FINAL_PROJECT_ML.pdf                # File báo cáo tiểu luận cuối kỳ (PDF)
├── README.md                           # File hướng dẫn này
└── data_preprocessing (1).py           # Code chứa Pipeline tiền xử lý dữ liệu
