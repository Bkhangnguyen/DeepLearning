# Bài Tập Xử Lý Dữ liệu với Pandas
## BTVN 01 - Tiền xử lý dữ liệu cơ bản

Mục tiêu: Chuyển đổi dữ liệu thô thành dữ liệu sạch, sẵn sàng cho quá trình huấn luyện mô hình.
---

### 1. Khám phá dữ liệu
- Sử dụng `head()` và `tail()` để xem cấu trúc dữ liệu
- Kiểm tra thông tin tổng quan: `shape`, `columns`, `describe`

### 2. Làm sạch dữ liệu
- Xóa cột `Hepatitis B` và `Population` do có nhiều giá trị thiếu
- Đổi tên cột `thinness 1-19 years` thành tên ngắn gọn hơn

### 3. Chuẩn hóa dữ liệu
- Ánh xạ giá trị trong cột `Status`:
  - "Developing" ra 0
  - "Developed" ra 1

### 4. Tách dữ liệu
- **X (Features):** Tất cả các cột trừ `Life expectancy`
- **y (Target):** Cột `Life expectancy`
---

## BTVN 02 - Xử lý giá trị khuyết và phân tích nhóm

---

### 1. Xử lý dữ liệu khuyết
- Đếm giá trị thiếu: `isnull().sum()`
- Thay thế bằng giá trị trung bình (`mean`) thay vì xóa dòng

### 2. Phân tích theo nhóm
- **Nhóm theo Quốc gia:** So sánh tuổi thọ giữa các nước
- **Nhóm theo Status:** So sánh tuổi thọ giữa nhóm phát triển và đang phát triển

*Cơ chế:* Chia dữ liệu thành các nhóm con và tính toán riêng biệt

### 3. Gộp dữ liệu
- Tạo bảng phụ `Noise_level`
- Ghép với bảng chính bằng khóa chung (ví dụ: `Country`)

---

## Kết luận tổng kết

### Kết quả đạt được

**Bài tập 01 - Tiền xử lý dữ liệu:**
- Đã loại bỏ 2 cột không cần thiết (`Hepatitis B`, `Population`)
- Chuẩn hóa cột `Status` thành dạng số (0, 1)
- Đổi tên cột dài thành tên ngắn gọn
- Tách thành công features (X) và target (y) cho ML

**Bài tập 02 - Xử lý nâng cao:**
- Xử lý triệt để dữ liệu khuyết bằng phương pháp thay thế
- Phân tích nhóm cho thấy chênh lệch tuổi thọ rõ rệt giữa các quốc gia
- Thành công ghép thêm dữ liệu mới vào dataset gốc

###  Nận xét chung

1. **Dữ liệu đầu vào** đã được làm sạch hoàn toàn, sẵn sàng cho training
2. **Quy trình xử lý** tuân thủ đúng các bước tiêu chuẩn trong data pipeline
3. **Kết quả phân tích** cung cấp insights hữu ích về mối quan hệ giữa phát triển kinh tế và tuổi thọ
