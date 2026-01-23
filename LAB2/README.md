#  Thực Hành Deep Learning – Tuần 2  
## Làm Chủ NumPy, Pandas & Matplotlib

---

## 1. Công Nghệ Sử Dụng

- **Python**  
  Ngôn ngữ lập trình chính cho toàn bộ bài thực hành

- **NumPy**  
  Xử lý mảng số học, ma trận và tính toán hiệu năng cao

- **Matplotlib (giới thiệu)**  
  Trực quan hóa dữ liệu bằng biểu đồ

- **Terminal / VS Code / Jupyter Notebook**  
  Môi trường phát triển và kiểm tra mã nguồn

---

## 2️. Các Bài Thực Hành Chi Tiết

---

### Bài 1: Ứng Dụng NumPy Vào Game 

**Mục tiêu:**  
Sử dụng NumPy array để xây dựng game hoàn chỉnh.

**Yêu cầu thực hiện:**

- Khởi tạo bàn cờ **3 × 3** bằng NumPy array
- Quy ước giá trị:
  - `99` → ô trống  
  - `1` → X  
  - `0` → O
- Người chơi nhập tọa độ `(hàng, cột)` để đánh dấu

**Thuật toán kiểm tra thắng:**

- 3 ô liên tiếp trên **cùng hàng**
- 3 ô liên tiếp trên **cùng cột**
- 3 ô liên tiếp trên **đường chéo chính hoặc phụ**

 **Game kết thúc khi có người chiến thắng**

---

### Bài 2: Kỹ Thuật Trích Xuất Phần Tử Ma Trận

**Mục tiêu:**  
Làm chủ indexing và slicing trong NumPy.

**Nội dung thực hành:**

- Tạo ma trận **3 × 3** bằng NumPy
- Thực hành indexing đa chiều:
  - Trích xuất toàn bộ **hàng** hoặc **cột**
  - Truy cập **phần tử đơn lẻ** bằng tọa độ
  - Lấy phần tử theo **pattern cụ thể**
  - Trích xuất phần tử theo **thứ tự đảo ngược**

 **Ứng dụng:** Xử lý dữ liệu dạng bảng và ma trận

---

### Bài 3: Phương Pháp Lọc Dữ Liệu

**Mục tiêu:**  
So sánh các cách lọc dữ liệu trong Python và NumPy.

#### Cách 1: Vòng lặp `for` truyền thống
- Kiểm tra điều kiện `i % 2 == 0`
- Thu thập các số chẵn vào danh sách mới

#### Cách 2: List Comprehension (Pythonic)
- Cú pháp ngắn gọn, dễ đọc
- Hiệu suất tốt hơn vòng lặp thông thường

#### Cách 3: NumPy Boolean Indexing
- Áp dụng **vectorization**
- Xử lý toàn bộ array cùng lúc
- Tốc độ vượt trội khi làm việc với dữ liệu lớn

---

### Bài 4: Chuẩn Bị Dữ Liệu Cho Machine Learning

**Mục tiêu:**  
Làm quen với pipeline chuẩn bị dữ liệu cho ML.

#### Bước 1: Tạo dataset giả lập
- Kích thước: **150 × 5**
- Gồm:
  - **4 features**: chiều cao, cân nặng, tuổi, lương
  - **1 label**: điểm trung bình

#### Bước 2: Tách Features và Labels

X = data[:, :4]   # 4 cột đầu
y = data[:, 4]    # cột cuối

#### Bước 3: Chia tập Train / Test

- Train: 70% dữ liệu (~105 mẫu)
- Test: 30% dữ liệu (~45 mẫu)

#### Bước 4: Tạo Cross-Validation Folds

- Chia tập train thành 10 folds
- Mỗi fold ≈ 10 mẫu
- Không chồng chéo dữ liệu giữa các fold

## 3. Kết Quả Đạt Được
### Kỹ Năng NumPy
- Thành thạo khởi tạo và thao tác mảng đa chiều

- Làm chủ indexing, slicing và boolean masking

- Hiểu và áp dụng vectorization để tối ưu hiệu năng

### Ứng Dụng Thực Tế

- Xây dựng game Tic-Tac-Toe hoàn chỉnh

- Xử lý dữ liệu dạng ma trận và bảng biểu

- Áp dụng vào các bài toán lọc và biến đổi dữ liệu

### Chuẩn Bị Cho Machine Learning

- Nắm vững pipeline chuẩn bị dữ liệu cơ bản

- Hiểu nguyên lý chia tập train/test

- Biết cách tạo cross-validation folds

- Sẵn sàng cho các bài toán phân tích dữ liệu phức tạp