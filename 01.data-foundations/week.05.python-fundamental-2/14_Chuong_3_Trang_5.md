# CẨM NANG PYTHON TOÀN TẬP

**CHƯƠNG – 3 | Trang – 5/6**

## 3. HÀM TRONG PYTHON (tiếp theo)

### 23. Câu lệnh pass trong Function

```python
def todo():
    pass  # code function sẽ được viết sau
print("Cần hoàn thành...")
```

**Vì sao dùng pass?**

- Đóng vai trò placeholder.
- Tránh lỗi thụt lề.
- Hữu ích trong quá trình phát triển.

### 24. Hàm Lambda (Anonymous Functions)

Lambda tạo các function ẩn danh nhỏ, chỉ gồm một biểu thức duy nhất.

**Cú pháp:**

```python
lambda arguments: expression
```

**Ví dụ:**

```python
add = lambda a, b: a + b
square = lambda x: x * x
max2 = lambda a, b: a if a>b else b
```

**Dùng Lambda:**

```text
>>> add(4, 5) → 9
>>> square(6) → 36
>>> max2(10, 20) → 20
```

★ Lambda phù hợp nhất cho các tác vụ nhỏ, đơn giản, chỉ dùng một lần.

### 25. Map, Filter và Reduce

| Function | Mục đích | Cú pháp | Ví dụ | Output |
|---|---|---|---|---|
| `map()` | Áp dụng function lên mọi phần tử của iterable. | `map(function, iterable)` | `list(map(lambda x: x*2, [1,2,3]))` | `[2,4,6]` |
| `filter()` | Lọc phần tử bằng function trả về True. | `filter(function, iterable)` | `list(filter(lambda x: x%2==0, [1,2,3,4,5,6]))` | `[2,4,6]` |
| `reduce()` | Kết gộp iterable về một giá trị duy nhất. | `from functools import reduce`<br>`reduce(function, iterable)` | `reduce(lambda x,y: x+y, [1,2,3,4])` | `10` |

★ `reduce()` nằm trong module `functools`.

### 26. Docstring trong Function

```python
def area(r):
    """Hàm này tính
    diện tích hình tròn."""
    return 3.14 * r * r
print(area.__doc__)
```

**Quy tắc Docstring**

- Dùng triple quotes (`""" """`).
- Là câu lệnh đầu tiên trong function.
- Mô tả chức năng của function.
- Truy cập bằng `__doc__`.

**Output:**

```text
Hàm này tính
diện tích hình tròn.
```

### 27. Thực hành tốt với Function

- Dùng tên function rõ nghĩa.
- Giữ function ngắn gọn và tập trung.
- Dùng parameter thay vì biến global.
- Trả về giá trị thay vì print (khi có thể).
- Viết docstring để làm rõ chức năng.
- Tránh side effect trong function.
- Kiểm thử function với nhiều đầu vào khác nhau.
- Tuân theo chuẩn PEP 8.

**Ghi nhớ PEP 8:** Code sạch là code được đọc nhiều hơn là được viết.

**Luyện tập nhỏ**

1. Viết function kiểm tra một chuỗi có phải palindrome không.
2. Viết function tính giai thừa của một số.
3. Dùng lambda để tìm bình phương của các số chẵn trong một list.

**Ghi chú cuối**

- Function là trái tim của code có tổ chức và tái sử dụng được.
- Thành thạo function nghĩa là bạn đã thành thạo Python.
- Luyện tập mỗi ngày để xây dựng những dự án tuyệt vời!
