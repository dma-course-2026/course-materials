# CẨM NANG PYTHON TOÀN TẬP

**CHƯƠNG – 3 | Trang – 2/6**

## 3. HÀM TRONG PYTHON (tiếp theo)

### 8. Function với nhiều Parameter

```python
def area(length, width):
    area = length * width
    return area
l = 10
w = 5
result = area(l, w)
print("Diện tích là", result)
```

**Điểm chính**

- Thứ tự argument phải khớp với thứ tự parameter.
- Số lượng argument phải bằng số lượng parameter.
- Argument khác nhau cho kết quả khác nhau.

### 9. Function với Default Parameter

```python
def greet(name = "Guest", msg = "Hello"):
    print(msg + ", " + name)

greet()            # dùng cả hai giá trị mặc định
greet("Alice")     # dùng msg mặc định
greet("Bob", "Hi") # không dùng giá trị mặc định nào
```

| Cách gọi | name | msg | Output |
|---|---|---|---|
| `greet()` | `"Guest"` | `"Hello"` | Hello, Guest |
| `greet("Alice")` | `"Alice"` | `"Hello"` | Hello, Alice |
| `greet("Bob", "Hi")` | `"Bob"` | `"Hi"` | Hi, Bob |

> ★ **Note:** Default parameter được dùng khi argument tương ứng không được truyền vào.

### 10. Variable-length Arguments

**(a) Dùng `*args` (Non-keyword Arguments)**

```python
def total(*nums):
    s = 0
    for n in nums:
        s = s + n
    return s
```

```text
total(1, 2, 3) → 6
total(10, 20) → 30
total() → 0
```

→ `*args` gói các positional argument thành một tuple.

**(b) Dùng `**kwargs` (Keyword Arguments)**

```python
def show(**info):
    for key, value in info.items():
        print(key, "=", value)
```

```python
show(name="Sagar", age=20)
```

```text
# name = Sagar
# age = 20
```

→ `**kwargs` gói các keyword argument thành một dictionary.

### 11. Trả về nhiều giá trị (Return Multiple Values)

```python
def operations(a, b):
    add = a + b
    sub = a - b
    mul = a * b
    return add, sub, mul

x, y, z = operations(10, 5)
print(x)  # 15
print(y)  # 5
print(z)  # 50
```

**Cách hoạt động?**

- Function trả về các giá trị dưới dạng một tuple.
- Các giá trị này có thể được unpack ra các biến riêng biệt.

### 12. Biến Local và Global

| Loại | Phạm vi | Nơi khai báo | Ví dụ | Truy cập từ đâu |
|---|---|---|---|---|
| Biến Local | Bên trong function | Trong function | `def func():`<br>&nbsp;&nbsp;&nbsp;&nbsp;`x=10 #local`<br>&nbsp;&nbsp;&nbsp;&nbsp;`print(x)` | Chỉ trong function |
| Biến Global | Toàn bộ chương trình | Ngoài mọi function | `x = 10 #global`<br>`def func():`<br>&nbsp;&nbsp;&nbsp;&nbsp;`print(x)` | Mọi nơi trong chương trình |
