# CẨM NANG PYTHON TOÀN TẬP

**CHƯƠNG – 2 | Trang – 2/5**

## 2. CÁC CÂU LỆNH ĐIỀU KHIỂN LUỒNG (tiếp theo)

### ★ 2. Câu lệnh lặp (Looping Statements)

Loop dùng để thực thi một khối code nhiều lần. Python có hai loại loop:

1. `for loop`
2. `while loop`

| for loop | while loop |
|---|---|
| `for variable in sequence:`<br>&nbsp;&nbsp;&nbsp;&nbsp;`# block of code` | `while condition:`<br>&nbsp;&nbsp;&nbsp;&nbsp;`# block of code` |

### ★ for Loop

Dùng để duyệt qua một sequence (list, tuple, string, range, v.v.)

```python
for i in range(1, 6):
    print(i)
```

**Output:** 1 2 3 4 5

**Giải thích:** `range(1,6)` sinh ra các số từ 1 đến 5 (6 bị loại trừ).

### ★ while Loop

Lặp lại một khối code chừng nào điều kiện còn True.

```python
i = 1
while i <= 5:
    print(i)
    i = i + 1
```

**Output:** 1 2 3 4 5

**Giải thích:** Loop chạy khi i nhỏ hơn hoặc bằng 5.

### ★ Sự khác biệt giữa for loop và while loop

| Đặc điểm | for loop | while loop |
|---|---|---|
| Mục đích | Duyệt qua sequence | Lặp dựa trên điều kiện |
| Khởi tạo | Không cần (tự động) | Cần (trước loop) |
| Điều kiện | Xử lý tự động | Kiểm tra thủ công |
| Tăng/Giảm | Xử lý tự động | Xử lý thủ công (trong loop) |
| Dùng khi nào | Biết trước số lần lặp | Không biết trước số lần lặp |

### ★ 3. Câu lệnh nhảy (Jump Statements)

Jump statement dùng để thay đổi luồng thực thi bình thường của chương trình. Python có ba jump statement: 1. `break` 2. `continue` 3. `pass`.

**1. break**

Dùng để dừng loop hoàn toàn.

```python
for i in range(1,6):
    if i == 3:
        break
    print(i)
```

**Output:** 1 2

**2. continue**

Bỏ qua vòng lặp hiện tại, tiếp tục vòng kế.

```python
for i in range(1,6):
    if i == 3:
        continue
    print(i)
```

**Output:** 1 2 4 5

**3. pass**

Không làm gì cả, dùng làm placeholder.

```python
for i in range(3):
    pass
print("Hello")
```

**Output:** Hello

**Tóm tắt**

- Control flow quyết định thứ tự thực thi.
- Loop lặp lại code.
- Jump statement điều khiển luồng bên trong loop.

**Ghi nhớ**

- Dùng `for loop` khi biết trước số lần lặp.
- Dùng `while loop` khi chưa biết trước số lần lặp.
- Dùng `break` để thoát, `continue` để bỏ qua, `pass` làm placeholder.
