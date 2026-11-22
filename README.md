# ỨNG DỤNG TRÍ TUỆ NHÂN TẠO (AI) TRONG PHÁT HIỆN TIN GIẢ TRÊN MẠNG XÃ HỘI TIẾNG VIỆT

## 1. Giới thiệu đề tài
Sự bùng nổ của các nền tảng mạng xã hội (Facebook, TikTok, YouTube) khiến tin giả (Fake News) lan truyền với tốc độ nhanh hơn gấp nhiều lần so với thông tin chính thống[cite: 6]. Dự án này xây dựng mô hình học máy và xử lý ngôn ngữ tự nhiên (NLP) nhằm tự động nhận diện và phân loại tin thật – tin giả tiếng Việt trên không gian mạng[cite: 6].

## 2. Mục tiêu nghiên cứu
* Xây dựng quy trình tiền xử lý và trích xuất đặc trưng ngôn ngữ cho văn bản tiếng Việt trên mạng xã hội[cite: 6].
* Huấn luyện, đánh giá và so sánh hiệu năng giữa các mô hình Học máy truyền thống (Multinomial Naive Bayes, SVM) và Học sâu (PhoBERT) trong bài toán phát hiện tin giả[cite: 6].

## 3. Phương pháp thực hiện
* **Tập dữ liệu:** Bộ dữ liệu *VFND (Vietnamese Fake News Dataset)* gồm 5.000 bài viết (2.500 tin thật, 2.500 tin giả), chia tỷ lệ 80% huấn luyện – 20% kiểm thử[cite: 6].
* **Quy trình:** Làm sạch dữ liệu & tách từ tiếng Việt (*Underthesea*) $\rightarrow$ Trích xuất đặc trưng (*TF-IDF* và *Word Embeddings*) $\rightarrow$ Huấn luyện mô hình (*Scikit-learn, PyTorch*) $\rightarrow$ Đánh giá qua các chỉ số *Accuracy, Precision, Recall, F1-score*[cite: 6].

## 4. Kết quả chính
* Mô hình học sâu **PhoBERT** đạt hiệu năng vượt trội nhất với **Accuracy đạt 94.2%** và **F1-Score đạt 94.0%**, cao hơn đáng kể so với **SVM** (89.5%) và **Naive Bayes** (85.1%).

## 5. Cấu trúc thư mục dự án
* `data/`: Chứa tập dữ liệu thô và dữ liệu đã qua tiền xử lý[cite: 1, 2].
* `src/`: Mã nguồn huấn luyện mô hình và đánh giá kết quả[cite: 1, 2].
* `docs/`: Tài liệu báo cáo, poster khoa học và hướng dẫn sử dụng[cite: 1, 2].
* `results/`: Lưu trữ biểu đồ trực quan hóa và bảng kết quả thực nghiệm[cite: 1, 2].

## 6. Giấy phép sử dụng (License)
Dự án này được phát hành dưới giấy phép **MIT License**. Xem chi tiết điều khoản tại tệp [LICENSE](./LICENSE).
