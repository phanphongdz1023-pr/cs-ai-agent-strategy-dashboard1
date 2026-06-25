# 📊 AI Agent CS Strategy & Analytics Dashboard

## 📝 Tổng Quan Dự Án
Dự án xây dựng một **Hệ thống Phân tích & Khuyến nghị Chiến lược** nhằm tối ưu hóa việc tích hợp và ứng dụng AI Agent vào cấu trúc vận hành ngành Khoa học Máy tính (Computer Science). Hệ thống phân tích sâu dữ liệu thực tế từ người lao động (Workers) kết hợp với đánh giá chuyên môn từ các chuyên gia công nghệ (Experts), từ đó đưa ra các lát cắt chiến lược cấp độ tác vụ (Task-level analysis) giúp doanh nghiệp cân bằng giữa hiệu suất công nghệ và quản trị nhân sự.

Ứng dụng được phát triển dưới dạng một **Interactive Dashboard** (Bảng điều khiển tương tác trực quan) thời gian thực bằng Streamlit, tối ưu hóa trải nghiệm trình bày báo cáo và thuyết trình đồ án.

---

## 🎯 4 Bài Toán Chiến Lược Được Giải Quyết
Bảng điều khiển được chia thành 4 phân hệ chiến lược tương ứng với 4 Tabs chức năng trực quan:

* **Tab 1: Điểm Mù Công Nghệ (Technological Blind Spots):** Xác định các tác vụ có năng lực tự động hóa kỹ thuật rất cao ($\ge 4.0/5.0$) nhưng nhân viên lại có xu hướng phản kháng mạnh ($\le 2.0/5.0$) do lo ngại mất quyền kiểm soát hoặc giảm chất lượng giám sát.
* **Tab 2: Đứt Gãy Thế Hệ (Generational Seniority Gap):** Phân tích xu hướng lạm dụng AI cho việc viết mã nguồn thuần túy ở các kỹ sư trẻ (Junior) ít kinh nghiệm, từ đó cảnh báo nguy cơ rỗng kiến thức nền tảng và đề xuất giải pháp đào tạo.
* **Tab 3: Tối Ưu Hóa ROI (ROI Maximization):** Lập bản đồ phân bổ 70% ngân sách IT tập trung vào các tác vụ Cốt lõi (Core) có tần suất lặp lại cao thuộc nhóm ngành nghề có quỹ lương lớn nhằm tối đa hóa chỉ số hoàn vốn tự động hóa.
* **Tab 4: Khung Giới Hạn Tự Trị (Guardrails Architecture):** Thiết lập ma trận ranh giới vận hành cho AI dựa trên mức độ không chắc chắn (Uncertainty) và rủi ro đạo đức (Ethical Concerns). Tự động phân loại luồng công việc thành **Vùng An Toàn** (Cho phép Agent tự trị) và **Vùng Nguy Hiểm** (Bắt buộc duyệt thủ công - Human-in-the-loop).

---

## 📂 Cấu Trúc Thư Mục Dự Án
```text
├── ccan.py                             # File mã nguồn chính khởi chạy ứng dụng Streamlit
├── requirements.txt                    # Danh sách các thư viện Python cần cài đặt
├── domain_worker_desires.csv           # Dữ liệu khảo sát nguyện vọng người lao động
├── domain_worker_metadata.csv          # Dữ liệu thâm niên và thông tin nền nhân sự
├── expert_rated_technological_capability.csv # Đánh giá chuyên gia về năng lực tự động hóa kỹ thuật
└── task_statement_with_metadata.csv    # Danh sách chi tiết và phân loại các tác vụ CS
