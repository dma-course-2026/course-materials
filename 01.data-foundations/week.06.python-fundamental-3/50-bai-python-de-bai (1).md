# Week 6: 50 bài tập python tiếp


---

## Bài 1. Số bạn trong lớp
Viết chương trình nhập vào sĩ số của một lớp và cho biết bạn có bao nhiêu người bạn trong lớp.

Ví dụ:

| Nhập từ bàn phím | Kết quả ra màn hình |
|---|---|
| Lớp bạn có bao nhiêu người? 40 | Vậy bạn có 39 người bạn trong lớp |

**Gợi ý:**
- Trâu: không có gì "trâu" cả — đây là 1 phép trừ.
- Nhận xét then chốt: bạn không tính chính mình, nên số người bạn = sĩ số − 1.

---

## Bài 2. Phép toán số học
Nhập vào 2 số nguyên dương `a` và `b`. Tính tổng, hiệu, tích, thương của 2 số đó và in kết quả ra màn hình.

Ví dụ:

| Nhập từ bàn phím | Kết quả ra màn hình |
|---|---|
| Nhập a: 10 <br> Nhập b: 5 | Tong 2 so: 15 <br> Hieu 2 so: 5 <br> Tich 2 so: 50 <br> Thương 2 so: 2.0 |

**Gợi ý:**
- Dùng 4 phép toán cơ bản `+`, `-`, `*`, `/`.
- Chú ý: `/` cho kết quả kiểu float (2.0, không phải 2).

---

## Bài 3. Hoán đổi
Viết chương trình nhập vào hai số. Hoán đổi giá trị của hai số đó.

Ví dụ:

| Nhập từ bàn phím | Kết quả ra màn hình |
|---|---|
| Nhập giá trị a: 2 <br> Nhập giá trị b: 3 | Giá trị a: 3 <br> Giá trị b: 2 |

**Gợi ý:**
- Cách cổ điển: dùng biến tạm `t = a; a = b; b = t`.
- Trong Python có cú pháp gọn hơn (gán nhiều biến đồng thời) — tự tìm hiểu.

---

## Bài 4. Số gấp đôi
Viết chương trình nhập một số nguyên `n`. In ra màn hình số gấp đôi của `n`.

Ví dụ:

| Nhập từ bàn phím | Kết quả ra màn hình |
|---|---|
| Nhập giá trị n: 2 | Số gấp đôi: 4 |

**Gợi ý:**
- Nhân `n` với 2.

---

## Bài 5. Điểm thi đua
Theo quy định của nhà trường:
- Mỗi trường hợp không đeo thẻ bị trừ `a` điểm.
- Mỗi trường hợp nói chuyện trong lớp bị trừ `b` điểm.
- Mỗi trường hợp đi học muộn bị trừ `c` điểm.

Trong tháng có `t` trường hợp không đeo thẻ, `n` trường hợp nói chuyện riêng, `m` trường hợp đi học muộn. Nhập `a, b, c, t, n, m` và tính tổng điểm bị trừ.

Ví dụ:

| Nhập từ bàn phím | Kết quả ra màn hình |
|---|---|
| 1 1 1 1 1 1 | 3 |

**Gợi ý:**
- Công thức: `t*a + n*b + m*c`.
- Nhiều số nhập cùng dòng → cần tách chuỗi và chuyển sang số.

---

## Bài 6. Diện tích khu vườn
Một khu đất hình chữ nhật có cạnh `a` và `b` (b là chiều dài, a là chiều rộng). Người ta xây một khu vui chơi hình tròn (đường kính = `a`) ở giữa khu đất. Hỏi khu đất còn lại (phần gạch chéo) có diện tích bằng bao nhiêu. Lấy pi = 3.14.

**Gợi ý:**
- Trâu: tính diện tích hình chữ nhật, tính diện tích hình tròn, lấy hiệu.
- Chú ý: bán kính hình tròn = `a/2`, nên `S_tròn = pi * (a/2)²`.

---

## Bài 7. Điểm trung bình
Nhập vào 3 số thực là điểm số của 3 môn thi. In ra màn hình **"Qua mon"** nếu điểm trung bình ≥ 5.0, ngược lại in **"Khong qua mon"**. Điểm trung bình lấy 4 chữ số thập phân.

Ví dụ:

