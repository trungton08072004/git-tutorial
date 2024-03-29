# Hướng dẫn Sử dụng Git: Một Cẩm Nang Toàn Diện

## 1. Giới Thiệu về Git

### 1.1 Khái niệm

Git là một hệ thống quản lý phiên bản phân tán (DVCS), vô cùng mạnh mẽ và linh hoạt, thiết kế để xử lý từ những dự án nhỏ đến các dự án lớn với hiệu suất cao. Được phát triển bởi Linus Torvalds vào năm 2005, Git đã trở thành công cụ chuẩn trong ngành phát triển phần mềm.

### 1.2 Lợi ích

Git không chỉ giúp bảo vệ tính toàn vẹn của mã nguồn qua các phiên bản khác nhau mà còn tối ưu hóa quy trình làm việc nhóm bằng cách cung cấp các tính năng như branching và merging, đồng thời hỗ trợ quản lý lịch sử thay đổi một cách hiệu quả.

## 2. Kiến Trúc của Git

### 2.1 Thành Phần Cốt Lõi

- **Working Directory**: Nơi chứa các file đang được làm việc.
- **Staging Area (Index)**: Khu vực tạm thời để lưu trữ các thay đổi trước khi commit vào repository.
- **Repository (Repo)**: Cơ sở dữ liệu của Git, lưu trữ lịch sử thay đổi và các snapshot của dự án.

## 3. Thuật ngữ cơ bản trong Git

- **Commit**: Lưu một snapshot của các thay đổi trong repository.
- **Branch**: Một dòng phát triển độc lập, cho phép bạn thử nghiệm và phát triển tính năng mà không ảnh hưởng đến phần khác của dự án.
- **Merge**: Kết hợp lịch sử của các nhánh lại với nhau.
- **Pull**: Lấy dữ liệu từ repository từ xa và tích hợp nó với nhánh hiện tại.
- **Push**: Gửi các thay đổi từ nhánh hiện tại lên repository từ xa.

## 4. Các Lệnh Cơ Bản của Git

- `git init`: Khởi tạo một repository mới.
- `git clone <url>`: Sao chép repository từ một địa chỉ từ xa.
- `git add <file>`: Thêm file vào staging area để chuẩn bị cho việc commit.
- `git commit -m "<message>"`: Commit các thay đổi trong staging area với một thông điệp mô tả.
- `git push <remote> <branch>`: Đẩy các thay đổi lên repository từ xa.
- `git pull <remote> <branch>`: Cập nhật nhánh hiện tại với các thay đổi từ nhánh từ xa.
- `git branch <branch-name>`: Tạo nhánh mới.
- `git checkout <branch-name>`: Chuyển đổi sang nhánh được chỉ định.
