# Slovo Lab — Học từ vựng Nga–Việt 🇷🇺🇻🇳

Ứng dụng flashcard tiếng Nga có giao diện tiếng Việt, trắc nghiệm, phát âm, lịch ôn tập và thống kê tiến độ.

## Bộ từ vựng

Hiện có **254 thẻ**, bao gồm bộ từ mẫu cũ và từ vựng tổng hợp từ 4 tài liệu học:

1. `незнакомые слова.docx` — 68 mục về Kamchatka.
2. `Путешествие. Лексика.docx` — từ về du lịch và chuyến tham quan.
3. `08.10. Резюме_повтор конструкций_приложение реплика.pptx` — chủ đề nghề nghiệp IT và ứng dụng Replika.
4. `13.10. Резюме_характеристика процесса_глаголы физики.pptx` — động từ vật lý và mô tả quá trình.

Một số từ trùng từ hai tài liệu được gộp lại. Bộ từ có thêm các thuật ngữ liên quan trực tiếp trong bài học, không chỉ từ danh sách riêng.

**Thẻ được thiết kế theo dạng:** từ tiếng Nga → nghĩa tiếng Việt → **giải thích ngắn bằng tiếng Nga mức B1**. Không còn câu ví dụ thay cho giải thích.

Ví dụ:

```json
{
  "ru": "долина",
  "vi": "thung lũng",
  "definition": "Низкое место между горами или холмами.",
  "topic": "Du lịch · Kamchatka"
}
```

## Chạy trên web

- Repository: https://github.com/hnguyen14itmo/1
- GitHub Pages (nếu đã bật): https://hnguyen14itmo.github.io/1/

Nếu Pages chưa hoạt động: trong repository mở **Settings → Pages**, chọn **Deploy from a branch → main → /(root)** và lưu.

## Thêm từ cùng ChatGPT

- Gửi danh sách từ mới trong cuộc trò chuyện.
- ChatGPT có thể cập nhật `vocabulary.json` trong repository được cấp quyền.
- Website sẽ tải bộ từ mới khi bạn mở lại trang, hoặc bấm **↻** để đồng bộ.
- Từ trùng sẽ được cập nhật giải thích, không làm mất tiến độ ôn.

Mỗi mục từ có 4 trường chính: `ru` (Nga), `vi` (Việt), `definition` (giải thích tiếng Nga), `topic` (chủ đề). Các tệp cũ có trường `example` vẫn được ứng dụng đọc tương thích để giữ dữ liệu.

## Lưu ý

- Tiến độ được lưu vào localStorage của từng trình duyệt, **không tự đồng bộ giữa các thiết bị**.
- Trong **Cài đặt**, hãy tải bản sao lưu JSON nếu muốn chuyển thiết bị hoặc tránh mất dữ liệu.
- Giọng đọc tiếng Nga phụ thuộc vào giọng đọc được cài trên trình duyệt / thiết bị.
- Repository và từ vựng công khai; không đưa mật khẩu, dữ liệu riêng tư vào `vocabulary.json`.
- Trong tài liệu gốc có một số lỗi chính tả như `касатка`; thẻ dùng cách viết chuẩn `косатка`.
