Tuyệt vời! Dưới đây là bài **Bài 3** đã được **sửa lại theo yêu cầu của bạn**:

---

# 🧱 Bài 3: Tạo dự án Git đầu tiên & Git Ignore  
## 🧱 Lesson 3: Create First Git Project & Git Ignore

---

## 🎯 🇻🇳 Mục tiêu  
- Tạo thư mục dự án để học Git  
- Khởi tạo Git trong thư mục  
- Cấu hình `.gitignore` trước khi thêm và commit  
- Thêm file vào Git (git add)  
- Giải thích `git add .`  

## 🎯 🇺🇸 Objectives  
- Create a project folder to learn Git  
- Initialize Git in the folder  
- Configure `.gitignore` before adding or committing files  
- Add files to Git using `git add`  
- Explain `git add .`

---

## 📁 1. Tạo thư mục dự án  
## 📁 1. Create project folder  

**Tên thư mục – Folder name:** `bai-3-gitignore-va-git-add`

### ✅ 🇻🇳 Cách 1: Tạo bằng tay  
1. Mở File Explorer hoặc Finder  
2. Tạo thư mục mới tên `bai-3-gitignore-va-git-add`  
3. Mở thư mục này bằng VS Code

### ✅ 🇺🇸 Method 1: Create manually  
1. Open File Explorer or Finder  
2. Create a new folder named `bai-3-gitignore-va-git-add`  
3. Open it in VS Code

---

### 💻 🇻🇳 Cách 2: Tạo bằng Terminal

```bash
mkdir bai-3-gitignore-va-git-add
cd bai-3-gitignore-va-git-add
code .
```

### 💻 🇺🇸 Method 2: Using Terminal

```bash
mkdir bai-3-gitignore-va-git-add
cd bai-3-gitignore-va-git-add
code .
```

---

## 🚀 2. Khởi tạo Git  
## 🚀 2. Initialize Git

```bash
git init
```

- 🇻🇳 Tạo thư mục ẩn `.git` để theo dõi phiên bản  
- 🇺🇸 Creates a hidden `.git` folder to track version history

---

## 🚫 3. Tạo file `.gitignore` trước  
## 🚫 3. Create `.gitignore` file first

> 🎯 🇻🇳 `.gitignore` giúp bạn loại trừ những file không nên được đẩy lên Git như file cấu hình cá nhân, file tạm, thư mục thư viện,…  
> 🎯 🇺🇸 `.gitignore` helps you exclude files that shouldn't be pushed to Git like personal configs, temp files, libraries, etc.

---

### 📄 🇻🇳 Một số file thường được ignore  
### 📄 🇺🇸 Common files to ignore

| Tệp / Thư mục        | 🇻🇳 Giải thích                  | 🇺🇸 Explanation                    |
|----------------------|-------------------------------|-----------------------------------|
| `node_modules/`      | Thư viện Node.js              | Node.js dependencies              |
| `.env`               | Biến môi trường (mật khẩu,…)  | Environment variables (secrets)   |
| `vendor/`            | Thư viện PHP/Laravel          | Laravel/PHP dependencies          |
| `.DS_Store`          | File hệ thống của macOS       | macOS system file                 |
| `dist/`              | Mã sau khi build              | Compiled production code          |
| `*.log`              | File log (ghi lỗi)            | Log files                         |

---

### ✍️ 🇻🇳 Tạo `.gitignore` bằng tay  
- Chuột phải → New File → đặt tên `.gitignore`  
- Thêm nội dung:

```gitignore
node_modules/
.env
.DS_Store
dist/
*.log
```

### 💻 🇺🇸 Or use Terminal

```bash
touch .gitignore
```

---

## 📄 4. Tạo file thực hành  
## 📄 4. Create practice file

```bash
echo "Xin chào Git!" > hello.txt
```

```bash
echo "API_KEY=123456" > .env
```

> 📌 `.env` chứa thông tin bí mật → sẽ bị **ignore**  
> 📌 `.env` contains secrets → will be **ignored**

---

## 🧪 5. Kiểm tra trạng thái  
## 🧪 5. Check Git status

```bash
git status
```

- 🇻🇳 Bạn sẽ thấy `hello.txt` là file chưa được theo dõi (untracked)  
- 🇺🇸 You'll see `hello.txt` as an untracked file  
- 🇻🇳 `.env` sẽ không xuất hiện vì đã bị `.gitignore`  
- 🇺🇸 `.env` won’t show because it’s ignored

---

## ➕ 6. Thêm file với `git add`  
## ➕ 6. Add files with `git add`

### 📌 6.1 🇻🇳 Thêm một tệp  
```bash
git add hello.txt
```

- 🇻🇳 Chỉ thêm file `hello.txt` vào vùng staging  
- 🇺🇸 Only adds `hello.txt` to the staging area

---

### 📌 6.2 🇻🇳 Thêm tất cả thay đổi  
```bash
git add .
```

- 🇻🇳 Thêm tất cả file mới/chỉnh sửa vào staging (trừ file bị ignore)  
- 🇺🇸 Add all new/modified files to staging (excluding ignored files)

> 🧠 **Staging area** (vùng tạm): khu vực tạm chứa thay đổi trước khi commit  
> 🧠 **Staging area**: a temporary zone before committing changes

---

## ✅ Tóm tắt  
## ✅ Summary

| Lệnh Git           | 🇻🇳 Mục đích                          | 🇺🇸 Purpose                         |
|--------------------|---------------------------------------|------------------------------------|
| `git init`         | Khởi tạo Git repository              | Initialize Git repository          |
| `touch .gitignore` | Tạo file ignore                      | Create ignore file                 |
| `git add file`     | Thêm 1 file vào staging              | Add single file to staging         |
| `git add .`        | Thêm tất cả file (trừ ignore)        | Add all files (except ignored)     |
| `git status`       | Kiểm tra trạng thái tệp              | Check file status                  |

---
