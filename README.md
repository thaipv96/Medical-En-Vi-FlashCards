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

## 📖 Mục lục

- [Giới thiệu](#-giới-thiệu)
- [Tính năng](#-tính-năng)
- [Ảnh chụp màn hình](#-ảnh-chụp-màn-hình)
- [Bắt đầu nhanh](#-bắt-đầu-nhanh)
- [Hướng dẫn sử dụng](#-hướng-dẫn-sử-dụng)
- [Kiến trúc kỹ thuật](#-kiến-trúc-kỹ-thuật)
- [Bốn TTS Engine](#-bốn-tts-engine)
- [Thuật toán SRS](#-thuật-toán-srs)
- [Phím tắt](#-phím-tắt)
- [Định dạng dữ liệu](#-định-dạng-dữ-liệu)
- [Tương thích trình duyệt](#-tương-thích-trình-duyệt)
- [Giới hạn hiện tại](#-giới-hạn-hiện-tại)
- [Đóng góp](#-đóng-góp)
- [Giấy phép](#-giấy-phép)
- [Ghi công](#-ghi-công)

---

## 🎯 Giới thiệu

**Flashcard Tiếng Anh Y khoa** là một ứng dụng web học tiếng Anh chuyên ngành y khoa, được thiết kế đặc biệt cho các bác sĩ, điều dưỡng và sinh viên y khoa người Việt. Toàn bộ giao diện bằng tiếng Việt, nội dung học bằng tiếng Anh.

### Điểm nổi bật

- 🚀 **Không cần cài đặt** — Một file HTML duy nhất (`index.html`), mở bằng trình duyệt là chạy.
- 🌐 **Sẵn sàng cho GitHub Pages** — Với tên `index.html`, ứng dụng tự động hiển thị tại root URL: `https://<username>.github.io/<repo>/`
- 📴 **Hoạt động offline** — Không cần Internet (trừ các TTS engine cloud tuỳ chọn).
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

### 🎴 Flashcard

- **Tỷ lệ dọc 5:6** — Chiều cao bằng 120% chiều rộng, tối ưu không gian đọc trên mobile.
- **Nội dung căn giữa 2 trục** — Thuật ngữ, IPA, nghĩa, câu ví dụ đều được căn giữa ngang và dọc.
- **Lật thẻ bằng tap** — Nhấn trực tiếp vào Front hoặc Back.
- **Nút TTS riêng** — Góc dưới-phải, không lẫn với nội dung học.
- **Hai mặt hiển thị** — Front (thuật ngữ), Back (nghĩa + ví dụ).

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

Ba nút **luôn hiển thị** ở cả Front và Back:
- **Front:** disabled (chưa xem đáp án)
- **Back:** enabled (đủ điều kiện Review)

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

## 🖼️ Ảnh chụp màn hình

> *Placeholder — vui lòng thêm ảnh chụp màn hình vào thư mục `docs/screenshots/` và cập nhật đường dẫn.*

### Desktop

![Desktop Front](docs/screenshots/desktop-front.png)
*Flashcard ở Front (thuật ngữ) — chế độ sáng*

![Desktop Back](docs/screenshots/desktop-back.png)
*Flashcard ở Back (nghĩa + ví dụ) với 3 nút Review enabled*

### Mobile

<p align="center">
  <img src="docs/screenshots/mobile-front.png" width="250" alt="Mobile Front">
  <img src="docs/screenshots/mobile-back.png" width="250" alt="Mobile Back">
  <img src="docs/screenshots/mobile-dark.png" width="250" alt="Mobile Dark Theme">
</p>

---

## 🚀 Bắt đầu nhanh

### Cách 1: Dùng trực tiếp qua GitHub Pages (nhanh nhất)

Nếu repository đã bật GitHub Pages, truy cập thẳng:

```
https://<username>.github.io/<repo>/
```

Ví dụ: `https://nguyenvana.github.io/medical-english-flashcards/`

> 💡 **Lưu ý:** Vì file chính là `index.html`, GitHub Pages tự động serve nó tại root URL, không cần gõ tên file.

### Cách 2: Tải trực tiếp (dùng offline)

1. **Tải file HTML** về máy:
   - Truy cập repository này → click **Code** → **Download ZIP**
   - Hoặc tải trực tiếp file [`index.html`](index.html)

2. **Mở bằng trình duyệt**:
   - Nhấp đúp vào file `index.html` → trình duyệt mặc định sẽ mở ứng dụng.
   - Hoặc kéo thả file vào cửa sổ Chrome/Firefox/Safari/Edge.

3. **Nạp dữ liệu đầy đủ** (tuỳ chọn):
   - Nhấn nút **Thêm** ở footer → **Nạp dữ liệu đầy đủ**
   - Chọn file `medical_english_vi.json`
   - Ứng dụng sẽ tự parse 2077 bản ghi

### Cách 3: Clone repository

```bash
git clone https://github.com/<username>/medical-english-flashcards.git
cd medical-english-flashcards

# Mở file index.html bằng trình duyệt
open index.html          # macOS
start index.html         # Windows
xdg-open index.html      # Linux
```

### Cách 4: Deploy lên GitHub Pages (cho nhiều người dùng)

1. Fork repository hoặc push code lên nhánh `main`.
2. Vào **Settings** → **Pages**.
3. Source: chọn **Deploy from a branch** → Branch `main` / folder `root`.
4. Truy cập `https://<username>.github.io/<repo>/`.

> 💡 **Ưu điểm của `index.html`:** GitHub Pages sẽ tự động dùng file này làm trang chủ, URL ngắn gọn không cần `/index.html` ở cuối.

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

### Cấu trúc repository

```
medical-english-flashcards/
├── index.html                         ← Ứng dụng chính (single file)
├── medical_english_vi.json            ← Dataset đầy đủ (2077 bản ghi)
├── README.md                          ← File này
├── LICENSE                            ← MIT License
├── .gitignore
├── CHANGELOG.md                       ← (tuỳ chọn)
├── CONTRIBUTING.md                    ← (tuỳ chọn)
├── docs/
│   └── screenshots/
│       ├── desktop-front.png
│       ├── desktop-back.png
│       ├── mobile-front.png
│       ├── mobile-back.png
│       └── mobile-dark.png
└── examples/
    └── progress-sample.json
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

### Phân tách state

```javascript
const state = {
  theme, mode, autoTTS, ttsEngine, cloudFallback,
  voice, rate,
  srs: { [cardKey]: LearningState },     // Persistent
  bookmarks: { [cardKey]: true },        // Persistent
  session: {                             // Ephemeral
    queue, currentIndex, currentCardKey,
    currentFace, visitToken,
    gradedCardKeys, visitedCardKeys
  }
};
```

### Lý do chọn Vanilla JavaScript

- **Zero dependencies** — Không cần npm, không có node_modules.
- **File size nhỏ** — Toàn bộ ứng dụng <100KB (chưa tính dataset).
- **Không build step** — Sửa code, refresh trình duyệt, xong.
- **Offline-first** — Không cần CDN, không phụ thuộc mạng.
- **Dễ audit** — Toàn bộ logic trong 1 file, dễ đọc, dễ kiểm tra bảo mật.

---

## 🎤 Bốn TTS Engine

### So sánh

| Engine | Chi phí | Offline | Chất lượng | Trạng thái |
|---|---|---|---|---|
| **Browser Native TTS** | Miễn phí | ✅ | ⭐⭐⭐ | ✅ Hoạt động ngay |
| **Kokoro Offline Neural** | Miễn phí | ✅ | ⭐⭐⭐⭐⭐ | ⚠️ Cần nhúng model |
| **Google Cloud TTS** | Trả phí | ❌ | ⭐⭐⭐⭐⭐ | ⚠️ Cần OAuth |
| **Microsoft Azure** | Trả phí | ❌ | ⭐⭐⭐⭐⭐ | ⚠️ Cần credentials |

### Thứ tự ưu tiên (chế độ Tự động)

```
1. Browser Native TTS   (nếu có voice tiếng Anh)
   ↓ thất bại
2. Kokoro Offline Neural (nếu đã nhúng model)
   ↓ thất bại
3. Google Cloud TTS      (nếu đã bật consent + có credentials)
   ↓ thất bại
4. Microsoft Azure       (nếu đã bật consent + có credentials)
```

**Quan trọng:** Cloud fallback mặc định **TẮT**. Văn bản không được gửi lên Google/Azure cho đến khi người dùng bật rõ ràng.

### Nội dung được đọc

| Loại thẻ | Front | Back |
|---|---|---|
| Từ vựng / Cụm từ | `term` | `example_en` |
| Cấu trúc câu | `pattern_en` | `example_en` |

**Không đọc:** IPA, tiếng Việt, metadata.

---

## 🧠 Thuật toán SRS

Ứng dụng sử dụng thuật toán lấy cảm hứng từ **SM-2** với ba mức đánh giá.

### Bốn trạng thái

```
New ──→ Learning ──→ Review ──→ Relearning
         ↑              ↓            │
         └──────────────┴────────────┘
```

### Bảng chuyển trạng thái

**New (thẻ mới):**

| Đánh giá | Trạng thái | Thời gian |
|---|---|---|
| Again | Learning step 0 | 10 phút |
| Hard | Learning step 0 | 20 phút |
| Good | Learning step 1 | 1 ngày |

**Learning step 0:**

| Đánh giá | Kết quả |
|---|---|
| Again | Giữ step 0, 10 phút |
| Hard | Giữ step 0, 20 phút |
| Good | Step 1, 1 ngày |

**Learning step 1:**

| Đánh giá | Kết quả |
|---|---|
| Again | Quay về step 0, 10 phút |
| Hard | Giữ step 1, 1.2 ngày |
| Good | **Tốt nghiệp → Review, 3 ngày** |

**Review:**

| Đánh giá | Kết quả |
|---|---|
| Again | Relearning, 10 phút, `lapseCount++` |
| Hard | Interval × 1.2, cập nhật EF |
| Good | Interval × EF mới, cập nhật EF |

**Relearning:**

| Đánh giá | Kết quả |
|---|---|
| Again | 10 phút |
| Hard | 20 phút |
| Good | **Tốt nghiệp → Review, 1 ngày** |

### Ease Factor

Công thức:

```
EF_new = EF_old + (0.1 - (5-q) × (0.08 + (5-q) × 0.02))
```

Trong đó `q` là điểm chất lượng:
- Again → q = 1
- Hard → q = 3
- Good → q = 5

**Giới hạn:** EF ∈ [1.3, 3.0]

### Giới hạn Interval

- **Tối thiểu:** 1 ngày
- **Tối đa:** 365 ngày
- **Làm tròn:** 1 chữ số thập phân

### Hàm thuần (dễ test)

```javascript
calculateNextState(currentState, rating, now)
calculateEaseFactor(currentEaseFactor, quality)
calculateNextInterval(currentInterval, rating, easeFactor)
calculateDueAt(now, interval)
validateLearningState(state)
```

Các hàm này **không** truy cập DOM, localStorage, hay TTS → dễ viết unit test.

---

## ⌨️ Phím tắt

| Phím | Chức năng |
|---|---|
| `←` | Thẻ trước |
| `→` | Thẻ tiếp |
| `Space` | Lật thẻ |
| `Enter` | Lật thẻ (khi card được focus) |
| `B` | Đánh dấu / bỏ đánh dấu |
| `R` | Xáo trộn |
| `Esc` | Dừng TTS / đóng panel |
| `1` | Đánh giá Again |
| `2` | Đánh giá Hard |
| `3` | Đánh giá Good |

> ⚠️ Phím 1/2/3 chỉ hoạt động khi Back đang mở và đủ điều kiện Review.

---

## 📄 Định dạng dữ liệu

Ứng dụng đọc file JSON theo cấu trúc:

```json
{
  "metadata": {
    "title": "Medical English Vocabulary and Sentence Structures",
    "total_word_phrases": 1505,
    "total_sentence_structures": 572
  },
  "word_phrases": [
    {
      "id": "WP000001",
      "term": "present with",
      "part_of_speech": "verb phrase",
      "ipa": {
        "primary": "/ˈprɛz.ənt wɪð/",
        "variety": "General American"
      },
      "meaning_vi": "Đến khám với triệu chứng...",
      "example_en": "The patient presented with chest pain...",
      "example_vi": "Bệnh nhân đến khám vì đau ngực...",
      "category": "History Taking",
      "frequency": "very_common",
      "usage_note_vi": "Thường dùng để mô tả lý do bệnh nhân đến khám..."
    }
  ],
  "sentence_structures": [
    {
      "id": "SS000001",
      "pattern_en": "The patient presents with [symptom].",
      "ipa": { "primary": "/ðə ˈpeɪ.ʃənt ˈprɛz.ənts wɪð/" },
      "meaning_vi": "Bệnh nhân biểu hiện với [triệu chứng].",
      "example_en": "The patient presents with persistent fever...",
      "example_vi": "Bệnh nhân biểu hiện với sốt dai dẳng..."
    }
  ]
}
```

### Trường bắt buộc

**word_phrases:**
- `id` — Định danh duy nhất (VD: `WP000001`)
- `term` — Thuật ngữ tiếng Anh
- `meaning_vi` — Nghĩa tiếng Việt

**sentence_structures:**
- `id` — Định danh duy nhất (VD: `SS000001`)
- `pattern_en` — Pattern câu tiếng Anh
- `meaning_vi` — Nghĩa tiếng Việt

### Trường tuỳ chọn

- `ipa.primary` — Phiên âm IPA
- `part_of_speech` — Từ loại
- `example_en` / `example_vi` — Câu ví dụ
- `usage_note_vi` — Ghi chú cách dùng
- `category`, `frequency`, `source_refs` — Metadata

---

## 🌐 Tương thích trình duyệt

| Trình duyệt | Phiên bản tối thiểu | Ghi chú |
|---|---|---|
| **Chrome** | 90+ | ✅ Đầy đủ tính năng |
| **Edge** | 90+ | ✅ Đầy đủ tính năng |
| **Firefox** | 88+ | ✅ Đầy đủ (một số voice có thể khác) |
| **Safari** | 14+ | ⚠️ Web Speech API có giới hạn voice |
| **Safari iOS** | 14+ | ⚠️ Autoplay TTS cần user interaction |
| **Chrome Android** | 90+ | ✅ Đầy đủ |
| **Samsung Internet** | 15+ | ✅ Đầy đủ |

### Yêu cầu

- **JavaScript:** ES6+ (không transpile)
- **CSS:** `aspect-ratio`, `dvh`, CSS custom properties
- **APIs:** `localStorage`, `SpeechSynthesis` (tuỳ chọn)

### Kiểm thử trên `file://`

Ứng dụng hoạt động khi mở trực tiếp qua `file://`:
- ✅ Hiển thị flashcard
- ✅ Flip, navigation
- ✅ SRS, Review
- ✅ LocalStorage
- ✅ Browser Native TTS
- ⚠️ Kokoro (cần nhúng model thủ công)

---

## ⚠️ Giới hạn hiện tại

### Đã hoạt động đầy đủ

- ✅ 84 bản ghi mẫu (có thể nạp full 2077 qua menu Thêm)
- ✅ Flashcard tỷ lệ 5:6 với nội dung căn giữa
- ✅ Ba nút Review luôn hiển thị
- ✅ SRS đầy đủ bốn trạng thái
- ✅ Browser Native TTS
- ✅ Theme sáng/tối
- ✅ Xuất/nhập tiến độ
- ✅ Keyboard navigation

### Chưa hoạt động đầy đủ

| Tính năng | Trạng thái | Ghi chú |
|---|---|---|
| **Kokoro Offline Neural** | ⚠️ Adapter sẵn sàng | Cần nhúng ~80MB model ONNX + WASM + voice data |
| **Google Cloud TTS** | ⚠️ Adapter sẵn sàng | Cần OAuth 2.0 token hợp lệ |
| **Microsoft Azure** | ⚠️ Adapter sẵn sàng | Cần resource key + region |

### Vì sao Kokoro chưa hoạt động?

Kokoro-82M ONNX cần:
- Model weights (~80 MB)
- Voice data (~10 MB)
- ONNX Runtime Web WASM (~20 MB)
- Tokenizer + G2P phonemizer

Tổng cộng ~110 MB → không thể nhúng vào file `index.html` mặc định. Người dùng cần tự tích hợp theo hướng dẫn trong code hoặc dùng Browser Native TTS.

### Không có kế hoạch hỗ trợ

- ❌ Dashboard thống kê phức tạp (giữ tối giản)
- ❌ Search / Filter nâng cao (không cần thiết cho flashcard)
- ❌ Sync đa thiết bị tự động (dùng export/import thay thế)

---

## 🤝 Đóng góp

Chúng tôi hoan nghênh mọi đóng góp! Dưới đây là cách bạn có thể giúp:

### Báo lỗi

1. Kiểm tra [Issues](../../issues) xem lỗi đã được báo chưa.
2. Nếu chưa, tạo [Issue mới](../../issues/new) với:
   - Trình duyệt + phiên bản
   - Hệ điều hành
   - Các bước tái hiện
   - Screenshot nếu có

### Đề xuất tính năng

- Tạo Issue với label `enhancement`.
- Mô tả rõ use case và lợi ích.

### Gửi Pull Request

```bash
# 1. Fork repository
# 2. Clone fork của bạn
git clone https://github.com/<your-username>/medical-english-flashcards.git
cd medical-english-flashcards

# 3. Tạo branch mới
git checkout -b feature/ten-tinh-nang

# 4. Sửa file index.html
# 5. Test kỹ trên Chrome + Firefox + mobile
# 6. Commit với message rõ ràng
git commit -m "feat: thêm tính năng X"

# 7. Push lên fork
git push origin feature/ten-tinh-nang

# 8. Tạo Pull Request
```

### Quy ước code

- **Vanilla JS** — Không thêm framework/dependency.
- **Single file** — Toàn bộ code trong `index.html`.
- **Comment rõ ràng** — Giải thích logic phức tạp.
- **Không phá vỡ tính năng hiện có** — Test kỹ trước khi PR.
- **Tuân thủ spec** — Flashcard phải là 5:6, 3 nút Review luôn hiện, v.v.

### Kiểm tra trước khi gửi PR

- [ ] Mở được qua `file://` (không cần server).
- [ ] Flashcard tỷ lệ 5:6 (`height/width ≈ 1.2`).
- [ ] Ba nút Review luôn hiển thị.
- [ ] Flip không đổi kích thước card.
- [ ] SRS bảng chuyển trạng thái đúng.
- [ ] Không có lỗi console.
- [ ] Test trên Chrome, Firefox, mobile (nếu có thể).

---

## 📜 Giấy phép

Dự án này được phát hành dưới giấy phép **MIT License**.

```
MIT License

Copyright (c) 2026 <Your Name>

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
```

Xem file [LICENSE](LICENSE) để biết chi tiết.

---

## 🙏 Ghi công

### Nguồn tham khảo từ vựng

Dữ liệu được biên soạn dựa trên các nguồn uy tín:

- [Cambridge Dictionary](https://dictionary.cambridge.org)
- [Oxford Learner's Dictionaries](https://www.oxfordlearnersdictionaries.com)
- [Merriam-Webster](https://www.merriam-webster.com)
- [MSD Manuals](https://www.msdmanuals.com)
- [MedlinePlus](https://medlineplus.gov)
- [NICE Guidelines](https://www.nice.org.uk)
- [PubMed](https://pubmed.ncbi.nlm.nih.gov)

### Công nghệ sử dụng

- [Web Speech API](https://developer.mozilla.org/en-US/docs/Web/API/Web_Speech_API) — Browser Native TTS
- [Kokoro-82M](https://huggingface.co/hexgrad/Kokoro-82M) — Neural TTS (planned integration)
- [ONNX Runtime Web](https://onnxruntime.ai/) — Inference engine (planned)
- [Lucide Icons](https://lucide.dev/) — SVG icon inspiration

### Cảm ơn

- Cộng đồng bác sĩ Việt Nam đã đóng góp ý kiến cho bộ từ vựng.
- Các tác giả của SM-2 algorithm (Piotr Woźniak) cho nền tảng SRS.
- Cộng đồng open source đã chia sẻ kiến thức về Web Speech API và Neural TTS.

---

## 📧 Liên hệ

- **Issues:** [GitHub Issues](../../issues)
- **Discussions:** [GitHub Discussions](../../discussions)
- **Email:** *(cập nhật email của bạn)*

---

<div align="center">

**⭐ Nếu dự án hữu ích, hãy tặng một star để ủng hộ!**

Made with ❤️ for Vietnamese medical professionals

</div>
