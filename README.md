# walmart-sales-forecasting

## 📌 Mô tả đề tài
Dự án này tập trung vào việc phân tích và dự báo doanh thu hàng tuần của các cửa hàng thuộc chuỗi bán lẻ Walmart. Dữ liệu phản ánh các yếu tố kinh tế, thời tiết, ngày lễ và chương trình giảm giá, nhằm xây dựng mô hình giúp tối ưu hóa hàng tồn kho, nhân sự và chiến lược kinh doanh.

---

## 🎯 Mục tiêu
- Phân tích mối quan hệ giữa các yếu tố kinh tế, thời tiết, khuyến mãi và doanh thu.
- Xây dựng mô hình dự báo doanh thu theo thời gian cho từng cửa hàng và phòng ban.
- Đánh giá hiệu quả các chiến dịch giảm giá và ảnh hưởng của yếu tố vĩ mô đến doanh số.
- So sánh hiệu suất giữa các mô hình Machine Learning truyền thống và mô hình chuỗi thời gian.

---

## 📂 Cấu trúc bộ dữ liệu

| Tệp tin        | Nội dung chính |
|----------------|----------------|
| `train.csv`    | 421,570 dòng - Doanh thu hàng tuần (Weekly_Sales) theo từng cửa hàng và phòng ban |
| `test.csv`     | 115,064 dòng - Dữ liệu kiểm tra không có cột doanh thu |
| `features.csv` | 8,190 dòng - Các yếu tố ảnh hưởng: CPI, nhiệt độ, tỷ lệ thất nghiệp, Markdown... |
| `stores.csv`   | 45 dòng - Thông tin cửa hàng: loại cửa hàng, diện tích |

---

## 🔍 Bài toán và phương pháp

### Loại bài toán:
- **Time Series Forecasting**: Dự báo doanh thu dựa vào thời gian.
- **Regression**: Phân tích mối quan hệ giữa các biến độc lập và doanh thu.

### Input:
- Ngày, loại cửa hàng, diện tích, CPI, tỷ lệ thất nghiệp, giá nhiên liệu, khuyến mãi (Markdown), ngày lễ...

### Output:
- Doanh thu hàng tuần (`Weekly_Sales`) của từng cửa hàng và phòng ban.

---

## 🧠 Các mô hình sử dụng

### Mô hình truyền thống:
- Random Forest
- XGBoost

### Mô hình chuỗi thời gian:
- ARIMA
- Prophet
- LSTM

---

## ⚙️ Tiền xử lý dữ liệu
- Xử lý dữ liệu thiếu (đặc biệt ở cột `MarkDown`, `CPI`, `Unemployment`)
- Chuẩn hóa và mã hóa dữ liệu phân loại (categorical)
- Trích xuất đặc trưng thời gian (ngày, tuần, năm, kỳ nghỉ)
- Kết hợp dữ liệu từ các tệp `features.csv`, `stores.csv` và `train.csv`

---

## 📊 Phân tích và trực quan hóa
- Phân tích xu hướng doanh thu theo thời gian và mùa vụ
- Tác động của ngày lễ và chương trình giảm giá đến doanh thu
- Tương quan giữa yếu tố vĩ mô và lượng bán

---

## 🧩 Hạn chế
- Dữ liệu thiếu ở một số cột quan trọng
- Không có thông tin chi tiết theo từng sản phẩm (chỉ có theo phòng ban)
- Cần xác định rõ ràng chu kỳ thời gian (weekly) cho mô hình time series

---

## 💡 Ứng dụng thực tiễn
- Hỗ trợ ra quyết định về nhập hàng và quản lý tồn kho
- Dự báo nhu cầu và lập kế hoạch nhân sự
- Đánh giá hiệu quả chương trình khuyến mãi
- Phân tích tác động từ yếu tố vĩ mô đến hoạt động kinh doanh bán lẻ

---

## ✅ Kết luận
Dự án "Walmart Sales Forecast" là một bài toán tổng hợp, kết hợp giữa phân tích dữ liệu, trực quan hóa và xây dựng mô hình dự báo. Qua đó, người thực hiện có thể rèn luyện toàn diện kỹ năng trong lĩnh vực **Data Science**, **Machine Learning** và **Time Series Forecasting**.

---
