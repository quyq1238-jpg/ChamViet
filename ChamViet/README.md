# Học liệu Tin học và Chấm Việt

Kho mã gồm:

- `index.html`: học liệu tương tác **Bài 4 — Bên trong máy tính**.
- `omr/`: ứng dụng **Chấm Việt**, hỗ trợ tạo bài kiểm tra, nhập và xác nhận đáp án, in phiếu, nhận dạng OMR, duyệt và lưu điểm, chấm lại và xuất báo cáo.

## Sử dụng Chấm Việt

Xem [hướng dẫn cài đặt, sử dụng và triển khai HTTPS](omr/README.md), [kết quả kiểm thử và giới hạn](omr/TEST_RESULTS.md), cùng [dữ liệu thử có nhãn](omr/samples/).

Backend dùng Python 3.12/FastAPI, SQLite và OpenCV; frontend dùng HTML/CSS/JavaScript. Mã nguồn không kèm tài khoản, ảnh bài làm thật, cơ sở dữ liệu hay khóa bí mật. `.env.example` chỉ chứa cấu hình mẫu.

GitHub Pages có thể phục vụ trang học liệu tĩnh `index.html`. Chấm Việt cần chạy backend Python trên máy chủ có ổ đĩa bền vững và HTTPS để sử dụng camera điện thoại.

## Đưa bản ZIP vào kho Git của bạn

Clone kho GitHub về máy, giải nén các tệp mã nguồn vào thư mục kho vừa clone, rồi thực hiện:

```bash
git switch -c cham-viet-omr
git add README.md omr
git commit -m "Add Cham Viet OMR grading application"
git push -u origin cham-viet-omr
```

Nếu nhánh này đã tồn tại, dùng một tên nhánh mới. Sau đó có thể tạo pull request trên GitHub để đưa thay đổi vào nhánh chính. Không thêm dữ liệu học sinh, cơ sở dữ liệu, môi trường Python hay tệp `.env` vào Git.
