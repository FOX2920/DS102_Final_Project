# Spam or Ham Email Classifier
Dự án này xây dựng một mô hình phân loại email là spam (thư rác) hay ham (thư hợp lệ) bằng cách áp dụng các kỹ thuật máy học và xử lý ngôn ngữ tự nhiên. Mục tiêu là tạo ra một mô hình phân loại hiệu quả, giúp lọc và phân loại email một cách chính xác.

### Các bước thực hiện
+ Thu thập và tiền xử lý dữ liệu: Thu thập dữ liệu email từ nguồn dữ liệu có sẵn, tiền xử lý dữ liệu bằng cách loại bỏ các ký tự đặc biệt, chuyển về chữ thường, tokenize, loại bỏ stopwords, stemming.
+ Đặc trưng hóa dữ liệu: Sử dụng TF-IDF và CountVectorizer để biểu diễn văn bản thành vector đặc trưng.
+ Xây dựng mô hình: Thử nghiệm các thuật toán máy học khác nhau như Naive Bayes, Logistic Regression, XGBoost, Support Vector Machine. Tiến hành tìm kiếm tham số tối ưu cho từng mô hình bằng GridSearchCV.
+ Đánh giá mô hình: Sử dụng các chỉ số đánh giá như Accuracy, Precision, Recall, **F1-score** để so sánh hiệu suất của các mô hình.
+ Lựa chọn mô hình tốt nhất: Dựa trên kết quả đánh giá, lựa chọn mô hình phù hợp nhất cho bài toán phân loại spam/ham.
### Kết quả
Trong dự án này, mô hình SVM với TF-IDF Vectorizer đạt được kết quả tốt nhất với F1-score là 90%. Mô hình XGBoost với CountVectorizer cũng cho kết quả khá tốt với độ chính xác 94.42% và F1-score 89.98%.
![image](https://github.com/FOX2920/DS102_Final_Project/assets/91709267/85d6f967-23b7-4644-a5ef-0ec03d1b800e)

### Cách sử dụng
+ Cài đặt các thư viện cần thiết: ```pip install -r requirements.txt```
+ Chạy file spam_or_ham_classifier_final1.ipynb để huấn luyện và đánh giá các mô hình.
+ Sử dụng hàm predict trong file trên để dự đoán nhãn spam/ham cho một email mới.
