# ServiceHub — Kế hoạch và tiến độ 6 Sprint

> Cập nhật: 10/11/2026. Tài liệu dựa trên trạng thái Issue/PR của repository `huyyl728/Team_3` và phạm vi ServiceHub Python đã được thảo luận. **Issue đóng không tự động chứng minh mã nguồn đã merge hoặc kiểm thử thành công.**

## Phạm vi và nguồn kiểm chứng

- GitHub repository: https://github.com/huyyl728/Team_3
- Nhánh mặc định `main` tại thời điểm rà soát chỉ có `README.md` với tiêu đề “Nhóm 3”, chưa có mã nguồn ServiceHub.
- [PR #9](https://github.com/huyyl728/Team_3/pull/9) (giao diện tĩnh Sprint 1) vẫn là bản nháp, chưa merge.
- Các Issue #1–#8 và #10–#28 đã đóng theo GitHub; các issue #10, #11, #12 có tiêu đề trùng nhau.
- **Các Issue #29–#43 được tạo mới làm backlog; không được đánh dấu Done nếu thiếu bằng chứng.**
- Phiên bản ZIP ServiceHub có VietQR đã được phát triển ngoài GitHub; phải được kiểm tra bí mật/cơ sở dữ liệu và đưa vào GitHub qua PR trước khi coi là tích hợp.

## Bảng tổng quan

| Sprint | Mục tiêu | Issue | Trạng thái theo GitHub | Đầu ra cần nghiệm thu |
|---|---|---|---|---|
| 1 | Ý tưởng, khởi tạo, giao diện HTML/CSS responsive | #1–#8, #10–#15 | Các Issue đã đóng; PR #9 chưa merge | Trang chủ, chi tiết, navigation, cấu trúc dự án |
| 2 | Tài khoản, phân quyền và cơ sở kinh doanh | #16–#21 | Các Issue đã đóng; chưa có code trên main | Đăng nhập, hồ sơ, Owner/Admin, phê duyệt cơ sở |
| 3 | Danh sách, tìm kiếm, quản lý dịch vụ, hình ảnh, chi tiết | #22–#28 | Các Issue đã đóng; chưa có code trên main | Lọc danh mục, gợi ý từ khóa, CRUD, upload, chi tiết |
| 4 | Đặt lịch, ví demo/VietQR, hội viên, thông báo, admin | #29–#33 | Open; cần tích hợp/kiểm thử | API + UI + test, mã nguồn và cấu hình an toàn |
| 5 | Kiểm thử thủ công, UX, bảo mật, Docker/LAN, CI | #34–#38 | Open / kế hoạch | 20 Test Case, bug report, CI, chạy LAN |
| 6 | UAT, tài liệu, báo cáo Sprint, demo, đánh giá triển khai | #39–#43 | Open / kế hoạch | Báo cáo nghiệm thu, kịch bản demo, backlog rủi ro |

## Sprint 1 — Khởi tạo & giao diện

**Mục tiêu:** có ý tưởng, cấu trúc mã nguồn và trang giao diện đầu tiên.

- [x] Các Issue lịch sử [#1](https://github.com/huyyl728/Team_3/issues/1), [#2](https://github.com/huyyl728/Team_3/issues/2), [#3](https://github.com/huyyl728/Team_3/issues/3), [#4](https://github.com/huyyl728/Team_3/issues/4), [#5](https://github.com/huyyl728/Team_3/issues/5), [#6](https://github.com/huyyl728/Team_3/issues/6), [#7](https://github.com/huyyl728/Team_3/issues/7), [#8](https://github.com/huyyl728/Team_3/issues/8) đã đóng trên GitHub.
- [x] Các Issue [#10](https://github.com/huyyl728/Team_3/issues/10)–[#15](https://github.com/huyyl728/Team_3/issues/15) đã đóng.
- [ ] Xác minh mã nguồn đã merge vào nhánh chính; [PR #9](https://github.com/huyyl728/Team_3/pull/9) vẫn nháp.
- **Acceptance Criteria:** HTML có trang chủ, trang chi tiết và điều hướng; CSS responsive; có hướng dẫn chạy.

## Sprint 2 — Tài khoản & nhà cung cấp

**Mục tiêu:** xác thực, hồ sơ, phân quyền và luồng đăng ký nhà cung cấp.

- [x] Các Issue [#16](https://github.com/huyyl728/Team_3/issues/16)–[#21](https://github.com/huyyl728/Team_3/issues/21) đã đóng theo GitHub.
- [ ] Đối chiếu mã nguồn trên nhánh chính với các thao tác đăng nhập, hồ sơ, đăng ký Owner, phê duyệt Admin.
- **Acceptance Criteria:** Customer không gọi API Admin; chủ cơ sở không sửa dữ liệu người khác; dữ liệu lưu được trong SQLite.

## Sprint 3 — Khám phá & dịch vụ

**Mục tiêu:** người dùng tìm được dịch vụ, chủ cơ sở quản lý dịch vụ và ảnh.

- [x] Các Issue [#22](https://github.com/huyyl728/Team_3/issues/22)–[#28](https://github.com/huyyl728/Team_3/issues/28) đã đóng theo GitHub.
- [ ] Đối chiếu mã nguồn và kiểm thử các chức năng search suggestions, category filter, CRUD, ảnh riêng, banner, chi tiết.
- **Acceptance Criteria:** tìm kiếm đúng với từ khóa không dấu, ảnh dịch vụ độc lập với banner cơ sở, quản lý đúng theo Owner.

## Sprint 4 — Nghiệp vụ mở rộng & VietQR

- [ ] [#29 — Đặt lịch và chống trùng](https://github.com/huyyl728/Team_3/issues/29)
- [ ] [#30 — Ví demo/VietQR, đối soát thủ công](https://github.com/huyyl728/Team_3/issues/30)
- [ ] [#31 — Hội viên theo cơ sở](https://github.com/huyyl728/Team_3/issues/31)
- [ ] [#32 — Thông báo và quản trị](https://github.com/huyyl728/Team_3/issues/32)
- [ ] [#33 — Tích hợp mã nguồn và hồi quy](https://github.com/huyyl728/Team_3/issues/33)
- **Acceptance Criteria:** không tự đánh dấu thanh toán khi mới tạo QR; không đưa `.env`, thông tin ngân hàng thực, database cá nhân hay uploads vào Git; API được kiểm thử và phân quyền.

## Sprint 5 — Nâng cao chất lượng

- [ ] [#34 — Kiểm thử thủ công 20 Test Case](https://github.com/huyyl728/Team_3/issues/34)
- [ ] [#35 — UX, tìm kiếm và bộ gợi ý 3 câu hỏi](https://github.com/huyyl728/Team_3/issues/35)
- [ ] [#36 — Rà soát bảo mật/phân quyền](https://github.com/huyyl728/Team_3/issues/36)
- [ ] [#37 — Docker, LAN, dữ liệu bền vững](https://github.com/huyyl728/Team_3/issues/37)
- [ ] [#38 — CI và xử lý lỗi API](https://github.com/huyyl728/Team_3/issues/38)
- **Acceptance Criteria:** có actual results và bug reports của 20 Test Case, hướng dẫn tái hiện và sửa lỗi; CI/khởi động local được xác minh.

## Sprint 6 — Nghiệm thu và bàn giao

- [ ] [#39 — Kiểm thử end-to-end](https://github.com/huyyl728/Team_3/issues/39)
- [ ] [#40 — Tài liệu cài đặt, kiến trúc](https://github.com/huyyl728/Team_3/issues/40)
- [ ] [#41 — Báo cáo Sprint và issue](https://github.com/huyyl728/Team_3/issues/41)
- [ ] [#42 — Demo và thuyết trình](https://github.com/huyyl728/Team_3/issues/42)
- [ ] [#43 — Rủi ro triển khai production](https://github.com/huyyl728/Team_3/issues/43)
- **Acceptance Criteria:** nhóm 4 thành viên demo được luồng đã xác minh, báo cáo rõ Pass/Fail/Blocked, nêu giới hạn của ví demo và VietQR.

## Cách quản lý nhóm 4 thành viên

Thành viên có trong issue lịch sử: `huyyl728`, `huybui330`, `Hung2k7n`, `tuanhungnguyendac-netizen`. Chưa tự gán issue mới vì cần xác nhận phân công thực tế.

- Frontend: giao diện, responsive, tìm kiếm/gợi ý.
- Backend: API, SQLite, kiểm tra nghiệp vụ, phân quyền.
- Provider/Admin: quản lý dịch vụ, lịch và bảng điều khiển.
- QA/Tích hợp: 20 test case, CI, Docker và báo cáo.

## Quy tắc đánh dấu hoàn thành

1. Issue **Closed** = trạng thái trên GitHub; chưa đủ để kết luận mã đã merge.
2. Chỉ chuyển Issue mới sang **Closed** khi có link commit/PR, test hoặc demo phù hợp tiêu chí nghiệm thu.
3. Không commit thông tin ngân hàng, mật khẩu, tệp `.env`, database hoặc upload cá nhân.
4. Không đánh đồng VietQR có thể quét với giao dịch đã thanh toán thành công.
5. Khi có kết quả chạy thực tế, cập nhật báo cáo Sprint và gắn bằng chứng vào Issue.
