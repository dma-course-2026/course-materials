# CẨM NANG PYTHON TOÀN TẬP

**CHƯƠNG – 3 | Trang – 6/6**

## 3. HÀM TRONG PYTHON (tiếp theo)

### 28. Function vs Method

| Khía cạnh | Function | Method |
|---|---|---|
| Thuộc về | Độc lập, không gắn với object hay class nào. | Thuộc về một object hoặc class. |
| Cú pháp gọi | `function_name(args)` | `object.method(args)` |
| Parameter đầu tiên | Không có gì đặc biệt. | Nếu user-defined, tham số đầu thường là `self`. |
| Ví dụ | `print()`, `len()`, `max()` | `"hello".upper()`, `list.append()` |
| Mục đích | Thực hiện tác vụ chung. | Thao tác trên dữ liệu của object. |

**Ghi nhớ**

- Function độc lập.
- Method được gọi trên object.
- Mọi thứ trong Python đều là object, kể cả function!

### 29. Module và Built-in Functions

**(a) Module Functions**

Module cung cấp nhiều function hữu ích. Import module rồi dùng function của nó.

```python
import math  # Import module math
print(math.sqrt(16))  # 4.0
print(math.pi)        # 3.141592653589793
print(math.factorial(5))  # 120
```

**(b) Built-in Functions**

Luôn có sẵn trong Python. Không cần import.

```python
abs(-7)           # 7
round(3.567, 2)  # 3.57
sorted([3,1,2])  # [1,2,3]
sum([1,2,3,4])   # 10
type(123)        # <class 'int'>
```

### 30. Phạm vi biến trong Function (Variable Scope)

| Phạm vi | Truy cập được ở đâu | Ví dụ | Output / Ghi chú |
|---|---|---|---|
| Local Scope | Chỉ trong function | `def f():`<br>&nbsp;&nbsp;&nbsp;&nbsp;`x=10 #local`<br>&nbsp;&nbsp;&nbsp;&nbsp;`print(x)` | Lỗi: x không được định nghĩa bên ngoài function. |
| Global Scope | Toàn bộ chương trình | `x=20 #global`<br>`def f():`<br>&nbsp;&nbsp;&nbsp;&nbsp;`print(x)` | `20` (dùng x global) |
| Enclosing Scope | Bên trong nested function | `def outer():`<br>&nbsp;&nbsp;&nbsp;&nbsp;`y=5`<br>&nbsp;&nbsp;&nbsp;&nbsp;`def inner():`<br>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;`print(y)`<br>&nbsp;&nbsp;&nbsp;&nbsp;`inner()` | `5` (inner truy cập được y) |
| Built-in Scope | Các tên có sẵn của Python | `print(len([1,2,3]))` | `3` (len là built-in) |

★ Quy tắc LEGB: Python tìm biến theo thứ tự: **L–Local → E–Enclosing → G–Global → B–Built-in**.

### 31. Nâng cao: Function Annotations và Docstrings

**(a) Function Annotations (Type Hints)**

```python
def add(a: int, b: int) -> int:
    """Trả về tổng hai số nguyên."""
    return a + b
result: int = add(4, 5)
```

**Note:** Python không ép buộc kiểu dữ liệu, nhưng công cụ có thể kiểm tra.

**(b) Docstrings**

```python
def greet(name: str) -> str:
    """Chào người dùng theo tên.
    Trả về một chuỗi lời chào."""
    return f"Hello, {name}!"
```

```python
print(greet.__doc__)  # in docstring
help(greet)           # hiển trong help()
```

### 32. Ví dụ thực hành

**1. Kiểm tra chẵn/lẻ**

```python
def is_even(n: int) -> bool:
    """True nếu n chẵn."""
    return n % 2 == 0
```

**2. Hàm lũy thừa**

```python
def power(base, exp: int) -> int:
    result = 1
    for _ in range(exp):
        result *= base
    return result
```

**3. Đảo ngược chuỗi**

```python
def reverse_text(text: str) -> str:
    """Trả về chuỗi bị đảo ngược."""
    return text[::-1]
```

> Function rất mạnh mẽ. Dùng chúng thật khôn ngoan. Code thông minh, code sạch, code đúng Python!