| Nhập từ bàn phím | Output |
|---|---|
| 4.5 6.7 3.0 | Diem trung binh la: 4.7333 <br> Khong qua mon |

**Gợi ý:**
- Tính trung bình = tổng/3.
- Định dạng 4 chữ số thập phân: dùng `%.4f` hoặc f-string với `:.4f`.
- Dùng cấu trúc `if ... else ...`.

---

## Bài 8. Kiểm tra ký tự Alphabet
Nhập vào một ký tự `c` bất kỳ. Nếu `c` thuộc bảng chữ cái tiếng Anh (a–z hoặc A–Z) thì in "la ki tu Alphabet", ngược lại in "khong phai la ki tu alphabet".

Ví dụ:

| Nhập từ bàn phím | Kết quả ra màn hình |
|---|---|
| A | a la ki tu Alphabet |

**Gợi ý:**
- So sánh ký tự: `'a' <= c <= 'z'` hoặc `'A' <= c <= 'Z'`.
- Hoặc dùng hàm sẵn có `isalpha()` của chuỗi — tùy mức độ muốn tự làm.

---

## Bài 9. Tính tiền điện
Nhập họ tên chủ hộ, chỉ số điện tháng trước (`chiso1`) và chỉ số tháng này (`chiso2`). Tính tiền điện biết:
- Mỗi kW trong 60 kW đầu tiên có đơn giá là 5 đ.
- Từ kW thứ 61 đến kW thứ 160 có đơn giá 8 đ.
- Từ kW thứ 161 trở lên có đơn giá 10 đ.

Ví dụ:

| Nhập từ bàn phím | Kết quả ra màn hình |
|---|---|
| Họ và tên: Lê Mạnh Đoan <br> Nhập chỉ số tháng trước, chỉ số tháng này: 1020 1070 | Họ và tên: Lê Mạnh Đoan <br> Tiền phải trả là   250.00 |

**Gợi ý:**
- Lượng điện tiêu thụ = `chiso2 - chiso1`.
- Dùng `if / elif / else` chia 3 khoảng.
- Khi vượt khoảng, cộng dồn tiền của các bậc trước.

---

## Bài 10. Chữ số hàng trăm, chục, đơn vị
Viết chương trình cho biết chữ số hàng trăm, hàng chục, hàng đơn vị của một số có ba chữ số.

Ví dụ:

| Nhập từ bàn phím | Kết quả ra màn hình |
|---|---|
| Nhập số n: 123 | Chữ số hàng trăm: 1 <br> Chữ số hàng chục: 2 <br> Chữ số hàng đơn vị: 3 |

**Gợi ý:**
- Hàng trăm = `n // 100`.
- Hàng chục = `(n // 10) % 10`.
- Hàng đơn vị = `n % 10`.
- Phép `//` là chia lấy nguyên, `%` là chia lấy dư.

---

## Bài 11. Hình vuông
Nhập vào 1 cạnh của một hình vuông. In ra màn hình diện tích và chu vi của nó.

Ví dụ:

| Nhập từ bàn phím | Kết quả ra màn hình |
|---|---|
| Nhập vào một cạnh: 2 | Diện tích hình vuông: 4 <br> Chu vi hình vuông: 8 |

**Gợi ý:**
- Diện tích = `a*a`, chu vi = `4*a`.

---

## Bài 12. Hình chữ nhật
Nhập vào 2 cạnh của một hình chữ nhật. In ra màn hình diện tích và chu vi của nó.

Ví dụ:

| Nhập từ bàn phím | Kết quả ra màn hình |
|---|---|
| Nhập chiều dài: 2 <br> Nhập chiều rộng: 3 | Dien tich hinh chu nhat la: 6.0 <br> Chu vi hinh chu nhat: 10.0 |

**Gợi ý:**
- `S = a*b`, `P = 2*(a+b)`.

---

## Bài 13. Hình tròn
Nhập vào bán kính của hình tròn. In ra màn hình diện tích và chu vi của nó (kết quả làm tròn 2 chữ số thập phân).

Ví dụ:

| Nhập từ bàn phím | Kết quả ra màn hình |
|---|---|
| Nhập bán kính R=2 | Diện tích hình tròn là: 12.56 <br> Chu vi hình tròn là: 12.56 |

**Gợi ý:**
- `S = π·R²`, `P = 2·π·R`.
- Định dạng `.2f`.

