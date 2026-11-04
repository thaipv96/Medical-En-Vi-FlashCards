# 🩺 Flashcard Tiếng Anh Y khoa

> Ứng dụng flashcard học từ vựng, cụm từ và cấu trúc câu tiếng Anh y khoa dành cho bác sĩ Việt Nam — chạy hoàn toàn offline, không cần cài đặt, không cần đăng ký.

[![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat-square&logo=html5&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/HTML)
[![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=flat-square&logo=css3&logoColor=white)](https://developer.mozilla.org/en-US/docs/Web/CSS)
[![JavaScript ES6+](https://img.shields.io/badge/JavaScript-ES6+-F7DF1E?style=flat-square&logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![No Dependencies](https://img.shields.io/badge/dependencies-0-success?style=flat-square)](#)
[![Single File](https://img.shields.io/badge/single--file-yes-blue?style=flat-square)](#)
[![Offline Ready](https://img.shields.io/badge/offline-ready-brightgreen?style=flat-square)](#)
[![License: MIT](https://img.shields.io/badge/License-MIT-yellow?style=flat-square)](LICENSE)

---

## 🎯 Giới thiệu

**Flashcard Tiếng Anh Y khoa** là một ứng dụng web học tiếng Anh chuyên ngành y khoa, được thiết kế đặc biệt cho các bác sĩ, điều dưỡng và sinh viên y khoa người Việt. Toàn bộ giao diện bằng tiếng Việt, nội dung học bằng tiếng Anh.

### Điểm nổi bật

- 🚀 **Không cần cài đặt** — Mở một file HTML duy nhất (`index.html`) hoặc truy cập liên kết bằng trình duyệt là chạy.
- 🌐 **GitHub Pages** — Ứng dụng tự động hiển thị tại root URL: `https://thaipv96.github.io/Medical-En-Vi-FlashCards/`
- 🎨 **Thiết kế tối ưu mobile** — Thao tác một tay, hỗ trợ cử chỉ vuốt.
- 🧠 **SRS thông minh** — Lặp lại ngắt quãng, tối ưu thời gian ôn tập.
- 🎤 **Bốn TTS engine** — Từ Browser Native (offline) đến Neural TTS chất lượng cao.
- 💾 **Lưu tiến độ tự động** — Xuất/nhập để sao lưu hoặc chuyển thiết bị.
- 🎯 **Dữ liệu thực** — 2077 bản ghi từ vựng và cấu trúc câu y khoa được biên soạn kỹ lưỡng.

### Đối tượng sử dụng

- 🩺 Bác sĩ lâm sàng cần trau dồi thuật ngữ tiếng Anh trong thực hành.
- 📚 Sinh viên y khoa chuẩn bị cho các kỳ thi quốc tế (USMLE, PLAB, MRCP…).
- 🏥 Nhân viên y tế tham gia hội thảo, viết bài báo khoa học quốc tế.
- 🎓 Giảng viên y khoa cần tài liệu học tập tương tác.

---

## ✨ Tính năng

### 📊 Ba chế độ học

1. **Tất cả thẻ** — Toàn bộ 2077 bản ghi.
2. **Từ vựng và cụm từ** — 1505 từ/cụm từ y khoa.
3. **Cấu trúc câu** — 572 pattern câu thực hành.

### 🎯 Ba nút Review luôn hiển thị

| Nút | Nhãn tiếng Anh | Ý nghĩa |
|---|---|---|
| 🔴 Chưa nhớ | Again | Không nhớ — quay lại học |
| 🟡 Khó | Hard | Nhớ nhưng khó khăn |
| 🟢 Nhớ tốt | Good | Nhớ tốt — tăng khoảng cách ôn tập |

### 🔁 Điều hướng linh hoạt

- **Chuột** — Click nút Previous/Next/Flip/Shuffle.
- **Bàn phím** — Mũi tên trái/phải, Space, Enter, phím tắt 1/2/3.
- **Cảm ứng** — Vuốt ngang để chuyển thẻ, vuốt không kích hoạt lật thẻ.

### 🎤 Bốn TTS Engine

- **Browser Native TTS** — Miễn phí, hoạt động offline, chất lượng phụ thuộc hệ điều hành.
- **Kokoro Offline Neural** — Neural TTS chất lượng cao, chạy hoàn toàn offline (khi được nhúng model).
- **Google Cloud TTS** — Giọng đọc Neural chất lượng cao, cần OAuth và kết nối Internet.
- **Microsoft Azure AI Speech** — Tương tự Google, có nhiều tuỳ chọn giọng đọc Neural.

### 💾 Lưu trữ tiến độ

- Tự động lưu tiến độ SRS sau mỗi lần Review.
- Lưu bookmark, cài đặt TTS, theme.
- **Xuất/nhập tiến độ** — Sao lưu hoặc chuyển giữa các thiết bị dưới dạng JSON.
- **Không lưu credentials** — API key Google/Azure chỉ tồn tại trong RAM.

### 🎨 Theme sáng/tối

- Chuyển đổi một chạm.
- Tự động lưu lựa chọn.
- Màu sắc tương phản cao, đạt chuẩn WCAG AA.

### ♿ Accessibility

- Semantic HTML, ARIA roles.
- Keyboard navigation đầy đủ.
- Screen reader compatible.
- `prefers-reduced-motion` support.
- Progress bar có `role="progressbar"` và ARIA values.

---

## 🚀 Bắt đầu nhanh

### Cách 1: Dùng trực tiếp qua GitHub Pages (nhanh nhất)

Truy cập trực tiếp:

```
https://thaipv96.github.io/Medical-En-Vi-FlashCards/
```

### Cách 2: Tải trực tiếp (dùng offline)

1. **Tải file HTML** về máy:
   - Truy cập repository này → click **Code** → **Download ZIP**
   - Hoặc tải trực tiếp file [`index.html`](index.html)

2. **Mở bằng trình duyệt**:
   - Nhấp đúp vào file `index.html` → trình duyệt mặc định sẽ mở ứng dụng.
   - Hoặc kéo thả file vào cửa sổ Chrome/Firefox/Safari/Edge.

### Cách 3: Clone repository

```bash
git clone https://github.com/<username>/medical-english-flashcards.git
cd medical-english-flashcards

# Mở file index.html bằng trình duyệt
open index.html          # macOS
start index.html         # Windows
xdg-open index.html      # Linux
```

---

## 📚 Hướng dẫn sử dụng

### Học một thẻ

1. **Đọc Front** — Thuật ngữ, IPA, từ loại.
2. **Đoán nghĩa** — Cố nhớ nghĩa tiếng Việt trước khi lật.
3. **Lật thẻ** — Tap vào thẻ hoặc nhấn phím Space.
4. **Đọc Back** — Nghĩa, câu ví dụ tiếng Anh, bản dịch, ghi chú.
5. **Đánh giá** — Chọn một trong ba nút Review:
   - **Chưa nhớ** — Sẽ gặp lại sau 10 phút (hoặc 20 phút nếu Hard).
   - **Khó** — Lặp lại với khoảng cách tăng nhẹ.
   - **Nhớ tốt** — Tăng khoảng cách ôn tập theo Ease Factor.
6. **Chuyển thẻ** — Tự động hoặc nhấn Next.

### Điều hướng

| Thao tác | Kết quả |
|---|---|
| Tap card | Lật thẻ |
| Swipe trái | Thẻ tiếp theo |
| Swipe phải | Thẻ trước |
| ← / → | Thẻ trước / tiếp |
| Space | Lật thẻ |
| 1 / 2 / 3 | Đánh giá Again / Hard / Good |
| B | Bookmark |
| R | Shuffle |
| Esc | Dừng TTS / đóng panel |

### Cài đặt TTS

1. Nhấn nút **Giọng đọc** ở footer.
2. Chọn engine:
   - **Tự động** — Thử Browser → Kokoro → Cloud theo thứ tự.
   - **Browser Native TTS** — Miễn phí, offline (khuyến nghị bắt đầu).
   - **Kokoro Offline Neural** — Cần model (~80MB) được nhúng riêng.
   - **Google Cloud TTS / Microsoft Azure** — Cần credentials.
3. Chọn giọng đọc (voice) và tốc độ (rate).
4. Nếu dùng cloud → bật **Cho phép cloud fallback** (mặc định TẮT).

### Xuất/nhập tiến độ

**Xuất:**
- Nhấn **Thêm** → **Xuất tiến độ học**
- File `medical_flashcards_progress_<timestamp>.json` được tải về.

**Nhập:**
- Nhấn **Thêm** → **Nhập tiến độ học**
- Chọn file JSON đã xuất trước đó.
- **Lưu ý:** Việc nhập sẽ ghi đè lên tiến độ hiện tại (có xác nhận).

---

## 🏗️ Kiến trúc kỹ thuật

### Nguyên tắc thiết kế

```
┌─────────────────────────────────────────┐
│      index.html (Single File)           │
│  ┌───────────────────────────────────┐  │
│  │  HTML (semantic + ARIA)           │  │
│  ├───────────────────────────────────┤  │
│  │  CSS (custom properties, theme)   │  │
│  ├───────────────────────────────────┤  │
│  │  JavaScript (Vanilla ES6+)        │  │
│  │  ┌─────────────────────────────┐  │  │
│  │  │  SRSManager (pure functions)│  │  │
│  │  │  TTSEngineManager           │  │  │
│  │  │  StorageManager             │  │  │
│  │  │  UIController               │  │  │
│  │  └─────────────────────────────┘  │  │
│  ├───────────────────────────────────┤  │
│  │  Dataset JSON (embedded/loaded)   │  │
│  └───────────────────────────────────┘  │
└─────────────────────────────────────────┘
```

### Các module chính

| Module | Trách nhiệm |
|---|---|
| **SessionManager** | Quản lý queue, currentIndex, visitToken |
| **SRSManager** | Tính toán trạng thái SRS (pure functions, không phụ thuộc DOM) |
| **ProgressManager** | Cập nhật thanh tiến độ theo visitedCardKeys |
| **TTSEngineManager** | Điều phối 4 engine TTS theo thứ tự ưu tiên |
| **TTSPlaybackManager** | Ngăn chặn phát chồng, quản lý request ID |
| **StorageManager** | Lưu/khôi phục từ localStorage |
| **BookmarkManager** | Quản lý đánh dấu thẻ |
| **ThemeManager** | Sáng/tối |
| **UIController** | Render, cập nhật DOM |
---

## 🎤 Bốn TTS Engine

| Engine | Chi phí | Offline | Chất lượng | Trạng thái |
|---|---|---|---|---|
| **Browser Native TTS** | Miễn phí | ✅ | ⭐⭐⭐ | ✅ Hoạt động ngay |
| **Kokoro Offline Neural** | Miễn phí | ✅ | ⭐⭐⭐⭐⭐ | ⚠️ Cần nhúng model |
| **Google Cloud TTS** | Trả phí | ❌ | ⭐⭐⭐⭐⭐ | ⚠️ Cần OAuth |
| **Microsoft Azure** | Trả phí | ❌ | ⭐⭐⭐⭐⭐ | ⚠️ Cần credentials |
---

### Nguồn tham khảo từ vựng
Dữ liệu được biên soạn dựa trên các nguồn uy tín:
- [Cambridge Dictionary](https://dictionary.cambridge.org)
- [Oxford Learner's Dictionaries](https://www.oxfordlearnersdictionaries.com)
- [Merriam-Webster](https://www.merriam-webster.com)
- [MSD Manuals](https://www.msdmanuals.com)
- [MedlinePlus](https://medlineplus.gov)
- [NICE Guidelines](https://www.nice.org.uk)
- [PubMed](https://pubmed.ncbi.nlm.nih.gov)
---

## 📧 Liên hệ
**Email:** *thaipv96@gmail.com*
---
