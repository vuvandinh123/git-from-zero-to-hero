# 📝 Bài 4: Commit thay đổi và xem lịch sử với Git
## Lesson 4: Commit Changes and View History with Git

---

## 📚 Thuật ngữ | Terminology
- **Staging Area**: Vùng chứa các thay đổi trước khi commit.  
  *Staging Area*: *A zone where changes are kept before committing. * 
---

## 🎯 Mục tiêu | Objectives

- Hiểu commit là gì và cách sử dụng.  
  *Understand what a commit is and how to use it.*  
- Biết cách viết commit message đúng chuẩn.  
  *Learn how to write proper commit messages.*  
- Biết cách xem lịch sử commit.  
  *Know how to view commit history.*

---

## 📌 1. Commit là gì? | What is a Commit?

Commit là hành động lưu lại các thay đổi trong dự án.  
*A commit is an action that saves your changes in the project.*

Git sẽ ghi nhớ "ảnh chụp" (snapshot) của code tại thời điểm đó.  
*Git remembers a "snapshot" of your code at that point in time.*

---

## ✅ 2. Cách tạo commit | How to Make a Commit

```bash
git add .
git commit -m "add: implement user login page"
```

📍 Giải thích | Explanation:

- `git add .`: Thêm tất cả thay đổi vào vùng staging  ( *Add all changes to the staging area* ) 
- `git commit -m "..."`: Tạo commit với nội dung cụ thể  ( *Create a commit with a specific message* )

---

## ✍️ 3. Cách viết commit message | How to Write a Proper Commit Message

| Loại commit | Ví dụ cú pháp | Ý nghĩa |  
|-------------|----------------|--------|  
| `add:`      | `add: create signup form` | Thêm mới chức năng |  
| `fix:`      | `fix: correct typo in title` | Sửa lỗi |  
| `update:`   | `update: improve UI layout` | Cập nhật nội dung |  
| `remove:`   | `remove: delete unused file` | Xoá nội dung không dùng |  
| `refactor:` | `refactor: simplify logic` | Tối ưu code mà không thay đổi chức năng |

📝 **Tips**:

- Luôn dùng tiếng Anh cho commit message  
  *Always use English for commit messages*  
- Không viết hoa chữ đầu, không cần chấm cuối câu  
  *Don't capitalize the first letter and no period at the end *
- Message càng cụ thể càng tốt  
  *The more specific the message, the better*

---

## 📜 4. Xem lịch sử commit | Viewing Commit History

```bash
git log
```

Hiển thị danh sách commit: ai thực hiện, khi nào, và nội dung gì  
*Displays a list of commits: who made them, when, and the message*

### Xem lịch sử gọn gàng hơn | View a cleaner history

```bash
git log --oneline --graph --all
```

Giúp bạn thấy sơ đồ các nhánh và commit một cách trực quan  
*Helps you visualize branch and commit history clearly*

---

## 🎯 Tổng kết  
## 🎯 Summary

| Mục đích | Lệnh |  
|---------|------|  
| Tạo commit | `git commit -m "message"` |  
| Thêm file vào staging | `git add .` hoặc `git add file.txt` |  
| Xem lịch sử commit | `git log` |  
| Xem sơ đồ commit đẹp | `git log --oneline --graph --all` |

---

Bạn đã nắm được cách **commit** và **xem lại lịch sử Git** rồi đó!  
*You've now learned how to **commit changes** and **view Git history**!*

👉 Bài tiếp theo: **Làm việc với nhánh (branch) trong Git**