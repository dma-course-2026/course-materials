# CẨM NANG PYTHON TOÀN TẬP

**CHƯƠNG – 3 | Trang – 4/6**

## 3. HÀM TRONG PYTHON (tiếp theo)

### 18. Docstring trong Function

```python
def add(a, b):
    """Hàm này trả về
    tổng của hai số."""
    return a + b
```

**Truy cập docstring:**

- `add.__doc__`
- `help(add)`

**Vì sao cần Docstring?**

- Mô tả chức năng của function.
- Cải thiện khả năng đọc hiểu và tài liệu hóa.
- Hữu ích với `help()` và các công cụ khác.
- Là thói quen tốt để viết code sạch.

### 19. Positional, Default và Keyword Arguments

| Loại | Định nghĩa | Ví dụ | Cách gọi | Output |
|---|---|---|---|---|
| Positional Arguments | Truyền theo đúng thứ tự parameter. | `def sub(a,b):`<br>&nbsp;&nbsp;&nbsp;&nbsp;`return a-b` | `sub(10,4)` | `6` |
| Default Arguments | Parameter có giá trị mặc định, dùng khi không truyền. | `def greet(name="Guest"):`<br>&nbsp;&nbsp;&nbsp;&nbsp;`return "Hello "+name` | `greet()` | `Hello Guest` |
| Keyword Arguments | Truyền bằng tên parameter, không quan trọng thứ tự. | `def info(name,age):`<br>&nbsp;&nbsp;&nbsp;&nbsp;`return name, age` | `info(age=20,name="Riya")` | `('Riya', 20)` |
| Mixed (Positional + Keyword) | Positional trước, keyword sau. | `def power(x,y=2):`<br>&nbsp;&nbsp;&nbsp;&nbsp;`return x**y` | `power(3,y=4)` | `81` |

### 20. `*args` và `**kwargs` chi tiết

**(a) `*args` (Non-keyword Variable-length Arguments)**

```python
def total(*nums):
    s = 0
    for n in nums:
        s += n
    return s
```

```text
total(1,2,3) → 6
total(10,20,30,40) → 100
total() → 0
```

`*args` gói các positional argument dư thành một tuple.

**(b) `**kwargs` (Keyword Variable-length Arguments)**

```python
def show(**info):
    for k, v in info.items():
        print(k, "=", v)
```

```python
show(name="Aman", age=19)
```

```text
name = Aman
age = 19
```

`**kwargs` gói các keyword argument dư thành một dictionary.

### 21. Câu lệnh return

```python
def square(x):
    return x * x
def no_return():
    print("Function này không có return.")
```

- `return` thoát khỏi function và trả giá trị về.
- Nếu không dùng `return`, `None` sẽ được trả về mặc định.
- `return` có thể trả về bất kỳ kiểu dữ liệu nào.

**Ví dụ:**

1. `return 10`  # integer
2. `return 3.14`  # float
3. `return "Hello"`  # string
4. `return [1,2,3]`  # list
5. `return True`  # boolean

### 22. Function lồng nhau (Nested và Inner Functions)

**(a) Nested Function (Function trong function)**

```python
def outer(msg):
    def inner():
        print(msg)
    inner()
outer("Hello từ nested function")
```

**Output:** Hello từ nested function

**(b) Inner Function (Encapsulation)**

```python
def counter():
    count = 0   # biến nonlocal
    def inc():
        nonlocal count
        count += 1
        return count
    return inc

c = counter()
print(c())  # 1
print(c())  # 2
```
