# Hướng dẫn Sử dụng Git: Một Cẩm Nang Toàn Diện

## 1. Giới Thiệu về Git

### 1.1 Khái niệm
![](./image/git.jpg)

Git là một hệ thống quản lý phiên bản phân tán (DVCS), vô cùng mạnh mẽ và linh hoạt, thiết kế để xử lý từ những dự án nhỏ đến các dự án lớn với hiệu suất cao. Được phát triển bởi Linus Torvalds vào năm 2005, Git đã trở thành công cụ chuẩn trong ngành phát triển phần mềm.

### 1.2 Lợi ích

Git không chỉ giúp bảo vệ tính toàn vẹn của mã nguồn qua các phiên bản khác nhau mà còn tối ưu hóa quy trình làm việc nhóm bằng cách cung cấp các tính năng như branching và merging, đồng thời hỗ trợ quản lý lịch sử thay đổi một cách hiệu quả.

## 2. Kiến Trúc của Git
![Cấu trúc của git](./image/cấu%20trúc%20git.jpg)

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
## 5. Demo: Tải và Cài đặt Git từ Đầu

Trong phần demo này, chúng ta sẽ đi qua các bước để tải về và cài đặt Git trên máy tính của bạn, sau đó thực hiện một số lệnh cơ bản để khởi tạo một repository Git mới.

### Bước 1: Tải Git

1. **Truy cập trang web chính thức của Git**
   - Mở trình duyệt web và truy cập vào [https://git-scm.com/](https://git-scm.com/).
   
2. **Tải xuống**
   - Nhấp vào nút "Download" để tải xuống phiên bản Git mới nhất cho hệ điều hành của bạn.

### Bước 2: Cài đặt Git

1. **Mở file cài đặt**
   - Sau khi tải xuống, mở file cài đặt Git (.exe, .dmg, hoặc .sh tùy thuộc vào hệ điều hành).
   
2. **Chạy trình cài đặt**
   - Thực hiện theo các bước trong trình cài đặt. Đối với người dùng Windows, bạn có thể chọn các tùy chọn mặc định. Người dùng macOS và Linux thường cần chạy qua Terminal.
   
3. **Kiểm tra việc cài đặt**
   - Mở Terminal hoặc Command Prompt và nhập `git --version` để xác nhận Git đã được cài đặt thành công.

### Bước 3: Cấu hình Git

1. **Thiết lập tên người dùng và email**
   - Mở Terminal hoặc Command Prompt.
   - Đặt tên người dùng của bạn bằng cách nhập `git config --global user.name "Tên của bạn"`.
   - Đặt email của bạn bằng cách nhập `git config --global user.email "email@của bạn"`.
   
2. **Kiểm tra cấu hình**
   - Kiểm tra các cấu hình hiện tại bằng lệnh `git config --list`.

### Bước 4: Khởi tạo một Repository mới

1. **Tạo một thư mục mới** (nếu cần)
   - Sử dụng lệnh `mkdir ten-du-an` để tạo một thư mục mới cho dự án của bạn.
   
2. **Di chuyển vào thư mục dự án**
   - Sử dụng lệnh `cd ten-du-an` để chuyển vào thư mục dự án bạn vừa tạo.
   
3. **Khởi tạo repository**
   - Trong thư mục dự án, nhập `git init` để khởi tạo một repository Git mới.
   
4. **Thêm file vào repository** (tùy chọn)
   - Sử dụng lệnh `git add <file_name>` để thêm các file vào staging area.
   - Hoặc sử dụng `git add .` để thêm tất cả các file trong thư mục hiện tại.
   
5. **Commit thay đổi**
   - Sử dụng lệnh `git commit -m "Thông điệp commit"` để lưu các thay đổi vào repository.

Lưu ý: Đảm bảo rằng bạn đã đặt tên và email trong cấu hình Git trước khi thực hiện commit đầu tiên.

