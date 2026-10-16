# CẨM NANG PYTHON TOÀN TẬP

**CHƯƠNG – 1 | Trang – 3/5**

## 2. BIẾN VÀ KIỂU DỮ LIỆU

### ★ Biến (Variable) là gì?

Một biến (variable) là tên được đặt cho một vùng nhớ trong chương trình. Nó được dùng để lưu trữ dữ liệu. Python **không có lệnh khai báo biến riêng**.

**Ví dụ:**

```python
x = 10             # integer
name = "Sagar"     # string
price = 25.5       # float
is_active = True   # boolean
```

> **Note:** Không cần khai báo kiểu dữ liệu trong Python.

### ★ Các kiểu dữ liệu trong Python

| Data Type | Mô tả | Ví dụ |
|---|---|---|
| `int` | Số nguyên | `x = 10` |
| `float` | Số thập phân | `pi = 3.14` |
| `str` | Chuỗi (text) | `name = "Python"` |
| `bool` | Boolean (True/False) | `is_active = True` |
| `list` | Tập hợp có thứ tự, thay đổi được | `nums = [1,2,3,4]` |
| `tuple` | Tập hợp có thứ tự, không thay đổi được | `t = (1,2,3)` |
| `dict` | Cặp Key – Value | `d = {"a":1,"b":2}` |
| `set` | Tập hợp không thứ tự, phần tử duy nhất | `s = {1,2,3}` |

**Kiểm tra kiểu dữ liệu:**

```python
x = 100
print(type(x))   # <class 'int'>

name = "Hello"
print(type(name))  # <class 'str'>

val = 3.14
print(type(val))   # <class 'float'>
```

### ★ Ép kiểu dữ liệu (Type Conversion)

Ta có thể chuyển đổi kiểu dữ liệu này sang kiểu dữ liệu khác.

| `int()` | `float()` | `str()` | `list()` | `tuple()` | `set()` |
|---|---|---|---|---|---|
| `x = "10"` | `x = "3.14"` | `x = 25` | `x = (1,2,3)` | `x = [1,2,3]` | `x = [1,2,2,3]` |
| `y = int(x)` | `y = float(x)` | `y = str(x)` | `y = list(x)` | `y = tuple(x)` | `y = set(x)` |
| `print(y) # 10` | `print(y) # 3.14` | `print(y) # 25` | `print(y) # [1,2,3]` | `print(y) # (1,2,3)` | `print(y) # {1,2,3}` |

### ★ Nhập dữ liệu từ người dùng (Input)

Ta có thể lấy dữ liệu người dùng nhập vào bằng hàm **`input()`**.

```python
name = input("Nhập tên: ")   # input luôn trả về string
age = int(input("Nhập tuổi: "))  # chuyển sang số nguyên
print("Tên:", name)
print("Tuổi:", age)
```

**Quan trọng:**

- `input()` luôn trả về string.
- Dùng type conversion khi cần.
- Biến trong Python phân biệt hoa – thường.

> Biến là nơi lưu trữ dữ liệu, còn kiểu dữ liệu xác định loại dữ liệu đó.
