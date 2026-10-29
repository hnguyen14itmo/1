# Slovo Lab — Học từ vựng tiếng Nga–Việt 🇷🇺🇻🇳

Ứng dụng web tĩnh giúp học từ vựng bằng flashcard, nghe phát âm tiếng Nga, trắc nghiệm, lịch ôn và thống kê.

## Mở website

Sau khi bật GitHub Pages:
**https://hnguyen14itmo.github.io/1/**

Để bật Pages lần đầu:

1. Vào [Settings → Pages](https://github.com/hnguyen14itmo/1/settings/pages).
2. Tại **Build and deployment → Source**, chọn **Deploy from a branch**.
3. Tại **Branch**, chọn **main** và thư mục **/(root)**, sau đó bấm **Save**.
4. Vào địa chỉ website ở trên để sử dụng (thời gian xuất bản phụ thuộc GitHub).

Trang có thể dùng trên điện thoại và máy tính.

## Cập nhật danh sách từ qua ChatGPT

Tệp `vocabulary.json` chứa danh sách từ được website tải lại khi mở.

Mỗi từ có định dạng:

```json
{
  "ru": "безопасность",
  "vi": "bảo mật",
  "example": "Информационная безопасность очень важна.",
  "topic": "Bảo mật"
}
```

- Đặt từ mới trong mảng `words` của `vocabulary.json`.
- Mỗi khi cập nhật tệp lên nhánh `main`, website sẽ tải nội dung mới khi mở hoặc khi bấm nút làm mới.
- Những từ trùng tiếng Nga được cập nhật nghĩa/ví dụ, không xóa lịch sử ôn của từ đó.
- Để xóa các thẻ mẫu ở những trình duyệt đã dùng trước đây, nên thao tác trong giao diện hoặc thay đổi cơ chế đồng bộ theo nhu cầu.

## Lưu tiến độ

- Lịch sử học nằm trong bộ nhớ `localStorage` của **trình duyệt đang sử dụng**; không tự đồng bộ giữa các thiết bị.
- Xuất sao lưu JSON ở phần **Cài đặt** trước khi xóa dữ liệu trình duyệt hoặc đổi máy.
- Phát âm tiếng Nga dùng giọng đọc có trên thiết bị; nếu không có giọng Nga thì có thể không phát âm chuẩn.
- Từ vựng trong GitHub repository công khai cũng là dữ liệu công khai. Không ghi thông tin cá nhân hay mật khẩu vào danh sách từ.

## Nguồn

- `index.html`: toàn bộ giao diện và logic app, không cần cài thư viện.
- `vocabulary.json`: danh sách từ từ xa, dễ cập nhật trong các lần sau.
- `README.md`: hướng dẫn này.
