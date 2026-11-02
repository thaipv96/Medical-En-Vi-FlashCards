<div align="center">

# 🩺 Medical Flashcards

### *Học từ vựng y khoa thông minh — Lật thẻ, nghe phát âm, nhớ lâu hơn*

[![Made with HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![License: MIT](https://img.shields.io/badge/License-MIT-22c55e?style=for-the-badge)](LICENSE)
[![Single File](https://img.shields.io/badge/Single%20File-100%25-7c3aed?style=for-the-badge)](.)

**⚡ Không cần cài đặt · Không cần build · Không cần server — chỉ cần mở file HTML là chạy!**

[🚀 Xem Demo](#-demo) · [✨ Tính năng](#-tính-năng-nổi-bật) · [🛠 Cài đặt](#-cài-đặt--sử-dụng) · [🤝 Đóng góp](#-đóng-góp)

</div>

---

## 🌟 Giới thiệu

**Medical Flashcards** là một ứng dụng web học từ vựng y khoa dưới dạng **flashcard tương tác**, được thiết kế đặc biệt cho sinh viên y khoa, điều dưỡng, dược sĩ và bất kỳ ai muốn chinh phục "biển" thuật ngữ y khoa tiếng Anh.

Với hơn **1.000+ thuật ngữ y khoa** được biên soạn kỹ lưỡng, mỗi thẻ bao gồm:

| Thành phần | Mô tả |
|------------|-------|
| 🔤 **Từ mới** | Thuật ngữ y khoa tiếng Anh |
| 🗣 **Phiên âm IPA** | Chuẩn quốc tế, giúp phát âm chính xác |
| 🏷 **Từ loại** | Danh từ / Động từ / Tính từ / Trạng từ |
| 🇻🇳 **Nghĩa tiếng Việt** | Giải thích rõ ràng, dễ hiểu |
| 📝 **Câu ví dụ** | Ngữ cảnh thực tế trong y khoa |
| 💬 **Dịch câu ví dụ** | Hiểu sâu, nhớ lâu |

> 💡 *"Học từ vựng không khó — chỉ là bạn chưa tìm được công cụ đúng!"*

---

## 🎬 Demo

<div align="center">

> 🖼 **Screenshot** *(khi upload lên GitHub, hãy thêm ảnh demo vào thư mục `/screenshots` và thay link bên dưới)*

</div>

---

## ✨ Tính năng nổi bật

### 🎯 Trải nghiệm học tập
- ✅ **1.000+ thuật ngữ y khoa** phủ rộng từ giải phẫu, sinh lý, bệnh học đến dược lý
- ✅ **Thẻ lật 3D** mượt mà với hiệu ứng `perspective` và `preserve-3d`
- ✅ **Điều hướng linh hoạt**: Chuột, phím tắt, hoặc vuốt màn hình cảm ứng
- ✅ **Thanh tiến trình** trực quan — theo dõi tiến độ học mỗi ngày
- ✅ **Xáo trộn ngẫu nhiên** — tránh học vẹt theo thứ tự
- ✅ **Khôi phục ban đầu** — quay về danh sách gốc bất cứ lúc nào

### 🔊 Text-to-Speech (TTS) — Điểm nhấn đặc biệt
- 🎙 **3 lớp TTS dự phòng** đảm bảo luôn hoạt động:
  1. **Puter.js** *(online, không cần API key)* — giọng đọc chất lượng cao
  2. **Google Translate TTS** — fallback ổn định
  3. **Web Speech API** — fallback offline hoàn toàn miễn phí
- 🔊 **Nút đọc thủ công** trên từng thẻ
- ⚡ **Tự động đọc** khi mở thẻ mới hoặc lật sang mặt nghĩa
- 🎛 **Bật/tắt tự động đọc** dễ dàng

### 📱 Responsive & Tối ưu
- 💻 **Desktop**: Hiệu ứng hover 3D tinh tế
- 📱 **Mobile**: Vuốt trái/phải để chuyển thẻ
- 📟 **Tablet**: Layout co giãn thông minh với `clamp()`
- 🎨 **UI hiện đại**: Gradient, glassmorphism, micro-animations

### ⌨️ Phím tắt tiện lợi
| Phím | Chức năng |
|------|-----------|
| `Space` / `Enter` | Lật thẻ |
| `←` Arrow Left | Thẻ trước |
| `→` Arrow Right | Thẻ sau |

---

## 🛠 Cài đặt & Sử dụng

### 🚀 Cách 1: Sử dụng trực tiếp (Khuyến nghị)

```bash
# Clone repo về máy
git clone https://github.com/your-username/medical-flashcards.git

# Mở file HTML trong trình duyệt
cd medical-flashcards
open index.html   # macOS
# hoặc
start index.html  # Windows
# hoặc
xdg-open index.html  # Linux

