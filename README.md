# Texture2D

**Texture2D 1.6 · Windows x64 · Desiger by TTT**

[![Phiên bản](https://img.shields.io/badge/version-1.6-9b42ec)](https://github.com/hack10293u-blip/Texture2D/releases/tag/1.6)
[![Windows](https://img.shields.io/badge/Windows-x64-19badb)](https://github.com/hack10293u-blip/Texture2D/releases/latest)
[![Telegram](https://img.shields.io/badge/Telegram-ttt__cth-26A5E4)](https://t.me/ttt_cth)

Ứng dụng tạo nhiều Unity AssetBundle từ một bundle gốc và nhiều ảnh thay thế.

## Tải xuống

- [Tải EXE 1.6](https://github.com/hack10293u-blip/Texture2D/releases/download/1.6/Texture2D-1.6.exe)
- [Tải ZIP kèm hướng dẫn](https://github.com/hack10293u-blip/Texture2D/releases/download/1.6/Texture2D-1.6-Windows.zip)
- [Xem tất cả phiên bản](https://github.com/hack10293u-blip/Texture2D/releases)

Chạy trực tiếp trên Windows x64, không cần cài Python. Khi dùng ZIP, giải nén rồi mở EXE.

## Tính năng

- Một ảnh, nhiều ảnh hoặc cả thư mục ảnh; mỗi ảnh tạo một bundle riêng.
- Chọn texture cần thay, tùy chọn resize về kích thước texture gốc.
- Ảnh xem trước đi kèm từng bundle để dễ nhận diện.
- Giao diện neon tím–hồng–cyan và chế độ sáng; nhớ lựa chọn.
- Kích hoạt offline vĩnh viễn theo mã máy, dùng key `TTT_XXXXX` và giấy phép `.lic`.
- Kiểm tra chữ ký bản dựng và giấy phép tại các bước xử lý.

## Kích hoạt

1. Mở app và sao chép mã máy `TTTM-…`.
2. [Liên hệ t.me/ttt_cth](https://t.me/ttt_cth), gửi mã máy để được cấp key và file `.lic`.
3. Nhập key, chọn file `.lic`, bấm **KÍCH HOẠT VĨNH VIỄN**.

App xác minh giấy phép ngay trên máy, không cần máy chủ. Key và file `.lic` phải được cấp cho đúng mã máy. Cài lại Windows có thể cần cấp lại giấy phép. Giấy phép bản 1.5 vẫn tương thích.

## Sử dụng

**Chọn bundle gốc → chọn ảnh → chọn texture → TẠO BUNDLE.**

```text
Ketqua/
  tên ảnh/
    scene_artist_autochess_01.assetbundle
    preview.png
```

Bundle gốc được giữ nguyên. Tên thư mục trùng sẽ thêm `_2`, `_3`… Không tạo JSON kết quả. PNG xem trước là ảnh texture, không phải ảnh chụp trong game.

Texture mới dùng RGBA32 và bundle nén LZ4 theo script gốc, nên dung lượng có thể lớn hơn. Đã kiểm tra bằng bundle mẫu và đọc lại ảnh thay thế; chưa kiểm chứng nạp vào game. Cơ chế offline giúp phát hiện sửa đổi, không bảo đảm chống crack tuyệt đối.

## Liên hệ

[Telegram · t.me/ttt_cth](https://t.me/ttt_cth)

Repository này chỉ phân phối bản ứng dụng cho người dùng và tài liệu hướng dẫn.