---

## Bài 14. Hình tam giác
Nhập vào ba số `a, b, c` bất kỳ. Kiểm tra xem nó có thể là độ dài ba cạnh hay không. Nếu không thì in ra màn hình `'Không là 3 cạnh của một tam giác'`. Ngược lại, in diện tích và chu vi của tam giác ra màn hình.

Ví dụ:

| Nhập từ bàn phím | Kết quả ra màn hình |
|---|---|
| Nhập 3 số a,b,c = 1 2 3 | 1.0 , 2.0 , 3.0 Không phải là 3 cạnh của tam giác |

**Gợi ý:**
- Điều kiện tam giác: tổng 2 cạnh bất kỳ > cạnh còn lại.
- Diện tích dùng công thức **Heron**: `S = √(p(p−a)(p−b)(p−c))` với `p = (a+b+c)/2`.
- `sqrt` nằm trong module `math`.

---

## Bài 15. Tam giác đều
Viết chương trình xét xem một tam giác có là tam giác đều hay không khi biết ba cạnh của tam giác.

Ví dụ:

| Nhập từ bàn phím | Kết quả ra màn hình |
|---|---|
| Nhap a = 2 <br> Nhap b = 2 <br> Nhap c = 2 | La tam giac deu |

**Gợi ý:**
- Điều kiện: 3 cạnh bằng nhau.

---

## Bài 16. Tam giác cân
Viết chương trình xét xem một tam giác có là tam giác cân hay không khi biết ba cạnh của tam giác.

Ví dụ:

| Nhập từ bàn phím | Kết quả ra màn hình |
|---|---|
| Nhập a = 2 <br> Nhập b = 2 <br> Nhập c = 3 | Là tam giác cân |

**Gợi ý:**
- Có ít nhất 2 cạnh bằng nhau: `a==b` hoặc `b==c` hoặc `a==c`.

---

## Bài 17. Tam giác vuông
Viết chương trình xét xem một tam giác có là tam giác vuông hay không khi biết ba cạnh của tam giác.

Ví dụ:

| Nhập từ bàn phím | Kết quả ra màn hình |
|---|---|
| Nhập a = 3 <br> Nhập b = 4 <br> Nhập c = 5 | Là tam giác vuông |

**Gợi ý:**
- Định lý Pythagoras: tổng bình phương 2 cạnh = bình phương cạnh còn lại.
- Phải xét cả 3 trường hợp vì không biết cạnh nào là cạnh huyền.

---

## Bài 18. Phương trình bậc 1
Viết chương trình giải phương trình bậc 1 (`ax + b = 0`).

Ví dụ:

| Nhập từ bàn phím | Kết quả ra màn hình |
|---|---|
| Nhập a = 2 <br> Nhập b = 3 | Phuong trình có một nghiệm! x = -1.5 |

**Gợi ý:**
- Nếu `a ≠ 0`: nghiệm duy nhất `x = -b/a`.
- Nếu `a = 0` và `b = 0`: vô số nghiệm.
- Nếu `a = 0` và `b ≠ 0`: vô nghiệm.

---

## Bài 19. Bất phương trình bậc 1
Viết chương trình giải bất phương trình bậc 1 (`ax + b ≥ 0`).

Ví dụ:

| Nhập từ bàn phím | Kết quả ra màn hình |
|---|---|
| Nhập a = 2 <br> Nhập b = 3 | Bất phương trình có nghiệm: x >= -1.5 |

**Gợi ý:**
- Nếu `a > 0`: `x ≥ -b/a`.
- Nếu `a < 0`: `x ≤ -b/a` (phải đổi chiều dấu).
- Nếu `a = 0`: dựa vào dấu `b`.

---

## Bài 20. Phương trình bậc 2
Viết chương trình giải phương trình bậc 2 (`ax² + bx + c = 0`).

Ví dụ:

| Nhập từ bàn phím | Kết quả ra màn hình |
|---|---|
| nhập a: 3 <br> nhập b: 5 <br> nhập c: 2 | Phương trình có 2 nghiệm phân biệt: <br> x1 = -0.6666666666666666 <br> x2 = -1.0 |

