# CẨM NANG PYTHON TOÀN TẬP

**CHƯƠNG – 2 | Trang – 3/5**

## 2. CÁC CÂU LỆNH ĐIỀU KHIỂN LUỒNG (tiếp theo)

### ★ 4. Câu lệnh lồng nhau (Nested Statements)

Một câu lệnh nằm bên trong câu lệnh khác được gọi là nested statement.

```python
x = 10
if x > 0:
    if x % 2 == 0:
        print("Số dương chẵn")
    else:
        print("Số dương lẻ")
```

**Output:** Số dương chẵn

**Tại sao Control Flow quan trọng?**

- Điều khiển luồng thực thi.
- Hỗ trợ ra quyết định.
- Cho phép lặp lại và tự động hóa.
- Giúp chương trình linh hoạt và thông minh hơn.

### ★ Ví dụ toán tử quan hệ

| Biểu thức | Toán tử | Ý nghĩa | Ví dụ | Kết quả |
|---|---|---|---|---|
| `a == b` | `==` | Bằng | `5 == 5` | True |
| `a != b` | `!=` | Khác | `5 != 3` | True |
| `a > b` | `>` | Lớn hơn | `7 > 4` | True |
| `a < b` | `<` | Nhỏ hơn | `2 < 9` | True |
| `a >= b` | `>=` | Lớn hơn hoặc bằng | `6 >= 6` | True |
| `a <= b` | `<=` | Nhỏ hơn hoặc bằng | `3 <= 5` | True |

### ★ Ví dụ toán tử logic

| Biểu thức | Toán tử | Ý nghĩa | Ví dụ | Kết quả |
|---|---|---|---|---|
| `x and y` | `and` | True nếu cả hai đều True | `True and False` | False |
| `x or y` | `or` | True nếu một trong hai True | `True or False` | True |
| `not x` | `not` | Đảo ngược kết quả | `not True` | False |

### ★ Ví dụ thực hành

**1. Kiểm tra số dương, âm hay bằng 0.**

```python
n = int(input("Nhập số: "))
if n > 0:
    print("Dương")
elif n < 0:
    print("Âm")
else:
    print("Bằng 0")
```

*Thử với: 5, -3, 0.*

**2. Kiểm tra số chẵn hay lẻ.**

```python
n = int(input("Nhập số: "))
if n % 2 == 0:
    print("Chẵn")
else:
    print("Lẻ")
```

*Thử với: 4, 7.*

**3. Tìm số lớn nhất trong 3 số.**

```python
a = int(input("Nhập a: "))
b = int(input("Nhập b: "))
c = int(input("Nhập c: "))
if a >= b and a >= c:
    print("Lớn nhất là", a)
elif b >= c:
    print("Lớn nhất là", b)
else:
    print("Lớn nhất là", c)
```

*Thử với: 10, 20, 15.*

**Note:**

- Thụt lề là bắt buộc trong Python.
- Dùng tên biến rõ nghĩa.
- Luôn kiểm tra điều kiện với nhiều dữ liệu đầu vào khác nhau.

### ★ Tóm tắt Control Flow

| Câu lệnh | Mục đích |
|---|---|
| `if` | Thực thi khối nếu điều kiện True |
| `if-else` | Thực thi 1 trong 2 khối |
| `elif` | Kiểm tra nhiều điều kiện |
| `nested if` | Điều kiện lồng trong điều kiện khác |
| `loops` | Lặp lại khối code |
| `jump statements` | Thay đổi luồng thực thi |
