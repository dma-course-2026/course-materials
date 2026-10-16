# CẨM NANG PYTHON TOÀN TẬP

**CHƯƠNG – 2 | Trang – 1/5**

## 2. CÁC CÂU LỆNH ĐIỀU KHIỂN LUỒNG

### ★ Control Flow là gì?

Control Flow xác định thứ tự thực thi các câu lệnh trong một chương trình. Python cung cấp nhiều câu lệnh control flow khác nhau để đưa ra quyết định và lặp lại hành động.

**Các loại Control Flow Statements**

1. Câu lệnh điều kiện (Conditional): `if`, `if-else`, `if-elif-else`
2. Câu lệnh lặp (Looping): `for loop`, `while loop`
3. Câu lệnh nhảy (Jump): `break`, `continue`, `pass`

### ★ 1. Câu lệnh điều kiện (Conditional Statements)

Dùng để đưa ra quyết định dựa trên điều kiện.

**a) Câu lệnh if**

→ Thực thi một khối code nếu điều kiện là True.

```python
x = 10
if x > 5:
    print("x lớn hơn 5")
```

**Output:** `x lớn hơn 5`

**b) Câu lệnh if-else**

→ Thực thi một khối nếu True, khối còn lại nếu False.

```python
x = 3
if x > 5:
    print("x lớn hơn 5")
else:
    print("x không lớn hơn 5")
```

**Output:** `x không lớn hơn 5`

**c) Câu lệnh if-elif-else**

→ Dùng khi có nhiều điều kiện cần kiểm tra.

```python
marks = 75
if marks >= 90:
    print("Điểm: A")
elif marks >= 60:
    print("Điểm: B")
elif marks >= 40:
    print("Điểm: C")
else:
    print("Điểm: Rớt")
```

**Output:** `Điểm: B`

### ★ Toán tử quan hệ (điều kiện)

| Toán tử | Ý nghĩa |
|---|---|
| `==` | Bằng |
| `!=` | Khác |
| `>` | Lớn hơn |
| `<` | Nhỏ hơn |
| `>=` | Lớn hơn hoặc bằng |
| `<=` | Nhỏ hơn hoặc bằng |

### ★ Toán tử logic

| Toán tử | Ý nghĩa |
|---|---|
| `and` | True nếu cả hai điều kiện đều True |
| `or` | True nếu một trong hai điều kiện là True |
| `not` | Đảo ngược kết quả, True thành False |

**Ví dụ:**

```text
x > 5 and y < 10  # True nếu cả hai điều True
x > 5 or y < 10   # True nếu một trong hai True
not(x > 5)        # True nếu điều kiện False
```

**Điểm chính**

- Dùng `if`, `else` để đưa ra quyết định.
- Dùng `elif` cho nhiều điều kiện.
- Thụt lề (indentation) rất quan trọng trong Python.
- Control flow giúp viết chương trình thông minh.

> Control flow chính là trái tim của mọi chương trình.