**Gợi ý:**
- Tính `Δ = b² − 4ac`.
- `Δ < 0`: vô nghiệm.
- `Δ = 0`: nghiệm kép `x = -b/(2a)`.
- `Δ > 0`: 2 nghiệm phân biệt `x = (-b ± √Δ) / (2a)`.

---

## Bài 21. Kiểm tra chẵn/lẻ
Viết chương trình nhập vào 1 số nguyên dương `n` từ bàn phím. Hãy cho biết số đó là số chẵn hay số lẻ và thông báo kết quả ra màn hình.

Ví dụ:

| Nhập từ bàn phím | Kết quả ra màn hình |
|---|---|
| Nhập n: 12 | 12 là số chẵn |

**Gợi ý:**
- `n % 2 == 0` ⇒ chẵn, ngược lại lẻ.

---

## Bài 22. Hai số cùng tính chẵn lẻ
Viết chương trình nhập 2 số tự nhiên `M, N` và thông báo "ĐÚNG" nếu `M, N` cùng tính chẵn lẻ, ngược lại thì thông báo "SAI".

Ví dụ:

| Nhập từ bàn phím | Kết quả ra màn hình |
|---|---|
| Nhập M: 10 <br> Nhập N: 20 | ĐÚNG |

**Gợi ý:**
- Mẹo: `(M + N) % 2 == 0` ⇔ `M, N` cùng tính chẵn lẻ.
- Hoặc so sánh trực tiếp `M%2 == N%2`.

---

## Bài 23. Kiểm tra ước số
Viết chương trình nhập vào 2 số nguyên, kiểm tra xem chúng có phải là ước của nhau không.

Ví dụ:

| Nhập từ bàn phím | Kết quả ra màn hình |
|---|---|
| nhập a: 5 <br> nhập b: 10 | 10 khong la uoc cua 5 <br> 5 la uoc cua 10 |

**Gợi ý:**
- `a` là ước của `b` ⇔ `b % a == 0`.
- Kiểm tra cả hai chiều.

---

## Bài 24. Giá trị nhỏ nhất của 2 số
Tìm giá trị nhỏ nhất trong 2 số nguyên `a` và `b` (`a, b` được nhập từ bàn phím).

Ví dụ:

| Nhập từ bàn phím | Kết quả ra màn hình |
|---|---|
| nhập a: 5 <br> nhập b: 10 | 5 là giá trị nhỏ nhất |

**Gợi ý:**
- `if a < b` → in `a`, ngược lại in `b`.
- Hoặc dùng `min(a, b)`.

---

## Bài 25. Giá trị lớn nhất của 3 số
Tìm giá trị lớn nhất trong 3 số nguyên `a, b, c` (`a, b, c` được nhập từ bàn phím).

Ví dụ:

| Nhập từ bàn phím | Kết quả ra màn hình |
|---|---|
| nhập a: 1 <br> nhập b: 2 <br> nhập c: 3 | Giá trị lớn nhất trong 3 số: 3 |

**Gợi ý:**
- Giả sử `max = a`, so sánh lần lượt với `b` rồi `c`, cập nhật nếu lớn hơn.
- Hoặc `max(a, b, c)` sẵn có.

---

## Bài 26. Giá trị lớn nhất của 4 số
Tìm giá trị lớn nhất trong 4 số nguyên `a, b, c, d` (`a, b, c, d` được nhập vào từ bàn phím).

Ví dụ:

| Nhập từ bàn phím | Kết quả ra màn hình |
|---|---|
| nhập a: 1 <br> nhập b: 2 <br> nhập c: 3 <br> nhập d: 4 | Giá trị lớn nhất trong 4 số: 4 |

**Gợi ý:**
- Mở rộng ý tưởng bài 25 cho 4 biến.
- Hoặc dùng `max(a, b, c, d)`.

---

## Bài 27. Giá trị nhỏ nhất của 5 số thực
Tìm giá trị nhỏ nhất trong 5 số thực `a, b, c, d, e` (`a, b, c, d, e` được nhập vào từ bàn phím).

Ví dụ:

| Nhập từ bàn phím | Kết quả ra màn hình |
|---|---|
| nhập a: 1 <br> nhập b: 2 <br> nhập c: 3 <br> nhập d: 4 <br> nhập e: 5 | Giá trị nhỏ nhất trong 5 số: 1.0 |

**Gợi ý:**
- Tương tự bài 24, nhưng cho 5 số thực.
- Dùng `min(a, b, c, d, e)`.

