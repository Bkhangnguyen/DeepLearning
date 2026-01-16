# README – Bài tập thực hành PyTorch

## 1. Công nghệ và công cụ sử dụng

- **Ngôn ngữ lập trình:** Python 3
- **Thư viện học máy chính:** PyTorch
- **Môi trường phát triển:** VS Code hoặc Jupyter Notebook
- **Nội dung kiến thức thực hành:**
  - Làm việc với Tensor
  - Cơ chế tự động tính đạo hàm (Autograd)
  - Thuật toán Gradient Descent
  - Xây dựng mô hình Hồi quy Tuyến tính (Linear Regression)
  - Quản lý và chia sẻ bộ nhớ giữa NumPy và PyTorch
---
## Các bài tập : 

### Bài 1: Tính đạo hàm đa thức
- Xác định một hàm đa thức bậc 5
- Sử dụng PyTorch để tính đạo hàm tự động (automatic differentiation)
- Xác định độ dốc của hàm tại một điểm `x` cụ thể

### Bài 2: Gradient và Gradient Descent thủ công
- Khởi tạo một tensor `x = 2` với cờ `requires_grad = True`
- Định nghĩa và tính gradient của một hàm bậc 3 theo `x`
- Áp dụng thuật toán **Gradient Descent** với tốc độ học `α = 0.1`
- Thực hiện cập nhật giá trị của `x` qua 10 bước lặp

### Bài 3: Xây dựng mô hình Hồi quy Tuyến tính
- Tạo bộ dữ liệu mẫu (synthetic dataset) với:
  - Đặc trưng `x`: số giờ học (giá trị ngẫu nhiên từ 1 đến 10)
  - Nhãn `y`: được tạo theo công thức `y = 3x + 5` cộng thêm nhiễu
- Khởi tạo ngẫu nhiên các tham số mô hình `w` (trọng số) và `b` (hệ số điều chỉnh)
- Tính hàm mất mát **Mean Squared Error (MSE)**
- Sử dụng Gradient Descent để cập nhật `w` và `b`
- Huấn luyện mô hình trong 100 epoch

### Bài 4: Chia sẻ bộ nhớ giữa NumPy và PyTorch
- Thực hành tạo tensor từ mảng NumPy bằng hai phương pháp:
  - `torch.from_numpy()`
  - `torch.tensor()`
- Phân tích sự khác biệt về **cơ chế quản lý bộ nhớ** 
- Minh họa trường hợp tensor thay đổi khi mảng NumPy gốc thay đổi

### Bài 5: Tạo và biến đổi hình dạng Tensor
- Thực hành tạo tensor với các hàm khởi tạo:
  - `empty`
  - `zeros`
  - `ones`
  - `random`
- Thay đổi kích thước tensor bằng các phương thức:
  - `view()`
  - `view_as()`
- Hiểu nguyên tắc reshape **không sao chép dữ liệu** (non-copying)

---
