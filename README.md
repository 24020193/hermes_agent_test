# 🤖 Hermes Agent System (`hermes_agent_test`)

Hệ thống đa Agent tự động thông minh (Multi-Agent System) quản lý không gian thảo luận, tự động cập nhật tin tức, tổng hợp thông tin và gợi ý chủ đề tương tác mỗi ngày.

---

## 🏛️ Kiến trúc & Phân vai hệ thống (Profiles)

Dự án bao gồm các tác nhân (Agents) hoạt động phối hợp trong một "phòng chính", dưới sự điều phối của một Agent Quản lý:

| Tên Agent Profile | Vai trò / Vị trí | Nhiệm vụ chính |
| :--- | :--- | :--- |
| **`agent_main`** | **Quản lý chính** | Điều phối toàn bộ hoạt động, giám sát phòng chính và quản lý tài nguyên hệ thống. |
| **`agent_new`** | chuyên gia tin tức | Tự động quét và **gửi tin tức mới nhất vào lúc 7:30 sáng** mỗi ngày. |
| **`agent_summary`** | chuyên gia tổng hợp | **Tổng hợp nội dung thảo luận** ngày hôm trước của *tất cả các profile* vào lúc 7:30 sáng, hoặc **tự động gợi ý chủ đề mới** nếu hôm trước không có thảo luận. |

---

## ⚙️ Tính năng cốt lõi (Core Features)

* **🧠 Lưu trữ Bộ nhớ (Memory Storage):** Hệ thống có khả năng lưu trữ nhật ký thảo luận và lịch sử tương tác giữa các profile, đảm bảo tính liên tục của thông tin.
* **⚡ Kỹ năng Tự sinh (Self-Generating Skills):** Các Agent sở hữu `skill` tự sinh, cho phép chúng tự động nâng cấp hoặc tạo ra các kỹ năng xử lý mới dựa trên ngữ cảnh công việc.
* **⏰ Lịch trình tự động (Cron-Jobs):** Hoạt động đồng bộ hóa mốc thời gian biểu cố định (7h30 sáng hàng ngày) để báo cáo tin tức và tổng hợp.

---


