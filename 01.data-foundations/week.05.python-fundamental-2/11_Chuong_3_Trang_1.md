# CẨM NANG PYTHON TOÀN TẬP

**CHƯƠNG – 3 | Trang – 1/6**

## 3. HÀM TRONG PYTHON

### 1. Hàm (Function) là gì?

Function là một khối code thực hiện một nhiệm vụ cụ thể. Nó giúp chia một chương trình lớn thành các phần nhỏ hơn, có thể tái sử dụng.

**Vì sao cần Function?**

- Giúp code có tổ chức, dễ hiểu.
- Thúc đẩy khả năng tái sử dụng code.
- Giảm sự lặp lại.
- Cải thiện việc debug và bảo trì.

### 2. Cú pháp của Function

```python
def function_name(parameters):
    # function body
    # statements
    return value  # optional
```

- `def`: từ khóa dùng để định nghĩa function.
- `function_name`: một identifier hợp lệ bất kỳ.
- `parameters`: giá trị đầu vào (tùy chọn).
- `return`: (tùy chọn) trả giá trị về cho nơi gọi.

### 3. Các loại Function

**(a) Built-in Functions**

Đây là các hàm có sẵn trong Python.

Ví dụ: `print()`, `len()`, `type()`, `input()`, `range()`, `max()`, `min()`, `sum()` v.v.

**(b) User-defined Functions**

Đây là các hàm do người dùng tự tạo bằng từ khóa `def`.

Ví dụ: `add()`, `area()`, `factorial()` v.v.

### 4. Ví dụ: Function đơn giản

```python
def greet():
    print("Hello, chào mừng đến với Python!")
# gọi hàm
greet()
```

**Luồng thực thi:**

1. Chương trình bắt đầu.
2. `greet()` được gọi.
3. Code trong `greet()` được thực thi.
4. Luồng điều khiển quay lại dòng tiếp theo.

**Output:**

```text
Hello, chào mừng
đến với Python!
```

### 5. Function có Parameter và Return Value

```python
def add(a, b):
    sum = a + b
    return sum
x = add(5, 7)
print("Tổng là", x)
```

- `a`, `b`: parameters (đầu vào)
- `sum`: biến local
- `return sum`: trả về kết quả
- `x`: nhận giá trị được trả về

**Output:** `Tổng là 12`

### 6. Các loại Argument

| Loại | Mô tả | Ví dụ | Cách gọi |
|---|---|---|---|
| Positional Arguments | Truyền theo đúng vị trí | `def add(a, b)` | `add(2, 3)` |
| Keyword Arguments | Truyền bằng tên parameter | `def add(a, b)` | `add(b=3, a=2)` |
| Default Arguments | Parameter có giá trị mặc định | `def greet(name="User")` | `greet()` hoặc `greet("Sagar")` |
| Variable-length Arguments | Nhận số lượng argument bất kỳ | `def sum_all(*args)` | `sum_all(1,2,3,4,5)` |

### 7. Function với Default Argument

```python
def greet(name = "Guest"):
    print("Hello, ", name)
greet()          # dùng giá trị mặc định
greet("Sagar")   # dùng giá trị được truyền
```

**Output:**

```text
Hello, Guest
Hello, Sagar
```

**Tóm tắt**

- Function giúp code module hóa, tái sử dụng.
- Dùng `def` để tạo function.
- Dùng `return` để trả giá trị về.
- Function có thể có parameter và default value.
