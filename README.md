# Giới thiệu về Git

Git là hệ thống quản lý phiên bản mã nguồn phân tán được sử dụng rộng rãi nhất hiện nay.

 Git cho phép bạn theo dõi lịch sử thay đổi của mã nguồn, cộng tác với người khác và quản lý nhiều phiên bản của dự án một cách hiệu quả.

# Kiến trúc của Git
Git có kiến trúc phi tập trung, nghĩa là mỗi người dùng đều có bản sao đầy đủ của kho lưu trữ (repository) trên máy tính của họ. Khi bạn thực hiện thay đổi, bạn chỉ cần cập nhật bản sao cục bộ của mình và sau đó đẩy (push) những thay đổi đó lên kho lưu trữ từ xa (remote repository).

# Các thuật ngữ
## Thành phần:

- Repository: Nơi lưu trữ lịch sử dự án (mã nguồn, phiên bản, thông tin). Có hai loại: Local (cục bộ) và Remote (từ xa).
  
- Working Directory: Thư mục làm việc trên máy tính, chứa các tệp dự án. Git theo dõi thay đổi trong thư mục này.
  
- Index: Vùng trung gian giữa Working Directory và Repository. Thêm thay đổi vào đây trước khi commit bằng lệnh git add.

- Commit: Lưu trữ bản sao thay đổi từ Index vào Repository. Mỗi commit có thông điệp mô tả thay đổi.

- Branch: Phiên bản song song của Repository, cho phép phát triển nhiều tính năng/sửa lỗi đồng thời.

- Merge: Kết hợp thay đổi từ một nhánh vào nhánh khác.
- Remote Repository: Phiên bản Repository trên máy chủ từ xa (GitHub, GitLab, Bitbucket).

- Clone: Sao chép Remote Repository vào Local Repository.

## Ưu điểm:

- Linh hoạt, hiệu quả.
- Phát triển song song.
- Quản lý, theo dõi thay đổi hiệu quả.
  

# Các lệnh cơ bản trong Git:
- git init: Khởi tạo một repository Git mới trong thư mục hiện tại.

- git clone : Sao chép (clone) một repository từ URL đã cho vào thư mục hiện tại.

- git add : Thêm một file hoặc thay đổi vào Index (Staging Area) để chuẩn bị cho commit.

- git commit -m "": Ghi nhận (commit) các thay đổi đã được thêm vào Index với một thông điệp mô tả.

- git status: Hiển thị trạng thái của các file trong thư mục làm việc và các file đã thêm vào Index.

- git pull: Kéo (pull) các thay đổi từ Remote Repository về Local Repository và tự động thực hiện merge.

- git push: Đẩy (push) các thay đổi từ Local Repository lên Remote Repository.

- git branch: Liệt kê tất cả các nhánh trong repository và chỉ ra nhánh hiện tại.

- git checkout : Chuyển đổi sang một nhánh khác.

- git merge : Gộp (merge) các thay đổi từ một nhánh vào nhánh hiện tại.

- git log: Hiển thị lịch sử các commit trong repository.

- git remote add : Thêm một Remote Repository với tên được chỉ định và URL đã cho.
git remote -v: Liệt kê tất cả các Remote Repository đã được cấu hình và URL tương ứng.

- git fetch: Kéo về (fetch) tất cả các thay đổi từ Remote Repository mà không thực hiện merge.

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