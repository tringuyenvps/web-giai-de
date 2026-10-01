# MY EXAM — bản đã sửa

## 1. Nguồn câu hỏi
App dùng **manifest.json bắt buộc**. Không còn probe `de1.json ... de20.json` và không có câu demo/fallback.

Mỗi thư mục môn có dạng:

```text
database/
  vsat/
    toan/
      manifest.json
      de1.json
      de2.json
      assets/
```

Manifest tối thiểu:

```json
{
  "version": 1,
  "exam": "vsat",
  "subject": "toan",
  "files": ["de1.json", "de2.json"]
}
```

## 2. Thời gian
- Toán: 90 phút
- Ngữ văn (`ngu_van`): 90 phút
- Các môn khác: 50 phút

Thời gian được lấy **theo mã môn**, không lấy từ `de*.json`, nên không thể bị nhân nhầm thành hàng giờ.

## 3. VSAT Toán hiện tại
Đề mẫu `de2.json` có đúng 25 câu: 9 Đúng/Sai + 6 MCQ + 5 Ghép hợp + 5 Trả lời ngắn = 150 điểm.

## 4. Chạy app
Dùng Live Server hoặc một local HTTP server. Mở `index.html` trực tiếp bằng `file://` có thể làm `fetch()` bị chặn.
