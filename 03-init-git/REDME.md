# 📘 Bài 3: Khởi tạo dự án đầu tiên với | Lesson 3: Initialize Your First Git Project

---

## 🎯 Mục tiêu bài học | Lesson Objectives

- Tạo thư mục dự án và khởi tạo Git  
  *(Create a project folder and initialize Git)*  
- Cấu hình `.gitignore` để loại trừ các file không cần thiết  
  *(Configure `.gitignore` to exclude unnecessary files)*  
- Sử dụng `git add` để thêm file vào vùng staging  
  *(Use `git add` to add files to the staging area)*  
- Kiểm tra trạng thái dự án bằng `git status`  
  *(Check project status using `git status`)*

---

## 📁 1. Tạo thư mục dự án | Create the project folder

### 🖐️ Cách 1: Tạo bằng tay  
### ✋ Method 1: Manual creation

- Tạo một thư mục tên là `learn-git`  
  *(Create a folder named `learn-git`)*
- Mở thư mục này bằng VS Code hoặc trình soạn thảo bạn yêu thích  
  *(Open the folder in VS Code or your preferred editor)*

---

### 💻 Cách 2: Tạo bằng terminal | Method 2: Using the terminal

```bash
mkdir learn-git
cd learn-git
code .
```

---

## 🌱 2. Khởi tạo Git | Initialize Git

```bash
git init
```

### 🇻🇳 Giải thích:  
Lệnh này sẽ tạo ra một thư mục ẩn tên là `.git` trong dự án của bạn. Thư mục này chứa toàn bộ thông tin lịch sử và cấu hình Git cho dự án.  
📦 `.git` là trung tâm hoạt động của Git trong thư mục hiện tại.

### 🇺🇸 Explanation:  
This command creates a hidden folder named `.git` in your project. This folder contains the entire Git history and configuration for the repository.  
📦 `.git` is the heart of Git in the current directory.

---

## 📂 3. Tạo file `.gitignore` | Create `.gitignore` file

File `.gitignore` dùng để **bỏ qua các file không nên** đưa vào hệ thống quản lý mã nguồn Git (như thư viện, file tạm, thông tin cá nhân, v.v).

The `.gitignore` file is used to **exclude files you don’t want** tracked by Git (such as libraries, temp files, personal configs, etc.).

### 📝 Ví dụ nội dung `.gitignore` | Example `.gitignore` content

```bash
node_modules/
.env
.DS_Store
vendor/
storage/
```

### 🗒️ Giải thích từng dòng | Explanation of each line

| Dòng | Mục đích (VN) | Purpose (EN) |
|------|---------------|--------------|
| `node_modules/` | Thư mục chứa thư viện NPM | NPM packages folder |
| `.env` | File chứa biến môi trường | Environment variables |
| `.DS_Store` | File hệ thống của macOS | macOS system file |
| `vendor/` | Thư viện PHP (Laravel) | PHP dependencies (Laravel) |
| `storage/` | Dữ liệu cache/tạm của Laravel | Cache/temp data for Laravel |

---

## 🔍 4. Kiểm tra trạng thái | Check Git status

```bash
git status
```

### 🇻🇳 Giải thích:  
Lệnh này cho bạn biết trạng thái hiện tại của thư mục làm việc: file nào đã thay đổi, file nào chưa theo dõi, và file nào đã được đưa vào vùng staging.

### 🇺🇸 Explanation:  
This command tells you the current status of your working directory: which files have been modified, which are untracked, and which are staged.

---

## 🧪 5. Thêm file vào vùng staging | Add files to staging area

**Vùng staging (Staging area)** là nơi bạn chuẩn bị các file trước khi lưu chúng vào Git (commit).

**The staging area** is like a prep zone where you collect changes before you officially commit them to Git history.

---

### ✅ 5.1 Thêm 1 file cụ thể | Add a specific file

```bash
git add index.html
```

- 🇻🇳 Lệnh này thêm `index.html` vào vùng staging  
- 🇺🇸 This adds `index.html` to the staging area

---

### ✅ 5.2 Thêm toàn bộ file | Add all changes

```bash
git add .
```

- 🇻🇳 Thêm tất cả file mới và đã thay đổi vào vùng staging  
- 🇺🇸 Adds all new and modified files to staging

📌 Lưu ý: Các file trong `.gitignore` sẽ không được thêm.  
📌 Note: Files listed in `.gitignore` will be skipped.

---

## 🧠 Tổng kết | Recap

| Hành động | Lệnh | Ý nghĩa |
|----------|------|--------|
| Khởi tạo Git | `git init` | Tạo repo Git trong thư mục hiện tại *(create a Git repo in current folder)* |
| Kiểm tra trạng thái | `git status` | Kiểm tra file đã thay đổi, đã stage, chưa stage *(see changes and staging info)* |
| Thêm file cụ thể | `git add <file>` | Đưa 1 file vào vùng staging *(stage one file)* |
| Thêm tất cả | `git add .` | Đưa tất cả file thay đổi vào staging *(stage all changes)* |
| Tạo `.gitignore` | thủ công | Định nghĩa các file cần loại bỏ khỏi tracking *(exclude files from Git tracking)* |

---

## 🎉 Bạn đã hoàn thành Bài 3!  
## 🎉 You’ve completed Lesson 3!

---

📦 Trong bài tiếp theo, chúng ta sẽ học cách `git commit` để lưu lại thay đổi một cách chính thức và khám phá `git log` để xem lịch sử commit.
