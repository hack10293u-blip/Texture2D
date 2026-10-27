# Texture2D 1.6

Liên hệ: https://t.me/ttt_cth

## Kích hoạt offline theo mã máy

1. Mở Texture2D-1.6.exe. Sao chép mã máy TTTM-… trên màn hình kích hoạt.
2. Bấm Liên hệ Telegram và gửi mã máy cho người cấp key.
3. Nhận key dạng TTT_XXXXX và file giấy phép .lic đi kèm.
4. Nhập key, bấm Chọn file .lic rồi KÍCH HOẠT VĨNH VIỄN.

Key không hết hạn. App kiểm tra chữ ký số và mã máy ngay trên máy, không cần Internet để kích hoạt hay sử dụng. Chỉ nút Telegram cần mạng để mở liên hệ. Chép cả key lẫn file .lic sang máy khác sẽ không kích hoạt được.

Key ngắn là mã nhận diện; file .lic chứa chữ ký và mã máy, nên cần nhận cả hai. Không thể dùng key ngắn riêng lẻ. App ghi nhớ giấy phép trong %LOCALAPPDATA%/Texture2DNeon/activation-machine.lic; không dùng JSON. Key TX2D-… của bản cũ không dùng cho bản gắn mã máy này.

Mã máy dựa trên Windows MachineGuid. Cài lại Windows hoặc thay đổi định danh Windows có thể cần cấp giấy phép mới. Giấy phép gắn với định danh cài đặt Windows, không phải cơ chế quản lý thiết bị qua máy chủ.

## Tạo bundle

Chọn bundle gốc → chọn 1/nhiều ảnh hoặc thư mục → chọn texture → TẠO BUNDLE.

    Ketqua/
      tên ảnh/
        scene_artist_autochess_01.assetbundle
        preview.png

Giữ bundle tên gốc, mỗi ảnh một thư mục; trùng tên thì thêm _2, _3… Không tạo bao-cao.json hay thong-tin.json. Nút Sáng/Tối ghi nhớ lựa chọn trong theme.txt. Nút Telegram ở góc trên mở t.me/ttt_cth.

Ảnh tự resize về kích thước texture nếu bật tùy chọn. Preview là ảnh texture thu nhỏ, không phải ảnh chụp trong game. App đọc lại bundle vừa lưu để kiểm tra pixel ảnh thay thế. Đã kiểm tra với bundle mẫu trong 1.zip, chưa thử nạp vào game.

## Bản 1.6
Tên cửa sổ: Texture2D • 1.6. Icon dùng nguyên ảnh vuông 1:1 được cung cấp, xuất các cỡ 16, 24, 32, 48, 64, 128 và 256 px.
Bản EXE có mã nhận diện bản dựng và dấu kiểm tra toàn vẹn SHA-256 được ký Ed25519. App kiểm tra khi khởi động và trước tác vụ. Giấy phép được kiểm tra lại ngay tại phần đọc bundle và trước mỗi ảnh. Bản sửa đổi hoặc giấy phép sai sẽ bị từ chối khi các kiểm tra phát hiện.
Các key và file .lic cấp bằng công cụ bản 1.5 vẫn dùng được; không cần cấp lại. Không thêm dịch vụ mạng hoặc ngày hết hạn.
Đây là lớp bảo vệ offline và phát hiện sửa đổi, không phải bảo đảm chống dịch ngược/crack tuyệt đối. Dấu ký nội bộ này không phải chứng chỉ Authenticode của Windows.