---

## Bài 28. Máy tính 2 ngôi
Bạn hãy nhập vào hai số nguyên (int) và một phép toán (str) rồi in ra màn hình kết quả của phép toán.

Ví dụ:

| Nhập từ bàn phím | Kết quả ra màn hình |
|---|---|
| Nhập số thứ 1: 12 <br> Nhập số thứ 2: 13 <br> Nhập phép toán: + | 12 + 13 = 25 |

**Gợi ý:**
- Đọc phép toán vào biến chuỗi.
- Dùng `if / elif` để chọn phép toán tương ứng.
- Với `/`, chú ý định dạng số thập phân.

---

## Bài 29. Số ngày của năm
Tìm số ngày của năm `N`, biết rằng năm nhuận là năm chia hết cho 400 hoặc chia hết cho 4 nhưng không chia hết cho 100. Ví dụ: các năm 2000, 2004 là năm nhuận và có số ngày là 366; các năm 1900, 1945 không phải là năm nhuận và có số ngày là 365.

Ví dụ:

| Nhập từ bàn phím | Kết quả ra màn hình |
|---|---|
| Nhập năm: 2021 | Số ngày của năm: 2021 là 365 |

**Gợi ý:**
- Điều kiện năm nhuận: `(n % 400 == 0) or (n % 4 == 0 and n % 100 != 0)`.
- Chú ý ưu tiên toán tử: dùng dấu ngoặc rõ ràng.

---

## Bài 30. Đổi giây sang giờ–phút–giây
Nhập vào thời gian 1 công việc nào đó là `x` giây. Hãy chuyển đổi và viết ra màn hình số thời gian trên dưới dạng bằng bao nhiêu giờ, bao nhiêu phút, bao nhiêu giây.

Ví dụ:

| Nhập từ bàn phím | Kết quả ra màn hình |
|---|---|
| Nhập vào số giây: 3567 | Kết quả = 0 giờ: 59 phút: 27 giây |

**Gợi ý:**
- Giờ = `x // 3600`, phần dư `x %= 3600`.
- Phút = `x // 60`, giây = `x % 60`.

---

## Bài 31. Đồng hồ điện tử — tăng 1 giây
Bảng của đồng hồ điện tử gồm một dãy ba số `h, p, s` thể hiện tương ứng giờ, phút và giây của thời điểm hiện tại. Cứ sau mỗi giây giá trị của bộ ba số `h, p, s` sẽ thay đổi thành 3 số `h1, p1, s1` tương ứng với thời điểm mới. Hãy tìm 3 số `h1, p1, s1` và in kết quả ra màn hình.

Ví dụ:

| Nhập từ bàn phím | Kết quả ra màn hình |
|---|---|
| Nhập giờ, phút, giây: 1 23 59 | 1 24 0 |

**Gợi ý:**
- Cộng 1 vào `s`. Nếu `s == 60` → `s = 0`, `p += 1`.
- Tương tự với `p` và `h`. Nếu `h == 24` → `h = 0`.

---

## Bài 32. Hệ phương trình bậc 1 hai ẩn
Giải hệ phương trình tuyến tính:
```
ax + by = m
cx + dy = n
```

Ví dụ:

| Nhập từ bàn phím | Kết quả ra màn hình |
|---|---|
| Nhập a = 1 <br> Nhập b = 2 <br> Nhập m = 3 <br> Nhập c = 2 <br> Nhập d = 3 <br> Nhập n = 5 | Hệ phương trình có 1 cặp nghiệm: <br> x = 1.0  va  y = 1.0 |

**Gợi ý:**
- Phương pháp **Cramer**: `D = a·d - b·c`, `Dx = m·d - b·n`, `Dy = a·n - c·m`.
- Nếu `D ≠ 0`: `x = Dx/D`, `y = Dy/D`.
- Nếu `D = 0` và `Dx = Dy = 0`: vô số nghiệm.
- Nếu `D = 0`, còn lại: vô nghiệm.

---

## Bài 33. Điểm thuộc đường tròn
Nhập vào tâm và bán kính của một đường tròn. Sau đó nhập vào một điểm `A(x, y)` bất kỳ và kiểm tra xem nó có thuộc đường tròn hay không?

Ví dụ:

