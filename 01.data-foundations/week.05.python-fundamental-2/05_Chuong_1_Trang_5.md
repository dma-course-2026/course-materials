# CẨM NANG PYTHON TOÀN TẬP

**CHƯƠNG – 1 | Trang – 5/5**

## 5. ÉP KIỂU VÀ NHẬP DỮ LIỆU NGƯỜI DÙNG

### ★ Ép kiểu (Type Casting)

Type casting là việc chuyển đổi một kiểu dữ liệu này sang kiểu dữ liệu khác. Python có hai loại ép kiểu:

1. **Ép kiểu ngầm định (Implicit – Tự động)**
2. **Ép kiểu tường minh (Explicit – Thủ công)**

**Ép kiểu ngầm định (Tự động)**

| Ví dụ | Giải thích | Kết quả |
|---|---|---|
| `x = 10`<br>`y = 3.5` | int + float → float | `13.5` |
| `x = 5`<br>`y = 2+3j` | int + complex → complex | `(5+3j)` |
| `x = True` | bool được chuyển sang int (1) | `1` |

**Ép kiểu tường minh (Thủ công)**

| Hàm | Mô tả | Ví dụ |
|---|---|---|
| `int()` | Chuyển sang integer | `int(3.14)` → `3` |
| `float()` | Chuyển sang float | `float(10)` → `10.0` |
| `str()` | Chuyển sang string | `str(25)` → `"25"` |
| `bool()` | Chuyển sang boolean | `bool(0)` → `False` |
| `complex()` | Chuyển sang complex | `complex(5)` → `(5+0j)` |

**★ Ví dụ ép kiểu**

```python
int(10.9)   # 10
float(7)    # 7.0
str(100)    # '100'
bool(5)     # True
bool(0)     # False
complex(8)  # (8+0j)
```

> **Note:** Cần ép kiểu tường minh khi Python không tự biết cách chuyển đổi.

### ★ Nhập dữ liệu từ người dùng trong Python

Python có hàm **`input()`** để nhận dữ liệu người dùng nhập vào.

| Hàm | Mô tả | Ví dụ | Output (nếu nhập 25) | Data Type |
|---|---|---|---|---|
| `input()` | Luôn trả về string | `name = input("Nhập tên: ")`<br>`print(name)` | `Nhập tên: Sagar`<br>`Sagar` | `str` |
| `int(input())` | Chuyển input sang integer | `age = int(input("Nhập tuổi: "))`<br>`print(age)` | `Nhập tuổi: 25`<br>`25` | `int` |
| `float(input())` | Chuyển input sang float | `price = float(input("Nhập giá: "))`<br>`print(price)` | `Nhập giá: 12.75`<br>`12.75` | `float` |

### ★ Ví dụ thực hành

**1. Nhập hai số từ người dùng và in tổng.**

```python
a = int(input("Nhập số thứ nhất: "))
b = int(input("Nhập số thứ hai: "))
print("Tổng =", a + b)
```

**2. Nhập bán kính và tính diện tích hình tròn.**

```python
r = float(input("Nhập bán kính: "))
area = 3.14 * r * r
print("Diện tích =", area)
```

**3. Nhập tên và in độ dài của tên.**

```python
name = input("Nhập tên: ")
print("Độ dài =", len(name))
```

**Điểm quan trọng**

- Tất cả biến phải khai báo trước khi dùng.
- Python phân biệt hoa – thường.
- Dùng tên biến rõ nghĩa.
- Chọn đúng kiểu dữ liệu để tiết kiệm bộ nhớ.
- Dùng ép kiểu khi cần thiết.
- Luôn xử lý dữ liệu nhập vào cẩn thận.

> Nắm vững operator, ép kiểu và input chính là nền tảng của lập trình Python.
