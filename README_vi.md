<p align="center">
  <img width="100" height="100" alt="logo" src="https://github.com/user-attachments/assets/86f005b2-bc0c-4542-bd70-3d556a4ff8ce" />
</p>

<h1 align="center">Auto Whisk</h1>
<p align="center">
  Tạo ảnh AI hàng loạt với Google Whisk — hoàn toàn tự động.<br>
  Phiên bản 8.3.0 · 7 ngôn ngữ · by <a href="https://duckmartians.info">duckmartians</a><br><br>
  <a href="https://chromewebstore.google.com/detail/auto-whisk-prompt-automat/gedfnhdibkfgacmkbjgpfjihacalnlpn"><img src="https://img.shields.io/badge/⬇_Download-Here-success?style=for-the-badge" alt="Download Here"></a><br><br>
  <a href="README.md"><img src="https://img.shields.io/badge/English-blue" alt="English"></a>
  <a href="README_vi.md"><img src="https://img.shields.io/badge/Tiếng%20Việt-green" alt="Tiếng Việt"></a>
</p>

---

## 📖 Auto Whisk là gì?

Extension trên Chrome giúp **tự động tạo ảnh hàng loạt** trên [Google Whisk AI](https://labs.google/fx/tools/whisk). Thay vì nhập từng mô tả rồi chờ, bạn chỉ cần:

- Nhập **danh sách mô tả** → Extension tạo ảnh lần lượt  
- Bật **tải tự động** → Ảnh về máy ngay khi xong  
- **Tạm dừng / Tiếp tục / Dừng hẳn** bất cứ lúc nào  
- **Thử lại** những ảnh bị lỗi chỉ với 1 click  

> Extension mở dưới dạng **bảng bên hông** (side panel) — không che màn hình chính.

---

## 🚀 Màn Hình Chọn Chế Độ (Gateway)

Bấm biểu tượng extension → bảng bên hông hiện 3 lựa chọn:

| | Chế độ | Mô tả |
|:---:|---|---|
| 🟢 | **7.6.0 — Nhanh** (Khuyên dùng) | Chạy ngầm, không cần mở Whisk. Đầy đủ tính năng. |
| ⚪ | **7.5.1 — Cổ điển** (Dự phòng) | Mô phỏng chuột trên trang Whisk. Dùng khi bản Nhanh lỗi. |
| 🟣 | **G-Labs Automation** | Phần mềm Windows độc lập, không cần trình duyệt. |

🌐 Góc phải trên có nút **đổi ngôn ngữ** (7 ngôn ngữ) — lựa chọn được lưu tự động.

---

## ⚡ Chế Độ Nhanh (7.6.0)

> **Khuyên dùng** — Tốc độ cao, chạy ngầm ổn định, không cần mở trang Whisk.

### Nhập mô tả

Gõ/dán các mô tả vào ô văn bản, hoặc bấm **"Nhập từ file"** để chọn file `.txt`.

**Hai chế độ tách mô tả:**

| Chế độ | Cách hoạt động | Khi nào dùng |
|---|---|---|
| **1 dòng = 1 mô tả** | Mỗi dòng là 1 mô tả riêng | Mô tả ngắn |
| **Cách dòng trống** | Các dòng liền nhau ghép thành 1 mô tả | Mô tả dài nhiều dòng |

### Thiết lập

| Tùy chọn | Chi tiết |
|---|---|
| **Tỉ lệ ảnh** | `1:1` · `16:9` · `9:16` · `4:3` · `3:4` |
| **Số ảnh / mô tả** | 1 → 4 ảnh (VD: 10 mô tả × 3 ảnh = 30 ảnh) |
| **Thư mục lưu** | Tên thư mục con trong Downloads |
| **Tải tự động** | Bật/tắt — mặc định **bật** |

### 🎨 Ảnh tham chiếu

Đính kèm ảnh mẫu để AI bắt chước phong cách, chủ thể hoặc bối cảnh.

Bấm **"Ảnh tham chiếu"** → cửa sổ quản lý hiện ra:

| Nhóm | Mô tả | Tối đa |
|---|---|:---:|
| **Chủ thể** | Nhân vật / đối tượng bạn muốn AI vẽ lại | 2 |
| **Bối cảnh** | Phong cảnh / nền muốn đặt chủ thể vào | 1 |
| **Phong cách** | Phong cách nghệ thuật muốn AI bắt chước | 1 |

**Cách dùng:** Bấm `+` chọn ảnh → Bấm **"Upload & Phân tích"** (AI tự phân tích nội dung) → Sửa caption nếu cần → **"Lưu Caption"** → **"Xong"**.

> Ảnh tham chiếu được áp dụng cho **tất cả** mô tả trong danh sách.

### Điều khiển

| Nút | Chức năng |
|:---:|---|
| ▶ **Bắt đầu** | Khởi chạy tạo ảnh lần lượt |
| ⏸ **Tạm dừng** | Bấm lại để tiếp tục |
| ⏹ **Dừng** | Dừng hẳn toàn bộ |

### Bảng kết quả

| Cột | Ý nghĩa |
|---|---|
| **#** | Số thứ tự |
| **Prompt** | Nội dung mô tả *(có thể sửa trực tiếp)* |
| **IMG 1, 2…** | Ảnh thu nhỏ — bấm để **xem phóng to** |
| **TT** | ⏳ Chờ · 🔄 Đang tạo · ✅ Xong · 🔃 Lỗi *(bấm để thử lại)* |

Nếu có lỗi → nút **"Thử lại các lỗi"** xuất hiện để thử lại tất cả cùng lúc.

### Đăng nhập

Extension **tự lấy phiên đăng nhập** Google của bạn. Nếu chưa có tab `labs.google`, extension tự mở tab ẩn → chờ bạn đăng nhập → lưu phiên tự động. Phiên hết hạn sẽ được **tự làm mới**.

> ⚠️ Bạn cần tài khoản Google có quyền truy cập Google Labs.

---

## 🖱️ Chế Độ Cổ Điển (7.5.1)

> **Dự phòng** — Mô phỏng thao tác chuột trên trang Whisk. Bắt buộc giữ tab Whisk mở.

### Yêu cầu

- Tab Whisk phải **đang mở** và là tab **đang xem** (active)  
- Extension tự thu nhỏ trang xuống 50% để tối ưu  

### Hai cách chạy

| Tùy chọn | Mô tả |
|---|---|
| **Dự án mới** | Tự mở Whisk, tạo project mới rồi chạy |
| **Tiếp tục trên trang hiện tại** | Chạy ngay trên project đang mở |

### Thiết lập riêng

| Tùy chọn | Chi tiết |
|---|---|
| **Chờ giữa các lần gửi** | Ngẫu nhiên (min–max giây) hoặc cố định (≥10 giây) |
| **Số lần lặp / mô tả** | Mỗi lần Whisk tạo 2 ảnh (VD: 5 mô tả × 3 lần = 30 ảnh) |
| **Bắt đầu từ vị trí** | Nhập số thứ tự để bỏ qua các mô tả phía trước |

### Nhật ký & Xử lý lỗi

- 📋 **Nhật ký thời gian thực** — theo dõi từng bước: chuẩn bị, gửi mô tả, tải ảnh, lỗi…  
- 📝 **Danh sách prompt lỗi** — liệt kê riêng kèm lý do, bấm **"Sao chép"** để copy và thử lại  
- 🔄 **Tự thử lại** khi hàng đợi đầy (tối đa 20 lần + tải lại trang)  
- ⏳ **Tự chờ** khi gặp thông báo lỗi, tiếp tục khi lỗi biến mất  
- 📥 **Quét rà soát cuối** (30 giây) để đảm bảo không bỏ sót ảnh  

---

## 📊 So Sánh Hai Chế Độ

| Tính năng | ⚡ 7.6.0 Nhanh | 🖱️ 7.5.1 Cổ điển |
|---|:---:|:---:|
| Cần mở tab Whisk | ❌ | ✅ Bắt buộc |
| Tốc độ | ⚡ Nhanh | 🐢 Chậm hơn |
| Chạy nền ổn định | ✅ | ⚠️ Cần giữ tab |
| Số ảnh / mô tả | 1–4 tuỳ chọn | Cố định 2 |
| Ảnh tham chiếu | ✅ | ❌ |
| Tên file theo nội dung | ✅ | Theo số thứ tự |
| Chọn tỉ lệ ảnh | 5 tỉ lệ | Mặc định Whisk |
| Mô tả nhiều dòng | ✅ | ❌ |
| Tuỳ chỉnh thời gian chờ | Tự động 2–5s | ✅ Tuỳ chỉnh |
| Lặp mô tả | Dùng số ảnh | ✅ Tuỳ chỉnh |
| Nhật ký chi tiết | Trạng thái vắn tắt | ✅ Đầy đủ |
| Xem ảnh phóng to | ✅ | ❌ |
| Sửa mô tả trong bảng | ✅ | ❌ |

---

## 💡 Mẹo Sử Dụng

- **Tắt "Hỏi vị trí lưu"** trong `chrome://settings/downloads` để tải tự động không bị gián đoạn  
- Tất cả cài đặt được **lưu tự động** — mở lại extension sẽ khôi phục đúng lần cuối  
- Nút 🏠 góc trên trái để quay về **màn hình chọn chế độ** bất cứ lúc nào  

---

<p align="center">
  <b>Designed by <a href="https://duckmartians.info">duckmartians</a></b><br>
  <a href="https://discord.gg/munMZEBMw5">Discord</a> ·
  <a href="https://github.com/duckmartians/Auto-Whisk-Multi-Version">GitHub</a>
</p>
