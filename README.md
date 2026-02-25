Link dataset: https://www.kaggle.com/datasets/fronkongames/steam-games-dataset/discussion


🎮 Steam Games Data Analysis & Revenue Prediction
📌 Giới thiệu dự án

Dự án này thực hiện phân tích dữ liệu các trò chơi trên nền tảng Steam nhằm:

Khám phá xu hướng phát hành game

Phân tích đặc điểm publisher

Phân tích hệ điều hành được hỗ trợ

Đánh giá mức độ tương tác người dùng

Xây dựng mô hình Machine Learning dự đoán số lượng người chơi ước tính của game

Dataset được thu thập từ Kaggle và xử lý lại để đảm bảo tính nhất quán và chính xác.

📊 Nội dung phân tích
1. Data Cleaning

Xử lý lỗi lệch cột trong file CSV

Chuyển đổi kiểu dữ liệu (object → numeric)

Tính toán:

total_reviews

review_ratio

estimated_revenue

Loại bỏ giá trị thiếu và outliers

2. Exploratory Data Analysis (EDA)

Các phân tích chính:

Phân bố hệ điều hành hỗ trợ (Windows, Mac, Linux)

Top 10 Publishers theo số lượng game

Phân tích số lượng review

Phân tích giá game

Phân tích tương quan giữa các biến

Nhận xét nổi bật:

Thị trường có xu hướng tập trung vào một số publisher lớn

Phần lớn game hỗ trợ Windows

Phân phối doanh thu có tính chất lệch phải (right-skewed)

🤖 Machine Learning
🎯 Bài toán

Bài toán được xây dựng dưới dạng Regression với mục tiêu:

Dự đoán số lượng người chơi trung bình (estimated_owners_mid) của game.

📌 Feature sử dụng
    "price",
    "release_year",
    "positive_ratio",
    "total_reviews",
    "windows",
    "mac",
    "linux"

🔧 Mô hình thử nghiệm

Linear Regression

Random Forest Regressor

Gradient Boosting

📈 Đánh giá mô hình

Sử dụng các chỉ số:

MAE

RMSE

R² Score

Kết quả cho thấy các mô hình phi tuyến (Random Forest, Gradient Boosting) cho hiệu suất tốt hơn so với Linear Regression.

Điều này cho thấy số lượng người chơi trung bình chịu ảnh hưởng từ mối quan hệ phi tuyến giữa nhiều yếu tố.

🛠 Công nghệ sử dụng

Python

Pandas

NumPy

Matplotlib

Scikit-learn

Jupyter Notebook

📌 Kết luận

Dự án giúp hiểu rõ hơn về cấu trúc thị trường game trên Steam và xây dựng mô hình dự đoán số lượng người chơi trung bình dựa trên các đặc trưng quan trọng.

Machine Learning cho thấy các yếu tố như giá game và đánh giá tích cực có ảnh hưởng mạnh đến trải nghiệm chơi game.