| Nhập từ bàn phím | Kết quả ra màn hình |
|---|---|
| Nhap ban kinh R: 3 <br> Nhap toa do tam duong tron: <br> x0: 1 <br> y0: 2 <br> Nhap toa do diem a: <br> xa: 2 <br> ya: 1 | Diem A nam trong duong tron |

**Gợi ý:**
- Khoảng cách `d = √((xa−x0)² + (ya−y0)²)`.
- So sánh `d` với `R`: `d < R` nằm trong, `d == R` nằm trên, `d > R` nằm ngoài.

---

## Bài 34. In các số lẻ ≤ n
Viết chương trình in ra các số lẻ nhỏ hơn hoặc bằng `n` (với `n` được nhập từ bàn phím).

Ví dụ:

| Nhập từ bàn phím | Kết quả ra màn hình |
|---|---|
| Nhap so n = 10 | 1 3 5 7 9 |

**Gợi ý:**
- Duyệt `i` từ 1 đến `n`, kiểm tra `i % 2 == 1`.
- Hoặc đi `i = 1, 3, 5, …` để tránh kiểm tra.

---

## Bài 35. Tổng Sₙ từ 1 đến n
Bạn hãy nhập vào số `n` (int) rồi in ra màn hình kết quả của phép toán cộng từ 1 đến `n`.

Ví dụ:

| Nhập từ bàn phím | Kết quả ra màn hình |
|---|---|
| Nhập số n: 5 | Tổng từ 1 đến 5 = 15 |

**Gợi ý:**
- Trâu: `for i in range(1, n+1)` cộng dồn.
- Công thức Gauss: `n·(n+1)/2` — gọn hơn, O(1).

---

## Bài 36. Tổng các số chẵn từ 1 đến n
Bạn hãy nhập vào số `n` (Integer) rồi in ra màn hình kết quả của phép toán cộng các số chẵn từ 1 đến `n`.

Ví dụ:

| Nhập từ bàn phím | Kết quả ra màn hình |
|---|---|
| Nhập n: 10 | Tổng các số chẵn từ 1 đến 10 = 30 |

**Gợi ý:**
- Duyệt `i` từ 1 đến `n`, cộng khi `i % 2 == 0`.
- Hoặc tổng = `2 + 4 + ... + 2k = 2·(1+2+...+k)` với `k = n//2`.

---

## Bài 37. Tổng các số lẻ từ 1 đến n
Bạn hãy nhập vào số `n` (Integer) rồi in ra màn hình kết quả của phép toán cộng các số lẻ từ 1 đến `n`.

Ví dụ:

| Nhập từ bàn phím | Kết quả ra màn hình |
|---|---|
| Nhập n: 10 | Tổng các số lẻ từ 1 đến 10 = 25 |

**Gợi ý:**
- Tương tự bài 36, nhưng điều kiện `i % 2 == 1`.
- Tính chất đẹp: tổng `k` số lẻ đầu tiên = `k²`.

---

## Bài 38. Tính giai thừa
Bạn hãy nhập vào số `n` (int) rồi in ra màn hình kết quả của phép toán giai thừa `n!`.

Ví dụ:

| Nhập từ bàn phím | Kết quả ra màn hình |
|---|---|
| Nhập n: 5 | 5 giai thừa = 120 |

**Gợi ý:**
- Duyệt `i` từ 1 đến `n`, nhân dồn vào biến `gt` khởi tạo = 1.
- Cẩn thận: `n!` lớn rất nhanh (nhưng Python số nguyên không tràn).

---

## Bài 39. Tính luỹ thừa aⁿ
Bạn hãy nhập vào cơ số `a` và số mũ `n` (int) rồi in ra màn hình kết quả của phép toán `aⁿ`.

Ví dụ:

| Nhập từ bàn phím | Kết quả ra màn hình |
|---|---|
| Nhập cơ số: 2 <br> Nhập số mũ: 3 | 2 lũy thừa 3 = 8 |

**Gợi ý:**
- Python có toán tử `**` sẵn: `a ** n`.
- Nếu tự viết: nhân `a` với chính nó `n` lần.
- Nâng cao: luỹ thừa nhanh (binary exponentiation) — O(log n).

---

