# 📘 TUD-LAB — Applied Mathematics Lab & Projects

[![Deploy Jupyter Book](https://github.com/DuyNhat1705/TUD-LAB/actions/workflows/deploy.yml/badge.svg)](https://github.com/DuyNhat1705/TUD-LAB/actions/workflows/deploy.yml)
[![Jupyter Book](https://img.shields.io/badge/built%20with-Jupyter%20Book-orange.svg)](https://jupyterbook.org/)
[![Python](https://img.shields.io/badge/python-3.11-blue.svg)](https://www.python.org/)
[![Website](https://img.shields.io/badge/live%20book-GitHub%20Pages-brightgreen)](https://duynhat1705.github.io/TUD-LAB/)

Repository chứa toàn bộ các bài tập thực hành và đồ án môn học **Toán ứng dụng (Applied Mathematics)**, được biên soạn dưới dạng Jupyter Notebook và xuất bản trực tuyến thông qua **Jupyter Book**.

🌐 **Xem trực tuyến tại:** [https://duynhat1705.github.io/TUD-LAB/](https://duynhat1705.github.io/TUD-LAB/)

---

## 👤 Thông tin sinh viên

- **Họ và tên:** Vũ Duy Nhất
- **MSSV:** 24127095
- **Môn học:** Toán ứng dụng (Applied Mathematics)
- **GitHub:** [@DuyNhat1705](https://github.com/DuyNhat1705)

---

## 📚 Danh sách đề tài & Nội dung

| # | Đề tài | Notebook | Nội dung chính |
|---|--------|----------|----------------|
| 1 | **Gauss Elimination** | [`1-Gauss.ipynb`](Projects/1-Gauss.ipynb) | Khử Gauss giải hệ phương trình tuyến tính, đưa ma trận về dạng bậc thang, phép thế ngược, xử lý nghiệm duy nhất, vô nghiệm và vô số nghiệm. |
| 2 | **Gram-Schmidt Process** | [`2-Gram-Schidt.ipynb`](Projects/2-Gram-Schidt.ipynb) | Trực giao hóa và trực chuẩn hóa hệ vectơ trong không gian Euclid; phân rã ma trận $QR$ ($A = QR$). |
| 3 | **Diagonalizable Matrix** | [`3-Diagonalizable Matrix.ipynb`](Projects/3-Diagonalizable%20Matrix.ipynb) | Tìm giá trị riêng, vectơ riêng, kiểm tra điều kiện chéo hóa và xây dựng phân rã $A = PDP^{-1}$. |
| 4 | **Linear Regression (OLS)** | [`4-Linear Regression.ipynb`](Projects/4-Linear%20Regression.ipynb) | Phương pháp bình phương tối thiểu (Ordinary Least Squares - OLS), nghiệm dạng đóng $\hat{\beta} = (X^T X)^{-1} X^T y$, đánh giá mô hình trên tập dữ liệu thực tế. |
| 5 | **Markov Chain (Final Project)** | [`5-Markov Chain.ipynb`](Projects/5-Markov%20Chain.ipynb) | Ứng dụng xích Markov trong mô hình hóa và dự báo trạng thái thị trường tài chính (dữ liệu S&P 500, ma trận chuyển xác suất, phân phối dừng, mở rộng đa chiều Price $\times$ Volume). |

---

## 📂 Cấu trúc thư mục

```text
TUD-LAB/
├── .github/
│   └── workflows/
│       └── deploy.yml          # GitHub Actions workflow triển khai Jupyter Book lên GitHub Pages
├── Projects/
│   ├── 1-Gauss.ipynb
│   ├── 2-Gram-Schidt.ipynb
│   ├── 3-Diagonalizable Matrix.ipynb
│   ├── 4-Linear Regression.ipynb
│   ├── 5-Markov Chain.ipynb
│   ├── _config.yml             # Cấu hình Jupyter Book
│   └── _toc.yml                # Mục lục sách Jupyter Book
├── requirements.txt            # Thư viện phụ thuộc
└── README.md                   # Tài liệu hướng dẫn
```

---

## 🛠️ Hướng dẫn cài đặt & Chạy cục bộ

### 1. Clone repository
```bash
git clone https://github.com/DuyNhat1705/TUD-LAB.git
cd TUD-LAB
```

### 2. Khởi tạo môi trường ảo (Khuyến nghị)
```bash
# Windows
python -m venv venv
venv\Scripts\activate

# Linux / macOS
python3 -m venv venv
source venv/bin/activate
```

### 3. Cài đặt các thư viện cần thiết
```bash
pip install -r requirements.txt
```

### 4. Mở Notebooks để chạy & kiểm thử
```bash
jupyter lab
# hoặc
jupyter notebook
```

### 5. Build Jupyter Book cục bộ
Để tạo bản dựng HTML cục bộ cho toàn bộ tài liệu:
```bash
jupyter-book build Projects
```
Sau khi build xong, mở file `Projects/_build/html/index.html` trên trình duyệt web để xem kết quả.

---

## 🚀 Tự động hóa triển khai (CI/CD)

Repository đã được tích hợp sẵn GitHub Actions workflow (`.github/workflows/deploy.yml`). Khi có bất kỳ commit mới nào được đẩy lên nhánh `main`, hệ thống sẽ:
1. Tự động thiết lập môi trường Python 3.11.
2. Cài đặt các gói phụ thuộc từ `requirements.txt`.
3. Biên dịch Jupyter Book thành mã nguồn tĩnh HTML.
4. Triển khai trực tiếp lên GitHub Pages tại [duynhat1705.github.io/TUD-LAB](https://duynhat1705.github.io/TUD-LAB/).

---

## 📦 Công nghệ & Thư viện sử dụng

- **Ngôn ngữ:** Python 3.11
- **Công cụ tài liệu:** [Jupyter Book](https://jupyterbook.org/)
- **Tính toán ma trận & Đại số:** `numpy`, `sympy`, `scipy`
- **Xử lý & Thống kê dữ liệu:** `pandas`, `scikit-learn`
- **Dữ liệu tài chính:** `yfinance`
- **Trực quan hóa đồ thị:** `matplotlib`