# edit-video-tranh-dang-nhac-trend

Skill VAS dựng video quảng cáo tranh 10 giây theo video gốc và nhạc người dùng cung cấp.

## Cài đặt

1. Tải [gói skill](edit-video-tranh-dang-nhac-trend-skill.zip) và giải nén vào `customs/skills/edit-video-tranh-dang-nhac-trend/` trong VAS. `SKILL.md`, `scripts/`, `assets/`, `workflow.md` và `plan-schema.md` cần nằm cùng thư mục skill.
2. Đọc `SKILL.md`, `workflow.md`, `plan-schema.md` và `AGENTS.md` của VAS. Chạy `python scripts/vas.py doctor` tại thư mục gốc VAS. Khi dựng, cần Python 3.11+, Pillow, NumPy, FFmpeg và ffprobe.
3. Để dùng trong ChatGPT trình duyệt, kết nối plugin/MCP VAS với máy VAS đang chạy trong tài khoản hoặc workspace ChatGPT của bạn. Kiểm tra `checkVAS` trước khi giao video. Kết nối này cần cấu hình riêng; link GitHub không tự cấp quyền truy cập máy.

Không đưa khóa API, footage hoặc dữ liệu fanpage lên GitHub. Sau khi cài, chỉ báo sẵn sàng và chờ người dùng cung cấp video gốc cùng nhạc. Không tự phiên âm, dựng thử hoặc đăng Facebook. Video chỉ có nhạc và chữ không cần Vbee hay Faster Whisper; dùng Faster Whisper cục bộ của VAS nếu sau này có lời nói và người dùng yêu cầu phiên âm.

## Lệnh mẫu cho ChatGPT

> Set up https://github.com/tranhthammy-art/edit-video-tranh-dang-nhac-trend for me. Read README.md and SKILL.md in the ZIP first. Install the skill into my VAS folder, check Python and FFmpeg, and connect the VAS MCP plugin in this ChatGPT account. Keep keys in the local .env, not in chat. After verifying checkVAS, tell me it is ready and wait for my source video and music. Do not transcribe or render anything on your own.