## Bài 40. Tổng các số chia hết cho 3 hoặc 5 trong [M, N]
Viết chương trình nhập 2 số nguyên dương `M` và `N` từ bàn phím (`M < N`). Tính và đưa ra màn hình tổng các số chia hết cho 3 hoặc 5 trong phạm vi từ `M` đến `N`.

Ví dụ:

| Nhập từ bàn phím | Kết quả ra màn hình |
|---|---|
| Nhập số M<N: <br> Nhập M: 3 <br> Nhập N: 5 | Kết quả: 8 |

**Gợi ý:**
- Duyệt `i` từ `M` đến `N`, cộng khi `i % 3 == 0 or i % 5 == 0`.
- Chú ý: dùng **hoặc** (`or`), không phải **và**.

---

## Bài 41. Tổng các số chia hết cho 2 và 3 trong [M, N]
Viết chương trình nhập 2 số nguyên dương `M` và `N` từ bàn phím (`M < N`). Tính và đưa ra màn hình tổng các số chia hết cho 2 và 3 trong phạm vi từ `M` đến `N`.

Ví dụ:

| Nhập từ bàn phím | Kết quả ra màn hình |
|---|---|
| Nhập số M<N: <br> Nhập M: 1 <br> Nhập N: 10 | Kết quả: 6 |

**Gợi ý:**
- Duyệt `i`, cộng khi `i % 2 == 0 and i % 3 == 0`.
- Nhận xét: `i % 2 == 0 and i % 3 == 0` ⇔ `i % 6 == 0`.

---

## Bài 42. Liệt kê các ước của n
Viết chương trình in ra tất cả các ước của một số `n`. Mỗi ước được ghi trên một dòng (với `n` được nhập từ bàn phím).

Ví dụ:

| Nhập từ bàn phím | Kết quả ra màn hình |
|---|---|
| Nhap so n = 5 | 1 <br> 5 |

**Gợi ý:**
- Trâu: duyệt `i` từ 1 đến `n`, in nếu `n % i == 0`. Độ phức tạp O(n).
- Tối ưu: chỉ cần duyệt đến `√n`; với mỗi `i` là ước thì `n/i` cũng là ước. O(√n).

---

## Bài 43. Đếm số ước của n
Viết chương trình nhập vào 1 số nguyên dương `n`, hãy cho biết `n` có bao nhiêu ước và thông báo kết quả ra màn hình.

Ví dụ:

| Nhập từ bàn phím | Kết quả ra màn hình |
|---|---|
| Nhập n: 10 | 10 co 4 uoc |

**Gợi ý:**
- Giống bài 42 nhưng đếm thay vì in.
- Có thể dùng tối ưu `√n` (chú ý nếu `i*i == n` chỉ đếm 1 lần).

---

## Bài 44. Đếm số trong khoảng (10, 20)
Nhập `N` số bất kỳ từ bàn phím, đếm các số lớn hơn 10 và nhỏ hơn 20 và thông báo kết quả ra màn hình.

Ví dụ:

| Nhập từ bàn phím | Kết quả ra màn hình |
|---|---|
| Nhập N: 4 <br> nhập số thứ 1 = 4 <br> nhập số thứ 2 = 12 <br> nhập số thứ 3 = 3 <br> nhập số thứ 4 = 15 | Số các số >10 và <20 là: 2 |

**Gợi ý:**
- Dùng biến đếm `dem = 0`.
- Duyệt `N` lần, với mỗi lần đọc một số và kiểm tra `10 < so < 20`.

---

## Bài 45. Kiểm tra số nguyên tố
Nhập vào một số nguyên không âm, kiểm tra xem nó có phải là số nguyên tố hay không?

Ví dụ:

| Nhập từ bàn phím | Kết quả ra màn hình |
|---|---|
| Nhập số n: 5 | 5 là số nguyên tố |

**Gợi ý:**
- Trâu: đếm số ước trong `[1, n]`. Nếu đúng 2 ước → nguyên tố. O(n).
- Hỏi: trâu lãng phí ở đâu? Chỉ cần tìm **một** ước thật sự nằm giữa `1` và `n` để kết luận "không nguyên tố".
- Tối ưu: chỉ cần kiểm tra ước đến `√n`. Vì nếu `n = a·b` thì ít nhất một trong `a, b` ≤ `√n`.
- Chú ý trường hợp đặc biệt: `n < 2` không là nguyên tố, `n = 2` là nguyên tố nhỏ nhất.

