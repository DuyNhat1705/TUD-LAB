---
title: TUD Lab — Applied Mathematics
---

# TUD Lab — Applied Mathematics

Chào mừng bạn đến với **TUD Lab Book** — Không gian lưu trữ và trình bày các bài tập thực hành (Lab) cùng đồ án môn học **Toán ứng dụng (Applied Mathematics)**.

Tài liệu được biên soạn dưới dạng Jupyter Notebook và xuất bản trực quan với **Jupyter Book / MyST Markdown**. Các bài tập tập trung vào việc hiện thực hóa thuật toán toán học bằng Python (cài đặt trực tiếp các phép biến đổi ma trận, hệ phương trình, đại số tuyến tính) và ứng dụng vào phân tích dữ liệu thực tế.

---

## Thông tin sinh viên

- **Họ và tên:** Vũ Duy Nhất
- **MSSV:** 24127095
- **Môn học:** Toán ứng dụng (Applied Mathematics)
- **GitHub:** [DuyNhat1705](https://github.com/DuyNhat1705/TUD-LAB)
- **Trang trực tuyến:** [duynhat1705.github.io/TUD-LAB](https://duynhat1705.github.io/TUD-LAB/)

---

## Danh mục Lab & Đồ án

::::{grid} 1 1 2 2
:gutter: 3

:::{card} [Lab 1: Gauss Elimination](1-Gauss.ipynb)
**Khử Gauss & Giải hệ phương trình tuyến tính**

Biến đổi sơ cấp trên dòng, đưa ma trận về dạng bậc thang (REF) và bậc thang rút gọn (RREF); thuật toán thế ngược (Back-substitution); xử lý và biện luận các trường hợp hệ phương trình có nghiệm duy nhất, vô số nghiệm hoặc vô nghiệm.
:::

:::{card} [Lab 2: Gram-Schmidt Process](2-Gram-Schidt.ipynb)
**Trực chuẩn hóa & Phân rã ma trận QR**

Thuật toán trực giao hóa và trực chuẩn hóa Gram-Schmidt cho hệ vectơ độc lập tuyến tính; xây dựng ma trận trực chuẩn $Q$ và ma trận tam giác trên $R$ ($A = QR$); ứng dụng phân rã QR để giải hệ phương trình tuyến tính.
:::

:::{card} [Lab 3: Diagonalizable Matrix](<3-Diagonalizable Matrix.ipynb>)
**Chéo hóa ma trận & Không gian riêng**

Tính đa thức đặc trưng $\det(A - \lambda I)$, tìm trị riêng (eigenvalues) và vectơ riêng (eigenvectors); kiểm tra điều kiện chéo hóa; xây dựng ma trận làm chéo $P, P^{-1}$ và ma trận đường chéo $D$ sao cho $A = PDP^{-1}$; ứng dụng tính lũy thừa cấp cao $A^k$.
:::

:::{card} [Lab 4: Linear Regression](<4-Linear Regression.ipynb>)
**Hồi quy tuyến tính (Ordinary Least Squares)**

Xây dựng mô hình hồi quy tuyến tính bằng phương pháp bình phương cực tiểu (OLS); giải phương trình chuẩn $\hat{\beta} = (X^T X)^{-1} X^T y$; đánh giá và lựa chọn đặc trưng tối ưu thông qua K-Fold Cross Validation trên tập dữ liệu thực tế.
:::

:::{card} [Final Project: Markov Chain](<5-Markov Chain.ipynb>)
**Ứng dụng xích Markov trong thị trường tài chính**

Đồ án cuối kỳ: Thu thập chuỗi thời gian tài chính S&P 500 từ `yfinance`; phân chia các trạng thái thị trường (Tăng, Giảm, Đi ngang); ước lượng ma trận xác suất chuyển tiếp trạng thái $P$; phân tích phân phối dừng $\pi$ và mở rộng mô hình không gian trạng thái đa chiều.
:::

::::

---

## Công nghệ & Công cụ sử dụng

- **Ngôn ngữ:** Python 3.12
- **Biên soạn & Xuất bản:** Jupyter Notebook, Jupyter Book v2 (MyST Markdown)
- **Thư viện tính toán & Đại số tuyến tính:** `numpy`, `sympy`, `scipy`
- **Xử lý dữ liệu & Học máy:** `pandas`, `scikit-learn`
- **Dữ liệu tài chính & Trực quan hóa:** `yfinance`, `matplotlib`
- **CI/CD:** GitHub Actions tự động build và deploy lên GitHub Pages
