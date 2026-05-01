# DATATHON 2026 - CT PTIT CapyData

Repo này chứa dữ liệu và notebook phân tích cho bài DATATHON 2026. Notebook chính hiện tại là `part2_eda_datathon2026.ipynb`, dùng để đọc các file CSV, tạo bảng/nhận xét EDA và xuất các biểu đồ vào thư mục `eda_figures`.

## Cấu trúc thư mục

```text
.
├── part2_eda_datathon2026.ipynb   # Notebook phân tích EDA và tạo hình kết quả
├── eda_figures/                   # Các biểu đồ PNG được xuất từ notebook
├── customers.csv                  # Dữ liệu khách hàng
├── geography.csv                  # Dữ liệu địa lý
├── inventory.csv                  # Dữ liệu tồn kho
├── order_items.csv                # Chi tiết sản phẩm trong đơn hàng
├── orders.csv                     # Thông tin đơn hàng
├── payments.csv                   # Thông tin thanh toán
├── products.csv                   # Danh mục sản phẩm
├── promotions.csv                 # Thông tin khuyến mãi
├── returns.csv                    # Dữ liệu hoàn trả
├── reviews.csv                    # Đánh giá sản phẩm
├── sales.csv                      # Dữ liệu doanh số tổng hợp
├── shipments.csv                  # Dữ liệu vận chuyển
├── web_traffic.csv                # Dữ liệu truy cập web
├── sample_submission.csv          # File mẫu nộp bài
└── Đề thi Vòng 1.pdf              # Đề bài gốc
```

## Yêu cầu môi trường

- Python 3.10 trở lên
- Jupyter Notebook hoặc JupyterLab
- Các thư viện Python:
  - `numpy`
  - `pandas`
  - `matplotlib`
  - `seaborn`
  - `ipython`

Có thể cài nhanh bằng:

```bash
pip install numpy pandas matplotlib seaborn ipython jupyter
```

## Hướng dẫn chạy lại kết quả

1. Đặt toàn bộ file CSV ở đúng thư mục gốc của repo, cùng cấp với notebook.
2. Mở notebook:

```bash
jupyter notebook part2_eda_datathon2026.ipynb
```

Hoac:

```bash
jupyter lab part2_eda_datathon2026.ipynb
```

3. Chọn `Run All` để chạy lại tất cả cell.
4. Sau khi chạy xong, các biểu đồ sẽ được ghi vào thư mục `eda_figures/`.

Notebook đang sử dụng:

```python
DATA_DIR = Path(".")
FIG_DIR = Path("eda_figures")
```

Vì vậy, nếu đổi vị trí file dữ liệu hoặc thư mục xuất hình, cần cập nhật lại hai biến trên trong notebook.

## Kết quả đầu ra

Thư mục `eda_figures/` hiện gồm các biểu đồ EDA chính:

- `part2_01_revenue_margin_trend.png`
- `part2_02_revenue_seasonality.png`
- `part2_03_product_portfolio.png`
- `part2_04_top_segments_quality.png`
- `part2_05_promotion_tradeoffs.png`
- `part2_06_top_promo_campaigns.png`
- `part2_07_customer_retention_age.png`
- `part2_08_acquisition_profit.png`
- `part2_09_returns_delivery.png`
- `part2_10_size_rating_delivery.png`
- `part2_11_traffic_quality_revenue.png`
- `part2_12_monthly_traffic_revenue.png`
- `part2_13_inventory_risk_map.png`
- `part2_14_inventory_product_risk.png`
