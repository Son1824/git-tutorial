# Giới thiệu về Git

Git là hệ thống quản lý phiên bản mã nguồn phân tán được sử dụng rộng rãi nhất hiện nay.

 Git cho phép bạn theo dõi lịch sử thay đổi của mã nguồn, cộng tác với người khác và quản lý nhiều phiên bản của dự án một cách hiệu quả.

# Kiến trúc của Git
Git có kiến trúc phi tập trung, nghĩa là mỗi người dùng đều có bản sao đầy đủ của kho lưu trữ (repository) trên máy tính của họ. Khi bạn thực hiện thay đổi, bạn chỉ cần cập nhật bản sao cục bộ của mình và sau đó đẩy (push) những thay đổi đó lên kho lưu trữ từ xa (remote repository).

## Các thuật ngữ
- Repository: Kho lưu trữ mã nguồn.
- Commit: Lưu lại một phiên bản của mã nguồn.
- Branch: Nhánh phát triển của mã nguồn.
- Merge: Hợp nhất các nhánh phát triển lại với nhau.
- Pull: Cập nhật mã nguồn từ kho lưu trữ từ xa về máy tính của bạn.
- Push: Gửi các thay đổi của bạn lên kho lưu trữ từ xa.

# Ví dụ sử dụng Git
Giả sử bạn đang làm việc trên một dự án phần mềm và bạn muốn theo dõi lịch sử thay đổi của mã nguồn. Bạn có thể sử dụng Git để thực hiện việc này như sau:

Khởi tạo một kho lưu trữ mới:
```bash
git init
```

Thêm các tập tin vào khu vực:
```bash
git add index.html main.css
```
Lưu lại một phiên bản mới của mã nguồn:
```bash
git commit -m "Added index.html and main.css"
```