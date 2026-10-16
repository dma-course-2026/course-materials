# CẨM NANG PYTHON TOÀN TẬP

**CHƯƠNG – 1 | Trang – 4/5**

## 3. TOÁN TỬ TRONG PYTHON

### ★ Toán tử (Operator) là gì?

Operator là một ký hiệu thực hiện một phép toán trên một hoặc nhiều toán hạng (operand/giá trị).

**Ví dụ:** `a + b`, `x * y`, `a > b`

**Các loại Operator**

1. Toán tử số học (Arithmetic)
2. Toán tử so sánh (Comparison)
3. Toán tử logic (Logical)
4. Toán tử gán (Assignment)
5. Toán tử định danh (Identity)
6. Toán tử thành viên (Membership)
7. Toán tử bitwise (Bitwise)

> **Note:** Operator dùng để thực hiện các phép toán.

### ★ 1. Toán tử số học (Arithmetic Operators)

| Toán tử | Tên | Ví dụ | Ý nghĩa |
|---|---|---|---|
| `+` | Cộng | `x + y` | Cộng hai giá trị |
| `-` | Trừ | `x - y` | Lấy x trừ y |
| `*` | Nhân | `x * y` | Nhân hai giá trị |
| `/` | Chia | `x / y` | Chia x cho y (kết quả float) |
| `//` | Chia lấy nguyên | `x // y` | Chia và lấy phần nguyên |
| `%` | Chia lấy dư | `x % y` | Phần dư của phép chia |
| `**` | Lũy thừa | `x ** y` | x lũy thừa y |

**Ví dụ:**

```python
a = 10
b = 3
print(a + b)    # 13
print(a - b)    # 7
print(a * b)    # 30
print(a / b)    # 3.333...
print(a // b)   # 3
print(a % b)    # 1
print(a ** b)   # 1000
```

### ★ 2. Toán tử so sánh (Comparison / Relational Operators)

| Toán tử | Tên | Ví dụ | Ý nghĩa |
|---|---|---|---|
| `==` | Bằng | `a == b` | True nếu a bằng b |
| `!=` | Khác | `a != b` | True nếu a khác b |
| `>` | Lớn hơn | `a > b` | True nếu a lớn hơn b |
| `<` | Nhỏ hơn | `a < b` | True nếu a nhỏ hơn b |
| `>=` | Lớn hơn hoặc bằng | `a >= b` | True nếu a ≥ b |
| `<=` | Nhỏ hơn hoặc bằng | `a <= b` | True nếu a ≤ b |

**Ví dụ:**

```python
a = 10
b = 5
print(a == b)   # False
print(a != b)   # True
print(a > b)    # True
print(a < b)    # False
print(a >= b)   # True
print(a <= b)   # False
```

### ★ 3. Toán tử logic (Logical Operators)

| Toán tử | Tên | Ví dụ | Ý nghĩa |
|---|---|---|---|
| `and` | Logical AND | `x and y` | True nếu cả x và y đều True |
| `or` | Logical OR | `x or y` | True nếu x hoặc y là True |
| `not` | Logical NOT | `not x` | True nếu x là False |

**Ví dụ:**

```python
x = True, y = False
print(x and y)  # False
print(x or y)   # True
print(not x)    # False
```

### ★ 4. Toán tử gán (Assignment Operators)

| Toán tử | Ví dụ | Tương đương | Toán tử | Ví dụ | Tương đương |
|---|---|---|---|---|---|
| `=` | `x = 5` | `x = 5` | `/=` | `x /= 3` | `x = x / 3` |
| `+=` | `x += 3` | `x = x + 3` | `%=` | `x %= 3` | `x = x % 3` |
| `-=` | `x -= 3` | `x = x - 3` | `//=` | `x //= 3` | `x = x // 3` |
| `*=` | `x *= 3` | `x = x * 3` | `**=` | `x **= 3` | `x = x ** 3` |

**Ví dụ:**

```python
x = 10
x += 5   # x = 15
x *= 2   # x = 30
x -= 10  # x = 20
```

> Operator chính là những viên gạch cơ bản xây nên các biểu thức trong Python.
