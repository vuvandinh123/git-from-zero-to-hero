# 📦 Bài 2: Hướng dẫn cài đặt Git  
## 📦 Lesson 2: How to Install Git

---

## 🇻🇳 Giới thiệu

Trước khi bạn có thể sử dụng Git, bạn cần cài đặt nó trên máy tính của mình. Bài viết này sẽ hướng dẫn bạn cách cài Git trên **Windows**, **macOS** và **Linux**.

---

## 🇺🇸 Introduction

Before you can use Git, you need to install it on your machine. This guide will show you how to install Git on **Windows**, **macOS**, and **Linux**.

---

## 🪟 Cài đặt Git trên Windows  
### 🪟 Installing Git on Windows

1. Truy cập trang chủ Git:  
   👉 [https://git-scm.com](https://git-scm.com)

2. Nhấn nút **Download for Windows**.

3. Mở file `.exe` và làm theo hướng dẫn cài đặt:
   - Cứ nhấn **Next** cho đến khi xong
   - Chấp nhận cấu hình mặc định (trừ khi bạn biết mình đang làm gì 😄)

4. Sau khi cài xong, mở **Git Bash** để bắt đầu dùng Git.

> ✅ **Kiểm tra:** Mở Git Bash và gõ `git --version`  
> Nếu hiện ra phiên bản → Bạn đã cài thành công!

---

1. Visit the official Git website:  
   👉 [https://git-scm.com](https://git-scm.com)

2. Click on **Download for Windows**.

3. Run the `.exe` file and follow the installation wizard:
   - Keep clicking **Next**
   - Accept default options (unless you know what you’re doing 😄)

4. After installation, open **Git Bash** to use Git.

> ✅ **Verify:** Open Git Bash and run `git --version`  
> If you see a version number → Git is installed successfully!

---

## 🍎 Cài đặt Git trên macOS  
### 🍎 Installing Git on macOS

### ✅ Cách 1: Dùng Homebrew (Khuyên dùng)

```bash
brew install git
```

### ✅ Cách 2: Tải trực tiếp từ trang chủ  
Vào [https://git-scm.com](https://git-scm.com) → Tải bản dành cho macOS

> ⚠ Sau khi cài, mở Terminal và kiểm tra bằng `git --version`

---

### ✅ Option 1: Using Homebrew (Recommended)

```bash
brew install git
```

### ✅ Option 2: Download from Website  
Visit [https://git-scm.com](https://git-scm.com) → Download the macOS version

> ⚠ After installing, open Terminal and check with `git --version`

---

## 🐧 Cài đặt Git trên Linux  
### 🐧 Installing Git on Linux

### ✅ Ubuntu/Debian:

```bash
sudo apt update
sudo apt install git
```

### ✅ Fedora:

```bash
sudo dnf install git
```

> ✅ Kiểm tra lại bằng `git --version`

---

### ✅ Ubuntu/Debian:

```bash
sudo apt update
sudo apt install git
```

### ✅ Fedora:

```bash
sudo dnf install git
```

> ✅ Check with `git --version`

---

## 🛠 Sau khi cài xong  
### 🛠 After Installation

Bạn nên cấu hình Git với thông tin của bạn:

```bash
git config --global user.name "Tên của bạn"
git config --global user.email "email@example.com"
```

---

You should configure Git with your name and email:

```bash
git config --global user.name "Your Name"
git config --global user.email "email@example.com"
```

---

## 🎯 Tổng kết  
### 🎯 Summary

- ✅ Cài Git trên mọi hệ điều hành đều dễ dàng  
- 🧠 Đừng quên cấu hình tên và email để Git ghi nhận tác giả commit

> 👉 Giờ bạn đã sẵn sàng để bắt đầu học Git từ những lệnh cơ bản!

---