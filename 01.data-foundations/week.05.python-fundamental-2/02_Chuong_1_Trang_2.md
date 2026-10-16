# CẨM NANG PYTHON TOÀN TẬP

**CHƯƠNG – 1 | Trang – 2/5**

## 1. GIỚI THIỆU VỀ PYTHON

### ★ Cú pháp Python (Python Syntax)

- Python syntax là tập hợp các quy tắc quy định cách một chương trình Python được viết.
- Python có **cú pháp đơn giản, dễ hiểu**, gần giống tiếng Anh.
- Python **phân biệt chữ hoa – chữ thường** (case-sensitive).

**Ví dụ:**

```python
# Đây là comment
print("Hello, Python!")
x = 10
y = 20
sum = x + y       # output
print(sum)        # 30
```

### ★ Định danh trong Python (Identifiers)

- Identifier dùng để đặt tên cho biến, hàm, class, v.v.
- Một identifier có thể chứa **chữ cái (a-z, A-Z)**, **chữ số (0-9)** và **dấu gạch dưới (_)**.
- Không được bắt đầu bằng chữ số.
- Không được chứa ký tự đặc biệt ngoại trừ `_`.
- Không được dùng từ khóa (keyword) của Python làm identifier.

| Hợp lệ ✓ | Không hợp lệ ✗ |
|---|---|
| `myVar` | `1name` (bắt đầu bằng số) |
| `_value` | `my-var` (chứa `-`) |
| `total_sum` | `total sum` (chứa khoảng trắng) |
| `Name123` | `@value` (chứa ký tự đặc biệt) |
| `var_1` | `for` (keyword) |

### ★ Các kiểu dữ liệu có sẵn (Built-in Data Types)

| Data Type | Mô tả | Ví dụ |
|---|---|---|
| `int` | Số nguyên (whole numbers) | `x = 10` |
| `float` | Số thập phân | `pi = 3.14` |
| `str` | Chuỗi (text) | `name = "Python"` |
| `bool` | Giá trị Boolean (True/False) | `is_active = True` |
| `list` | Tập hợp có thứ tự, có thể thay đổi | `nums = [1,2,3]` |
| `tuple` | Tập hợp có thứ tự, không thể thay đổi | `t = (1,2,3)` |
| `dict` | Cặp key – value | `d = {"a": 1, "b": 2}` |

> **Note:** Chúng ta sẽ tìm hiểu chi tiết tất cả các kiểu dữ liệu này ở những chương sau.

### ★ Toán tử cơ bản (Basic Operators)

**Toán tử số học**

| Toán tử | Ý nghĩa |
|---|---|
| `+` | Cộng (Addition) |
| `-` | Trừ (Subtraction) |
| `*` | Nhân (Multiplication) |
| `/` | Chia (Division) |
| `//` | Chia lấy nguyên (Floor Division) |
| `%` | Chia lấy dư (Modulus) |
| `**` | Lũy thừa (Exponent) |

**Toán tử so sánh**

| Toán tử | Ý nghĩa |
|---|---|
| `==` | Bằng |
| `!=` | Khác |
| `>` | Lớn hơn |
| `<` | Nhỏ hơn |
| `>=` | Lớn hơn hoặc bằng |
| `<=` | Nhỏ hơn hoặc bằng |

**Toán tử Logic**

| Toán tử | Ý nghĩa |
|---|---|
| `and` | Logical AND |
| `or` | Logical OR |
| `not` | Logical NOT |

**Toán tử gán**

| Toán tử | Ý nghĩa |
|---|---|
| `=` | Gán |
| `+=` | Cộng và gán |
| `-=` | Trừ và gán |
| `*=` | Nhân và gán |
| `/=` | Chia và gán |
| `%=` | Chia dư và gán |
