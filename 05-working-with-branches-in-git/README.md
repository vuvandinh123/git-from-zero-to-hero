# 📝 Bài 5: Làm việc với nhánh (branch) trong Git  
## Lesson 5: Working with Branches in Git**

---

## 📚 Thuật ngữ | Terminology  
**Branch:** Nhánh là một dòng phát triển độc lập trong dự án.  
**Branch:** A branch is an independent line of development in a project.

---

## 🎯 Mục tiêu | Objectives  

| 🎯 Mục tiêu (Tiếng Việt) | 🎯 Objectives (English) |
|--------------------------|--------------------------|
| Hiểu nhánh là gì và vì sao nên dùng | Understand what branches are and why we use them |
| Biết cách tạo, chuyển, hợp nhất và xoá nhánh | Learn how to create, switch, merge, and delete branches |

---

## 📌 1. Nhánh là gì? | What is a Branch?  
Nhánh cho phép bạn phát triển tính năng mới, sửa lỗi mà không ảnh hưởng đến mã nguồn chính.  
*A branch allows you to develop new features or fix bugs without affecting the main codebase.*

> Git mặc định có một nhánh tên là `main` (trước đây là `master`).  
> *Git creates a default branch named `main` (formerly `master`).*

---

## ✅ 2. Tạo và chuyển nhánh | Creating and Switching Branches

```bash
git branch feature/login  
git switch feature/login
```

**Hoặc dùng lệnh rút gọn:**  
**Or use a shorter command:**

```bash
git switch -c feature/login
```

**Hoặc cách truyền thống (cũ hơn):**  
**Or the traditional (older) way:**

```bash
git checkout -b feature/login
```

---

📍 **Giải thích | Explanation**

| Lệnh (Command) | Mô tả (Description) |
|----------------|---------------------|
| `git branch <tên>` | Tạo một nhánh mới (Create a new branch) |
| `git switch <tên>` | Chuyển sang nhánh đã có (Switch to an existing branch) |
| `git switch -c <tên>` | Tạo và chuyển sang nhánh mới (Create and switch to a new branch) |
| `git checkout -b <tên>` | Tạo và chuyển sang nhánh mới (Create and switch to a new branch — old syntax) |

📌 `git switch` là cú pháp mới hơn, dễ hiểu hơn so với `git checkout`.  
📌 `git switch` is a newer and clearer syntax compared to `git checkout`.

--- 

## 🔁 3. Hợp nhất nhánh | Merging Branches  

```bash
git switch main  
git merge feature/login
```

📍 **Giải thích | Explanation**  

| Bước (Step) | Mô tả (Description) |
|-------------|---------------------|
| Chuyển về nhánh chính | Switch to main branch |
| Hợp nhất nhánh phụ | Merge feature branch |

> Nếu có xung đột, Git sẽ yêu cầu bạn giải quyết trước khi hoàn tất merge.  
> *If there's a conflict, Git will ask you to resolve it before completing the merge.*

---

## 🗑 4. Xoá nhánh | Deleting Branches  

```bash
git branch -d feature/login
```

📍 **Lưu ý | Note**  
- `-d`: Xoá nếu đã merge (Delete if already merged)  
- `-D`: Xoá mạnh tay kể cả chưa merge (Force delete even if not merged)

---

## 🗺 5. Xem danh sách nhánh | Viewing Branches  

```bash
git branch
```

Hiển thị nhánh local, nhánh hiện tại có dấu `*`  
*Shows local branches, current one marked with `*`*
```bash
git branch -a
```

Hiển thị cả nhánh local và remote  
*Shows both local and remote branches*

---

## 💡 6. Tips đặt tên nhánh | Tips for Naming Branches

| Mẫu tên (Pattern) | Ý nghĩa (Meaning) | Ví dụ (Example) |
|------------------|-------------------|-----------------|
| `feature/<tên>`  | Thêm tính năng mới (New feature) | `feature/user-login` |
| `bugfix/<tên>`   | Sửa lỗi (Bug fix) | `bugfix/login-crash` |
| `hotfix/<tên>`   | Sửa lỗi gấp trên production (Urgent fix) | `hotfix/security-patch` |
| `refactor/<tên>` | Cải tiến cấu trúc code (Refactor) | `refactor/user-service` |
| `test/<tên>`     | Viết hoặc cập nhật test (Testing) | `test/signup-form` |

📝 **Gợi ý thêm | Extra Suggestions:**
- Dùng dấu `-` thay cho khoảng trắng → `feature/user-profile`
- Tên ngắn gọn, có ý nghĩa
- Viết bằng tiếng Anh để dễ làm việc nhóm

---

## 🎯 Tổng kết | Summary

| Mục đích (Purpose) | Lệnh (Command) |
|--------------------|----------------|
| Tạo nhánh mới (Create new branch) | `git branch <name>` |
| Tạo và chuyển (Create & switch) | `git switch -c <name>` |
| Chuyển nhánh (Switch branch) | `git switch <name>` |
| Hợp nhất nhánh (Merge branch) | `git merge <name>` |
| Xoá nhánh (Delete branch) | `git branch -d <name>` |
| Xem nhánh (View branches) | `git branch` / `git branch -a` |

✅ Giờ bạn đã thành thạo làm việc với nhánh trong Git rồi đó!  
*✅ You've now mastered how to work with branches in Git!*

---

👉 **Bài tiếp theo: Làm việc với Git Remote (push, pull, clone)**  
**Next lesson: Working with Git Remote (push, pull, clone)**

---
