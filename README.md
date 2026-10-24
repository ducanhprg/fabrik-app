# Spotter

*[English](README.en.md)*

Spotter theo dõi máy in 3D trong mạng nhà bạn: trạng thái và camera trực tiếp trên một trang web,
gửi thông báo kèm ảnh qua Telegram (hoặc email) khi bản in bắt đầu, in xong, bị lỗi hoặc bị kẹt,
và cho phép điều khiển (tạm dừng, tiếp tục, hủy, nhiệt độ, đèn). Mọi thứ chạy trên máy tính của bạn,
không qua dịch vụ đám mây nào.

Dùng được với **Snapmaker U1** và các máy **Klipper / Moonraker** khác, và máy **Bambu Lab** ở chế độ LAN.
Hiện chỉ chạy trên Windows. Giao diện mặc định là tiếng Việt (nút **English** ở góc trên bên phải để đổi).

## Cài đặt

1. Tải **`Spotter-<phiên bản>-windows.zip`** ở bản mới nhất trong mục [Releases](../../releases/latest),
   rồi giải nén vào một thư mục riêng (ví dụ `Documents\Spotter`). Đừng để trong Program Files:
   Spotter tự cập nhật ngay trong thư mục của nó.
2. Nhấp đúp **`spotter.exe`**. Nếu Windows báo "Windows protected your PC", bấm
   **More info → Run anyway**. Khi tường lửa hỏi, hãy cho phép nếu bạn muốn mở trang Spotter từ điện thoại.
3. Trang Spotter tự mở trong trình duyệt (<http://localhost:8484>). Giữ cửa sổ màu đen mở:
   đóng nó là Spotter dừng.
4. Bấm **Quét mạng** và thêm máy in của bạn.
   - **Bambu Lab:** bật chế độ **LAN only** và **developer mode** trên máy in, rồi nhập **mã truy cập**
     (access code, xem trong phần cài đặt mạng trên màn hình máy in) khi thêm máy. Giữ `ffmpeg.exe` cạnh
     `spotter.exe`: camera của Bambu cần nó.

Cài đặt được lưu trong thư mục `data` cạnh `spotter.exe` (trong đó có token Telegram và mã truy cập máy in:
đừng chia sẻ thư mục này).

## Thông báo qua Telegram

Bấm **Cài đặt Telegram** trên thanh ở đầu trang (hoặc nút **Thông báo**) và làm theo bốn bước:

1. **Tạo bot:** trong Telegram, nhắn cho [@BotFather](https://t.me/BotFather), gửi `/newbot`, đặt tên cho bot,
   rồi dán token mà nó gửi cho bạn. Spotter hiện tên bot khi token đúng.
2. **Chọn nơi nhận thông báo:** chỉ mình bạn, một nhóm (gia đình hoặc bạn bè cùng in), hoặc một kênh.
   **Mở Telegram** đưa bạn đến đúng chỗ: bấm Start trong bot, hoặc chọn nhóm hay kênh để thêm bot vào.
3. Bấm **Tìm** và chọn cuộc trò chuyện bạn muốn.
4. **Gửi tin nhắn thử**; khi tin nhắn đến, bấm **Lưu**.

Token của bot giống như mật khẩu: đừng chia sẻ nó.

## Cập nhật

Spotter kiểm tra phiên bản mới mỗi ngày một lần (tắt được trong nút phiên bản ở góc trên bên phải).
Khi có bản mới, trang Spotter hiện một thanh thông báo và bạn nhận một tin nhắn. Bấm **Có gì mới**, rồi
**Cài đặt**: Spotter tải về, kiểm tra đúng là bản phát hành thật (có chữ ký), rồi tự khởi động lại.
Khi máy đang in, việc cài đặt sẽ chờ in xong. **Kiểm tra ngay** ở cùng chỗ để kiểm tra luôn.

## Chạy cùng Windows (không bắt buộc)

Để Spotter chạy nền từ lúc bật máy, không cần cửa sổ: mở terminal **bằng quyền Administrator** trong
thư mục của Spotter và chạy

```
.\spotter.exe install
```

Sau đó trang Spotter luôn ở <http://localhost:8484>. `.\spotter.exe uninstall` để gỡ (cài đặt của bạn vẫn còn).
Cập nhật vẫn hoạt động như cũ.

## Khi gặp trục trặc

- **Không tìm thấy máy in:** máy tính và máy in phải cùng một mạng. Nếu khác mạng con (ví dụ máy in dùng
  Wi-Fi còn máy tính cắm dây), thêm mạng con đó trong Thông báo → mạng con cần quét thêm, hoặc thêm máy in
  bằng địa chỉ IP.
- **Không nhận được thông báo:** VPN có thể chặn Telegram; thử tắt VPN. **Gửi thử** trong Thông báo sẽ cho
  biết lỗi.
- **"Is Spotter already running?":** Spotter đang chạy rồi (ở cửa sổ khác hoặc chạy nền). Trang Spotter vẫn
  được mở.

`FFMPEG.txt` trong file zip cho biết bản ffmpeg đi kèm và nơi có mã nguồn của nó.