---

## Bài 46. Kiểm tra số hoàn hảo
Viết chương trình nhập vào 1 số nguyên dương `n`. Kiểm tra xem `n` có phải là số hoàn hảo không. Số `N` được gọi là số hoàn hảo, nếu tổng các ước số của nó (không kể nó) bằng `N`.

Ví dụ:

| Nhập từ bàn phím | Kết quả ra màn hình |
|---|---|
| nhập n: 6 | 6 là số hoàn hảo |

**Gợi ý:**
- Duyệt `i` từ 1 đến `n−1`, cộng vào tổng nếu `n % i == 0`.
- Có thể tối ưu bằng cách chỉ duyệt đến `√n` (ghép cặp ước).

---

## Bài 47. Các số hoàn hảo nhỏ hơn n
Viết chương trình tìm các số hoàn chỉnh nhỏ hơn `n` (với `n` được nhập từ bàn phím).

Ví dụ:

| Nhập từ bàn phím | Kết quả ra màn hình |
|---|---|
| Nhap so n: 15 | 6 |

**Gợi ý:**
- Với mỗi `i` trong `[1, n]`, kiểm tra `i` có hoàn hảo không (dùng ý bài 46).
- Lưu ý: 2 vòng lặp lồng nhau → O(n²), đủ dùng với `n` nhỏ.
- **Liên tưởng:** đây là mẫu "duyệt + kiểm tra tính chất" rất phổ biến trong bài tập cơ bản (số nguyên tố nhỏ hơn n, số chính phương nhỏ hơn n, …).

---

## Bài 48. Số chính phương
Số chính phương là số mà căn bậc hai của nó là 1 số nguyên dương. Viết chương trình nhập vào một số nguyên dương `n` và cho biết `n` có phải là số chính phương hay không?

Ví dụ:

| Nhập từ bàn phím | Kết quả ra màn hình |
|---|---|
| nhập n: 16 | 16 là số chính phương |

**Gợi ý:**
- Lấy `m = int(√n)`, kiểm tra `m*m == n`.
- Chú ý: do sai số của số thực `sqrt`, nên có thể cần kiểm tra cả `(m+1)² == n` hoặc dùng tìm kiếm nhị phân cho an toàn.

---

## Bài 49. Số 3 chữ số `abc = a³ + b³ + c³` (số Armstrong)
Viết chương trình tìm tất cả các số có 3 chữ số `abc` sao cho `abc = a³ + b³ + c³`.

Ví dụ:

| Nhập từ bàn phím | Kết quả ra màn hình |
|---|---|
| *(không nhập)* | 1 5 3 <br> 3 7 0 <br> 3 7 1 <br> 4 0 7 |

**Gợi ý:**
- Duyệt 3 vòng lồng nhau: `a` từ 1 đến 9 (hàng trăm khác 0), `b` và `c` từ 0 đến 9.
- Với mỗi bộ, kiểm tra điều kiện và in ra.
- Chỉ 10·10·10 = 1000 bộ → chạy tức thì.
- **Liên tưởng:** đây là lớp bài toán "số có tính chất đặc biệt" — mô-típ **brute-force trên không gian nhỏ**.

---

## Bài 50. Số 3 chữ số thoả `a + b + c = a·b·c`
Viết chương trình tìm tất cả các số có 3 chữ số sao cho tổng tất cả các chữ số bằng tích của chúng.

Ví dụ:

| Nhập từ bàn phím | Kết quả ra màn hình |
|---|---|
| *(không nhập)* | 1 2 3 <br> 1 3 2 <br> 2 1 3 <br> 2 3 1 <br> 3 1 2 <br> 3 2 1 |

**Gợi ý:**
- Duyệt 3 vòng cho `a, b, c` (cùng khoảng để liệt kê hết hoán vị).
- Kiểm tra `a + b + c == a*b*c`.
- **Nhận xét toán học:** bộ `(1, 2, 3)` là bộ số nguyên dương duy nhất (xét theo tập, không kể thứ tự) thoả tính chất này — có thể chứng minh bằng cách giả sử `a ≤ b ≤ c` rồi chặn.

---

*50 bài tiếp theo. Khi làm, hãy tự viết code trước và chỉ dùng AI để tìm hiểu kiến thức, chúc các bạn luyệt tập tốt.*
