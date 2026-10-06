# YT Downloader

App tải video và playlist YouTube về máy dưới dạng **MP3** hoặc **video MP4**, chạy trên **macOS** và **Windows**.

## Tải về

Vào trang [**Releases mới nhất**](https://github.com/dinhduan183/YT-Downloader-release/releases/latest) và tải file theo máy của bạn:

| Hệ điều hành | File |
|---|---|
| macOS (chip Apple M1 trở lên) | `YouTube-Downloader-macOS.zip` |
| Windows 10/11 | `YouTube-Downloader-Windows.zip` |

## Tính năng

- Tải **video lẻ** hoặc **cả playlist**.
- Chọn **MP3** (320 / 192 / 128 kbps) hoặc **Video MP4** (Tốt nhất / 1080p / 720p / 480p).
- Quét và hiện danh sách video của playlist trước khi tải.
- Tải **1–3 bài cùng lúc**, có % từng bài và thanh tiến độ chung.
- Tự thử lại khi YouTube chặn tạm thời (lỗi 403); có nút **Tải lại bài lỗi**.
- Nhớ thư mục lưu và các lựa chọn cho lần mở sau.
- Báo khi có phiên bản mới.

### Cách đặt tên file

- **Video lẻ:** `<Thư mục lưu>/<Tên video>.mp3`
- **Playlist:** `<Thư mục lưu>/<Tên playlist>/01. <Tên video>.mp3`

## Cài đặt

App cần **ffmpeg** để chuyển sang MP3 và ghép video. Chỉ cần cài một lần.

### macOS

1. Cài ffmpeg bằng [Homebrew](https://brew.sh):
   ```bash
   brew install ffmpeg
   ```
2. Giải nén `YouTube-Downloader-macOS.zip`, kéo **YouTube Downloader.app** vào thư mục **Applications**.
3. **Lần mở đầu tiên:** chuột phải vào app → **Open** → **Open**.
   App chưa được Apple ký nên macOS sẽ báo "không xác định được nhà phát triển". Chỉ cần làm bước này một lần.

> Chưa hỗ trợ Mac chip Intel.

### Windows

1. Cài ffmpeg (mở **PowerShell** và chạy):
   ```powershell
   winget install Gyan.FFmpeg
   ```
2. Giải nén `YouTube-Downloader-Windows.zip`, mở thư mục **YouTube Downloader** và chạy **YouTube Downloader.exe**.
   Giữ nguyên thư mục `_internal` bên cạnh file `.exe`.
3. Nếu Windows SmartScreen chặn: bấm **More info** → **Run anyway**.

## Sử dụng

1. Dán link video hoặc playlist YouTube vào ô **URL**.
2. Chọn **thư mục lưu**, **định dạng** và **chất lượng**.
3. Bấm **Tải về** (hoặc nhấn Enter).

Với link video nằm trong playlist (có `&list=...`): tick **"Tải cả playlist nếu link có playlist"** để tải cả playlist, bỏ tick để chỉ tải video đó.

## Cập nhật

Khi có bản mới, app hiện thông báo ở đầu cửa sổ. Bấm **Tải về** để mở trang release, tải file mới rồi thay app cũ.

Nếu tải liên tục bị lỗi, hãy cập nhật lên bản mới nhất: YouTube thay đổi thường xuyên và mỗi bản mới đi kèm công cụ tải mới hơn.

## Lưu ý

Chỉ dùng để tải nội dung bạn có quyền tải, và tuân thủ [Điều khoản dịch vụ của YouTube](https://www.youtube.com/t/terms).
