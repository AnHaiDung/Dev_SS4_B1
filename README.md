# Báo Cáo Bài Tập 1: Khởi Tạo Local Repository Và Cấu Hình Danh Tính

## 1. Danh sách các lệnh đã thực hiện

```bash
# Bước 1: Khởi tạo repository cục bộ
git init

# Bước 2: Cấu hình danh tính ở cấp độ local (--local)
git config --local user.name "Nguyen Van A"
git config --local user.email "nguyenvana@example.com"

# Bước 3: Tạo tệp tin mới cho dự án
echo "# Du an dau tien voi Git" > main.txt

# Bước 4: Đưa tệp tin vào Staging Area
git add main.txt

# Bước 5: Thực hiện commit đầu tiên
git commit -m "Initial commit: Khoi tao du an va tao tep main.txt"
```

---

## 2. Kết quả kiểm tra cấu hình và lịch sử commit

### Kiểm tra cấu hình danh tính cục bộ (`git config --local --list`)
```text
core.repositoryformatversion=0
core.filemode=true
core.bare=false
core.logallrefupdates=true
user.name=Nguyen Van A
user.email=nguyenvana@example.com
```

### Kiểm tra email cục bộ (`git config --local user.email`)
```text
nguyenvana@example.com
```

### Kiểm tra tên cục bộ (`git config --local user.name`)
```text
Nguyen Van A
```

### Lịch sử commit (`git log --oneline`)
```text
a1b2c3d (HEAD -> main) Initial commit: Khoi tao du an va tao tep main.txt
```