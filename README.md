# Nhóm 3 — ServiceHub

ServiceHub là dự án nền tảng khám phá, quản lý và đặt dịch vụ (Python/SQLite, HTML/CSS/JavaScript). Nhóm sử dụng 6 Sprint để quản lý công việc.

## Sprint backlog và tiến độ

Xem tài liệu [Kế hoạch Sprint 1–6](docs/SPRINT_PLAN_1_TO_6.md) để biết mục tiêu, Issue đã đóng, Issue còn mở và tiêu chí nghiệm thu.

| Sprint | Phạm vi | GitHub Issue |
| --- | --- | --- |
| 1 | Khởi tạo, giao diện, responsive | #1–#8, #10–#15 |
| 2 | Tài khoản, phân quyền, cơ sở | #16–#21 |
| 3 | Tìm kiếm, dịch vụ, hình ảnh | #22–#28 |
| 4 | Đặt lịch, hội viên, ví demo, VietQR, quản trị | #29–#33 |
| 5 | Kiểm thử, UX, bảo mật, Docker, CI | #34–#38 |
| 6 | Nghiệm thu, tài liệu, báo cáo và demo | #39–#43 |

> **Trạng thái:** Issue cũ đã đóng không có nghĩa mã nguồn đã có trên nhánh `main`. Tại thời điểm lập kế hoạch, code ServiceHub đang ở phiên bản ZIP phát triển ngoài GitHub và phải được review/tích hợp an toàn qua PR. Các Issue mới vẫn Open cho đến khi có bằng chứng nghiệm thu. [PR #9](https://github.com/huyyl728/Team_3/pull/9) của Sprint 1 vẫn là bản nháp.

## Quy tắc cộng tác

- Dùng issue để phân công và theo dõi công việc; gắn PR, commit và test tương ứng.
- Không commit `.env`, mật khẩu, tài khoản ngân hàng, dữ liệu SQLite cá nhân hoặc thư mục uploads.
- VietQR là luồng tạo yêu cầu chuyển khoản; chỉ xác nhận đã thanh toán sau khi đối soát giao dịch thực tế.
