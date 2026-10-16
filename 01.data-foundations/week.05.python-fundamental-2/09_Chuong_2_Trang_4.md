# CẨM NANG PYTHON TOÀN TẬP

**CHƯƠNG – 2 | Trang – 4/5**

## 2. CÁC CÂU LỆNH ĐIỀU KHIỂN LUỒNG (tiếp theo)

### ★ 5. Câu lệnh pass

`pass` là một toán tử rỗng (null operation). Nó không làm gì cả, dùng làm placeholder cho code trong tương lai.

```python
for i in range(5):
    pass
print("Loop kết thúc")
```

**Output:** Loop kết thúc

**Khi nào dùng pass?**

- Khi đang viết loop, function hoặc class và muốn triển khai sau.
- Khi cú pháp yêu cầu một câu lệnh nhưng bạn chưa muốn thực thi gì cả.

### ★ 6. Mệnh đề else với Loop

Python cho phép dùng `else` với `for` và `while` loop. Khối `else` chạy khi loop hoàn tất bình thường (không có `break`).

**a) else với for loop**

```python
for i in range(3):
    print(i)
else:
    print("For loop hoàn tất")
```

**Output:**

```text
0 1 2
For loop hoàn tất
```

**b) else với while loop**

```python
i = 1
while i <= 3:
    print(i)
    i = i + 1
else:
    print("While loop hoàn tất")
```

**Output:**

```text
1 2 3
While loop hoàn tất
```

**Note:** Nếu câu lệnh `break` được thực thi, khối `else` sẽ không chạy.

| Loop hoàn tất bình thường | Loop bị dừng bởi break |
|---|---|
| `for i in range(3):`<br>&nbsp;&nbsp;&nbsp;&nbsp;`print(i)`<br>`else:`<br>&nbsp;&nbsp;&nbsp;&nbsp;`print("Else chạy")`<br>`# Output: 0 1 2`<br>`Else chạy` | `for i in range(3):`<br>&nbsp;&nbsp;&nbsp;&nbsp;`if i == 1:`<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`break`<br>&nbsp;&nbsp;&nbsp;&nbsp;`print(i)`<br>`else:`<br>&nbsp;&nbsp;&nbsp;&nbsp;`print("Else không chạy")`<br>`# Output: 0` |

### ★ Ví dụ Control Flow lồng nhau

```python
for i in range(1,4):
    if i % 2 == 0:
        print(i, "là số chẵn")
    else:
        print(i, "là số lẻ")
```

**Output:**

```text
1 là số lẻ
2 là số chẵn
3 là số lẻ
```

**Điểm cần nhớ**

- Control flow quyết định thứ tự thực thi.
- Dùng `if`, `elif`, `else` để ra quyết định.
- Dùng loop (`for`, `while`) để lặp lại.
- `break`, `continue`, `pass` giúp điều khiển loop.
- `else` với loop chỉ chạy khi loop hoàn tất bình thường.

**Tóm tắt**

- `if`, `elif`, `else` → Ra quyết định
- `for`, `while` → Lặp lại
- `break` → Thoát loop
- `continue` → Bỏ qua vòng hiện tại
- `pass` → Không làm gì (placeholder)
- `else` với loop → Chạy khi loop hoàn tất bình thường
