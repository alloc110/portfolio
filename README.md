# 🚀 Nguyễn Hùng Thiên Lộc — Data & AI Engineering Portfolio

[![GitHub Pages](https://img.shields.io/badge/GitHub%20Pages-Live%20Portfolio-blue?style=for-the-badge&logo=githubpages&logoColor=white)](https://alloc110.github.io/portfolio/)
[![LinkedIn](https://img.shields.io/badge/LinkedIn-Nguyen_Hung_Thien_Loc-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://linkedin.com/in/nguyenhtloc110)
[![GitHub](https://img.shields.io/badge/GitHub-alloc110-181717?style=for-the-badge&logo=github&logoColor=white)](https://github.com/alloc110)

Trang Portfolio cá nhân của **Nguyễn Hùng Thiên Lộc** — Kỹ sư Dữ liệu (Data Engineer) chuyên sâu về **Data Warehouse (PostgreSQL, dbt)**, **Real-Time Streaming Systems (Golang, Kafka, Flink, Redis)** và **AI Agents / Text-to-SQL**.

---

## 🌟 3 Dự Án Flagship Nổi Bật (Featured Repositories)

### 1. 🛡️ [Real-Time Fraud Detection Platform (J-DataPipe)](https://github.com/alloc110/Fraud-Detection-System)
> **Stack:** `Golang 1.21` • `Apache Kafka` • `Redis` • `XGBoost` • `gRPC/Protobuf` • `PostgreSQL 15` • `Kubernetes (HPA)` • `Grafana`
- **Mô tả:** Nền tảng chặn gian lận giao dịch tài chính thời gian thực theo cơ chế **In-line Pre-authorization Blocking**.
- **Điểm nổi bật:**
  - Cổng thanh toán Golang hiệu năng cao, giải quyết nút thắt GIL và context switching.
  - Kiểm tra số dư trên Redis Cache và kết nối suy luận XGBoost qua gRPC multiplexing & Protobuf nén payload.
  - Cơ chế ghi bất đồng bộ Write-Behind qua Kafka vào PostgreSQL; tự động co giãn Pods linh hoạt trên Kubernetes HPA.
  - **Benchmark đã kiểm chứng:** Duy trì ổn định **300 concurrent TPS (>18,000 tx/phút)** với **100% tỷ lệ thành công** và độ trễ E2E **836 ms** (đáp ứng tiêu chuẩn ngân hàng `< 2s`).

---

### 2. 🏠 [ClawSense: FinHouse Price Intelligence & Text-to-SQL](https://github.com/alloc110/ClawSense)
> **Stack:** `Python 3.11` • `FastAPI` • `Google Gemini AI` • `LangChain` • `dbt-core 1.7` • `PostgreSQL 15` • `Jenkins CI/CD` • `Docker` • `Prometheus & Grafana`
- **Mô tả:** Hệ thống phân tích giá và trí tuệ thị trường bất động sản thông minh thời gian thực tích hợp AI Agent và quy trình ELT tự động.
- **Điểm nổi bật:**
  - Quy trình tự động hóa chuyển đổi dữ liệu nhiều tầng theo kiến trúc **Medallion (Bronze Raw → Silver Normalized → Gold Data Marts)** bằng dbt-core qua Jenkins Pipeline CI/CD.
  - Tích hợp **AI Agent Text-to-SQL** (FastAPI + LangChain + Gemini AI) cho phép người dùng đặt câu hỏi tự nhiên và nhận về câu truy vấn SQL cùng báo cáo phân tích giá.
  - Giám sát toàn diện build duration, pipeline health và database metrics qua Prometheus và Grafana.

---

### 3. 🎯 [FindMyBoss: IT Job Harvester & LaTeX CV Studio](https://github.com/alloc110/FindMyBoss)
> **Stack:** `Python 3.12` • `FastAPI` • `Multi-Provider AI (Gemini, Claude, GPT-4o, DeepSeek)` • `Tectonic XeTeX (Rust)` • `Playwright Chromium` • `SQLite WAL` • `Docker Compose`
- **Mô tả:** Nền tảng thu hoạch tin tuyển dụng IT từ 6 cổng thông tin lớn tại VN, phân tích khoảng cách ATS và xưởng tạo CV LaTeX tự động.
- **Điểm nổi bật:**
  - Cào dữ liệu tuyển dụng từ **6 cổng** (ITviec, TopDev, TopCV, VietnamWorks, JobsGO, Indeed VN) với Playwright Chromium và cơ chế chống chặn IP.
  - Nạp Master CV PDF làm "Source of Truth" để chống AI bịa đặt kinh nghiệm, áp dụng tiêu chuẩn viết CV STAR / Google XYZ.
  - Trình soạn thảo Overleaf-style Side-by-Side biên dịch PDF trong **2.7 giây** nhờ engine Tectonic XeTeX (Rust) siêu nhẹ mà không cần bộ cài TeXLive 5GB.
  - Kiến trúc 3 Docker Microservices phân lập (Web Studio, LaTeX Renderer, Scraper Worker) với **24/24 passing unit tests**.

---

## 💼 Kinh Nghiệm & Thành Tựu

- **Thịnh Thế Vinh Hoa (09/2026 – Hiện tại) — Data Engineer Intern**:
  - Thiết kế PostgreSQL DWH & 30+ ELT pipelines tự động (95% on-schedule) cho tập đoàn bán lẻ 7 thương hiệu.
  - Đối soát dữ liệu (~200K dòng/ngày/thương hiệu), phát hiện 200 điểm lệch và xây dựng automated heal workflows.
  - Triển khai 5+ Grafana dashboards & 9+ alerts real-time (< 1 phút phát hiện sự cố).
  - Tự động hóa báo cáo Metabase, cắt giảm 85% thời gian thủ công (2 giờ/ngày).
- **Gradient Technologies (03/2026 – 06/2026) — Data Engineer Intern**:
  - Pipeline bất đồng bộ Windmill lấy dữ liệu từ 10 REST API tài chính (99% success rate).
  - Phát triển 20+ Python API với latency < 500ms.
- **Giải thưởng & Năng lực thuật toán**:
  - 🥉 **Huy chương Đồng Học sinh Giỏi Quốc gia Tin học (VOI 2024)** (Top 88/235).
  - 🥉 **Huy chương Đồng Olympic Toán học 30-4 (2021)**.
  - 🌐 **Thí sinh ICPC Asia Regional Contest (2024, 2025)**.
  - 🎓 Tốt nghiệp Cử nhân Khoa học Máy tính (Chuyên ngành Khoa học Dữ liệu) — Đại học Mở TP.HCM (HCMOU).
  - 🗣️ Tiếng Anh: **TOEIC 675**.

---

## 🌐 Triển Khai GitHub Pages

Repository này được cấu hình sẵn để triển khai tự động lên GitHub Pages:
- **URL chính thức:** [https://alloc110.github.io/portfolio/](https://alloc110.github.io/portfolio/)
- File `.nojekyll` giúp GitHub Pages phục vụ toàn bộ các tài nguyên trực tiếp mà không qua bộ lọc Jekyll.
