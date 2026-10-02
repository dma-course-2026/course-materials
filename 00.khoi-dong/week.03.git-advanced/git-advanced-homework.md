# Git Advanced Homework

Bài tập về nhà dùng để thực hành lại các nội dung Git đã demo trên lớp.

Mỗi học viên thực hiện trên **repository cá nhân** của mình.

## Mục tiêu

Hoàn thành workflow:

```text
Developer
→ Branch
→ Edit
→ Add
→ Commit
→ Push
→ Pull Request
→ Merge
→ Pull main
→ Check history
```

Ngoài ra cần thực hành:

- Feature Branch Workflow
- Pull Request
- Merge strategy
- Merge conflict
- Resolve conflict
- Kiểm tra commit history

---

## Cấu trúc bài tập

Tạo thư mục:

```text
assignments/
└── 3.git-advanced/
    ├── README.md
    ├── merge-demo.md
    └── conflict-demo.md
```

---

# Phần 1 — Developer Workflow

Từ `main` mới nhất, tạo branch:

```text
feature/git-homework
```

Tạo file:

```text
assignments/3.git-advanced/README.md
```

Nội dung mẫu:

```markdown
# Git Advanced Homework

Student: <Mã học viên> - <Họ tên>

## Goal

Practice Feature Branch Workflow and Pull Request.
```

Thực hiện ít nhất **2 commit** trên feature branch.

Ví dụ:

```text
Add Git homework
Update homework description
```

Sau đó thực hiện:

```text
Push feature branch
→ Create Pull Request
→ Review Files changed
→ Merge Pull Request
```

Pull Request:

```text
feature/git-homework → main
```

Sau khi merge:

```bash
git switch main
git pull origin main
```

Kết quả cần hiểu:

```text
Local feature branch
→ Remote feature branch
→ Pull Request
→ main
```


---

# Phần 2 — Merge Conflict

## Bước 1 — Chuẩn bị

Trên `main`, tạo:

```text
assignments/3.git-advanced/conflict-demo.md
```

Nội dung ban đầu:

```text
Status: Draft
```

Commit và đưa file vào `main`.

## Bước 2 — Tạo hai branch

Từ cùng một trạng thái `main`, tạo:

```text
feature/status-a
feature/status-b
```

Mental model:

```text
                    feature/status-a
                   /
main -------------
                   \
                    feature/status-b
```

## Bước 3 — Branch A

Trên `feature/status-a`, sửa:

```text
Status: Draft
```

thành:

```text
Status: Ready
```

Commit, push và tạo PR:

```text
feature/status-a → main
```

Merge PR này trước.

## Bước 4 — Branch B

Branch `feature/status-b` vẫn được tạo từ trạng thái cũ:

```text
Status: Draft
```

Sửa thành:

```text
Status: In Progress
```

Commit, push và tạo PR:

```text
feature/status-b → main
```

Lúc này `main` đã có:

```text
Status: Ready
```

trong khi feature branch có:

```text
Status: In Progress
```

GitHub dự kiến sẽ báo:

```text
Can't automatically merge
```

---

# Phần 3 — Resolve Conflict trên local

Chuyển về branch:

```bash
git switch feature/status-b
```

Cập nhật remote:

```bash
git fetch origin
```

Đưa `main` mới nhất vào feature branch:

```bash
git merge origin/main
```

Kiểm tra:

```bash
git status
```

File có thể xuất hiện:

```text
<<<<<<< HEAD
Status: In Progress
=======
Status: Ready
>>>>>>> origin/main
```

Resolve thành nội dung cuối cùng:

```text
Status: Ready for Review
```

Xóa toàn bộ conflict markers rồi:

```bash
git add assignments/3.git-advanced/conflict-demo.md
git commit -m "Resolve status conflict with main"
git push
```

Pull Request cũ sẽ tự động cập nhật.

**Không tạo Pull Request mới.**

Sau khi PR không còn conflict, merge PR vào `main`.

---



# Phần 4 — Cập nhật kết quả vào README

Trong:

```text
assignments/3.git-advanced/README.md
```

bổ sung:

```markdown
## Kết quả

- Feature workflow PR: <link>
- Merge demo PR: <link>
- Conflict PR A: <link>
- Conflict PR B: <link>

## Commands đã thực hành

- git switch
- git status
- git diff
- git add
- git commit
- git push
- git pull
- git fetch
- git merge
- git log
```


# Flow cần nhớ

```text
main
 ↓
create feature branch
 ↓
edit
 ↓
git add
 ↓
git commit
 ↓
git push
 ↓
Pull Request
 ↓
review / resolve conflict nếu có
 ↓
merge
 ↓
pull main
```

Mục tiêu của bài tập là hiểu:

```text
Branch nào đang làm việc?
Code đang ở local hay remote?
Commit đã được push chưa?
Pull Request đang đưa branch nào vào branch nào?
Khi main thay đổi thì feature branch cần đồng bộ như thế nào?
Conflict xảy ra ở đâu và ai quyết định nội dung cuối cùng?
```
