# Bài tập Python - Week 5



- **Group 1 (Bài 1 – 10):** Nhập/Xuất và Số Học Cơ Bản
- **Group 2 (Bài 11 – 33):** Các bài toán thực tế về hình học và phương trình
- **Group 3 (Bài 34 – 40):** Vòng Lặp Cơ Bản

Mỗi bài gồm **đề bài**, **ví dụ Input/Output** và **gợi ý**. Không kèm lời giải — hãy tự thực hành trước.

---

## Chương 1 – Nhập/Xuất và Số Học Cơ Bản

> Nhắc nhanh: `input(prompt)` trả về chuỗi, cần `int()`/`float()` để tính toán. Phép toán cơ bản: `+ - * / // % **`. In kết quả nên dùng f-string `f"...{biến}..."`.

### Bài 1 – Số Bạn Trong Lớp
**Đề bài:** Viết chương trình nhập vào sĩ số của một lớp và cho biết bạn có bao nhiêu người bạn trong lớp.

**Ví dụ:** Nhập `35` → Xuất `Vậy bạn có 34 người bạn trong lớp`.

**Gợi ý:** Ép kiểu `int()` khi nhập. Số bạn = sĩ số − 1 (trừ chính mình).

---

### Bài 2 – Phép Toán Số Học
**Đề bài:** Nhập vào 2 số nguyên dương a và b. Tính tổng, hiệu, tích, thương của 2 số đó và in kết quả ra màn hình.

**Ví dụ:** `a = 12`, `b = 4` → Tổng 16, Hiệu 8, Tích 48, Thương 3.0.

**Gợi ý:** Dùng lần lượt `+`, `-`, `*`, `/`. Chú ý `/` luôn ra số thực.

---

### Bài 3 – Hoán Đổi
**Đề bài:** Nhập vào 2 số nguyên a, b. Hoán đổi giá trị 2 biến và in kết quả.

**Ví dụ:** `a = 5`, `b = 8` → Sau khi hoán đổi: a = 8, b = 5.

**Gợi ý:** Python cho phép `(a, b) = (b, a)`; hoặc dùng biến tạm.

---

### Bài 4 – Số Gấp Đôi
**Đề bài:** Nhập vào số n và in ra số gấp đôi.

**Ví dụ:** `n = 7` → `Số gấp đôi của n là: 14`.

**Gợi ý:** Nhân 2 hoặc cộng `n + n`.

---

### Bài 5 – Nội Quy
**Đề bài:** Nhập a, b, c, t, n, m và tính tổng chi phí theo công thức
`tổng chi phí = t × a + n × b + m × c`.

**Ví dụ:** Nhập `1500 2500 4000 2 4 1` → `Tổng chi phí là: 17000`.

**Gợi ý:** Nhập 6 số trên một dòng bằng `map(int, input().split())`. Áp dụng đúng công thức, chú ý thứ tự biến.

---

### Bài 6 – Diện Tích Khu Vườn
**Đề bài:** Một khu đất hình chữ nhật có cạnh a và b. Người ta xây một khu vui chơi hình tròn tại vị trí trong khu đất. Hỏi diện tích còn lại bằng bao nhiêu? Biết π = 3.14.

**Ví dụ:** `a = 10`, `b = 20` → `Diện tích còn lại: 121.50`.

**Gợi ý:** `S1 = a*b`; khu vui chơi hình tròn có bán kính = a/2, nên `S2 = π*(a/2)²`. Kết quả = S1 − S2, in dạng `{...:.2f}`.

---

### Bài 7 – Điểm Số
**Đề bài:** Nhập 3 điểm số thực, tính điểm trung bình và xét kết quả đậu/rớt.

**Ví dụ:** Nhập `5.0 7.5 8.5` → `Điểm trung bình là: 7.0`, `Đậu`.

**Gợi ý:** `map(float, input().split())` để nhập 3 số. Trung bình = (a+b+c)/3. Dùng `if/else` so sánh với ngưỡng 5.0.

---

### Bài 8 – Kiểm Tra Ký Tự
**Đề bài:** Nhập một ký tự và kiểm tra xem có phải là chữ cái Alphabet không.

**Ví dụ:** Nhập `g` → `g là ký tự Alphabet`.

**Gợi ý:** So sánh `'a' <= ch <= 'z'` hoặc `'A' <= ch <= 'Z'`. Có thể dùng `.isalpha()` nhưng nên hiểu cách so sánh thủ công.

---

### Bài 9 – Tính Tiền Điện
**Đề bài:** Nhập họ tên chủ hộ, chỉ số điện kế tháng trước và tháng này. Tính tiền điện theo bảng giá:
- 60 kW đầu: 5đ/kW
- kW thứ 61–160: 8đ/kW
- Từ kW 161 trở lên: 10đ/kW

**Ví dụ:** Nhập chỉ số `1500 1580` → tiêu thụ 80 kW → `Số tiền phải trả là: 460.00`.

**Gợi ý:** Lượng điện = chỉ số mới − chỉ số cũ. Dùng `if/elif/else` ba bậc; khi ở bậc cao hơn phải cộng dồn tiền của các bậc dưới (60×5, 100×8, …).

---

### Bài 10 – Đọc Số Có 3 Chữ Số
**Đề bài:** Nhập số n có 3 chữ số và in ra chữ số hàng trăm, hàng chục, hàng đơn vị.

**Ví dụ:** `n = 456` → hàng trăm = 4, hàng chục = 5, hàng đơn vị = 6.

**Gợi ý:** Hàng trăm = `n // 100`, hàng chục = `(n % 100) // 10`, hàng đơn vị = `n % 10`.

---

## Chương 2 – Hình Học và Phương Trình

> Nhắc nhanh: Dùng `if - elif - else` để rẽ nhánh; `and`, `or`, `not` để kết hợp điều kiện. Thư viện `math` cung cấp `math.sqrt`, `math.pi`.

### Bài 11 – Hình Vuông
**Đề bài:** Nhập cạnh hình vuông. In diện tích và chu vi.

**Ví dụ:** Cạnh = 6 → Diện tích 36, Chu vi 24.

**Gợi ý:** Diện tích = `a*a` (hoặc `a**2`); chu vi = `4*a`.

---

### Bài 12 – Hình Chữ Nhật
**Đề bài:** Nhập chiều dài và chiều rộng. In diện tích và chu vi hình chữ nhật.

**Ví dụ:** Dài = 8, Rộng = 5 → Diện tích 40.0, Chu vi 26.0.

**Gợi ý:** Diện tích = `dai * rong`; chu vi = `2 * (dai + rong)`.

---

### Bài 13 – Hình Tròn
**Đề bài:** Nhập bán kính hình tròn. In diện tích và chu vi (làm tròn 2 chữ số thập phân).

**Ví dụ:** R = 3.5 → Diện tích 38.47, Chu vi 21.98.

**Gợi ý:** `S = π·R²`, `C = 2·π·R`. Dùng `math.pi` cho chuẩn. In bằng `{...:.2f}`.

---

### Bài 14 – Hình Tam Giác
**Đề bài:** Nhập 3 số a, b, c. Kiểm tra có tạo thành tam giác không. Nếu có, tính diện tích và chu vi.

**Ví dụ:** `3 4 5` → Chu vi 12.00, Diện tích 6.00.

**Gợi ý:** Điều kiện tam giác: tổng 2 cạnh bất kỳ lớn hơn cạnh còn lại. Diện tích dùng công thức Heron: với `p = (a+b+c)/2`, `S = sqrt(p·(p−a)·(p−b)·(p−c))`.

---

### Bài 15 – Tam Giác Đều
**Đề bài:** Nhập 3 cạnh a, b, c. Kiểm tra có phải tam giác đều không.

**Ví dụ:** `a = b = c = 5` → `Là tam giác đều`.

**Gợi ý:** Trước tiên kiểm tra có là tam giác không. Sau đó so sánh `a == b == c`.

---

### Bài 16 – Tam Giác Cân
**Đề bài:** Nhập 3 cạnh a, b, c. Kiểm tra có phải tam giác cân không.

**Ví dụ:** `a = 5, b = 5, c = 8` → `Là tam giác cân`.

**Gợi ý:** Tam giác cân khi có ít nhất hai cạnh bằng nhau: `a == b or b == c or a == c`.

---

### Bài 17 – Tam Giác Vuông
**Đề bài:** Nhập 3 cạnh a, b, c. Kiểm tra có phải tam giác vuông không (Định lý Pythagoras).

**Ví dụ:** `a = 3, b = 4, c = 5` → `Là tam giác vuông`.

**Gợi ý:** Kiểm tra 3 trường hợp: `a² + b² == c²` hoặc `a² + c² == b²` hoặc `b² + c² == a²`. Hoặc sắp xếp để cạnh lớn nhất đứng cuối rồi so với tổng bình phương 2 cạnh còn lại.

---

### Bài 18 – Giải Phương Trình Bậc 1 (ax + b = 0)
**Đề bài:** Nhập hệ số a, b. Giải phương trình bậc nhất một ẩn.

**Ví dụ:** `a = 2, b = -4` → `Phương trình có một nghiệm: x = 2.0`.

**Gợi ý:** Nếu `a == 0`: xét `b == 0` (vô số nghiệm) hoặc `b ≠ 0` (vô nghiệm). Nếu `a ≠ 0`: `x = -b/a`.

---

### Bài 19 – Bất Phương Trình Bậc 1 (ax + b ≥ 0)
**Đề bài:** Nhập a, b. Giải bất phương trình bậc nhất một ẩn.

**Ví dụ:** `a = 3, b = -9` → `Bất phương trình có nghiệm: x >= 3.0`.

**Gợi ý:** Nhân/chia hai vế cho a cần chú ý dấu của a: `a > 0` → `x >= -b/a`; `a < 0` → `x <= -b/a` (đổi chiều); `a = 0` → xét `b` để kết luận vô nghiệm hoặc đúng với mọi x.

---

### Bài 20 – Phương Trình Bậc 2 (ax² + bx + c = 0)
**Đề bài:** Nhập a, b, c. Giải phương trình bậc 2 sử dụng Δ = b² − 4ac.

**Ví dụ:** `a = 1, b = -3, c = 2` → `x1 = 2.0, x2 = 1.0`.

**Gợi ý:** Nếu `a == 0`: lùi về phương trình bậc 1. Ngược lại tính Δ: Δ<0 vô nghiệm; Δ=0 nghiệm kép `x = -b/(2a)`; Δ>0 hai nghiệm `x = (-b ± √Δ) / (2a)`.

---

### Bài 21 – Kiểm Tra Chẵn Lẻ
**Đề bài:** Nhập n và kiểm tra số chẵn hay lẻ.

**Ví dụ:** `n = 7` → `7 là số lẻ`.

**Gợi ý:** `n % 2 == 0` thì chẵn, ngược lại lẻ.

---

### Bài 22 – Cùng Tính Chẵn Lẻ
**Đề bài:** Kiểm tra M và N có cùng tính chẵn lẻ không.

**Ví dụ:** `M = 6, N = 8` → `ĐÚNG`.

**Gợi ý:** Hai số cùng tính chẵn lẻ khi `M % 2 == N % 2`; hoặc `(M + N) % 2 == 0`; hoặc `(M - N) % 2 == 0`.

---

### Bài 23 – Ước Số Của Nhau
**Đề bài:** Viết chương trình nhập vào 2 số nguyên a và b, kiểm tra xem chúng có phải là ước của nhau không.

**Ví dụ:** `a = 6, b = 18` → `18 không là ước của 6`, `6 là ước của 18`.

**Gợi ý:** `a` là ước của `b` khi `b % a == 0`. Cần xét cả hai chiều, cẩn thận trường hợp chia cho 0.

---

### Bài 24 – Tìm Giá Trị Nhỏ Nhất Của 2 Số
**Đề bài:** Tìm giá trị nhỏ nhất trong 2 số nguyên a và b (a, b được nhập từ bàn phím).

**Ví dụ:** `a = 15, b = 8` → `8 là giá trị nhỏ nhất`.

**Gợi ý:** Dùng `if a < b` ... hoặc hàm có sẵn `min(a, b)`.

---

### Bài 25 – Tìm Giá Trị Lớn Nhất Của 3 Số
**Đề bài:** Tìm giá trị lớn nhất trong 3 số nguyên a, b, c.

**Ví dụ:** `a = 10, b = 22, c = 15` → `Giá trị lớn nhất trong 3 số là: 22`.

**Gợi ý:** Cách thủ công: gán `max_val = a`, rồi so với b, c. Hoặc dùng `max(a, b, c)`.

---

### Bài 26 – Tìm Giá Trị Lớn Nhất Của 4 Số
**Đề bài:** Tìm giá trị lớn nhất trong 4 số nguyên a, b, c, d.

**Ví dụ:** `a = 10, b = 22, c = 15, d = 45` → `45`.

**Gợi ý:** Mở rộng cách của bài 25; hoặc `max(a, b, c, d)`.

---

### Bài 27 – Tìm Giá Trị Nhỏ Nhất Của 5 Số
**Đề bài:** Tìm giá trị nhỏ nhất trong 5 số thực a, b, c, d, e.

**Ví dụ:** `3.5, 1.2, 4.8, -2.5, 0.0` → `-2.5`.

**Gợi ý:** Nhập 5 số bằng `map(float, input().split())`, rồi dùng `min(...)` hoặc so sánh tuần tự.

---

### Bài 28 – Thực Hiện Phép Toán
**Đề bài:** Nhập vào hai số nguyên và một phép toán (`+`, `-`, `*`, `/`) rồi in ra màn hình kết quả.

**Ví dụ:** `10`, `5`, phép toán `+` → `10 + 5 = 15`.

**Gợi ý:** Dùng `if/elif` cho từng ký hiệu phép toán. Với `/`, nhớ xử lý trường hợp mẫu bằng 0.

---

### Bài 29 – Tìm Số Ngày Của Năm
**Đề bài:** Xác định năm N có 365 hay 366 ngày (năm nhuận). Năm nhuận: chia hết cho 400, hoặc chia hết cho 4 nhưng không chia hết cho 100.

**Ví dụ:** `N = 2024` → `Số ngày của năm 2024 là 366`.

**Gợi ý:** Điều kiện năm nhuận: `(N % 400 == 0) or (N % 4 == 0 and N % 100 != 0)`. Nhuận → 366, không nhuận → 365.

---

### Bài 30 – Đổi Giờ Phút Giây
**Đề bài:** Nhập số giây và đổi thành giờ : phút : giây.

**Ví dụ:** `3665` → `1 giờ : 1 phút : 5 giây`.

**Gợi ý:** `giờ = s // 3600`; `phút = (s % 3600) // 60`; `giây = s % 60`. Có thể dùng `divmod()` cho gọn.

---

### Bài 31 – Đồng Hồ Điện Tử
**Đề bài:** Bảng của đồng hồ điện tử gồm một dãy ba số h, p, s thể hiện tương ứng giờ, phút và giây của thời điểm hiện tại. Cứ sau mỗi giây, giá trị của bộ ba số này sẽ thay đổi tương ứng với thời điểm mới. Hãy tìm và in kết quả ra màn hình.

**Ví dụ:** Nhập `23 59 58` → Xuất `23 59 59`.

**Gợi ý:** Tăng `s` thêm 1. Nếu `s == 60` → `s = 0` và tăng `p`; nếu `p == 60` → `p = 0` và tăng `h`; nếu `h == 24` → `h = 0`. Dạng gọn: chuyển tất cả về tổng giây, cộng 1, rồi chia dư 86400 (số giây trong ngày).

---

### Bài 32 – Giải Hệ Phương Trình Bậc Nhất Hai Ẩn
**Đề bài:** Giải hệ: `ax + by = m` và `cx + dy = n`.

**Ví dụ:** `a=2, b=3, m=8, c=4, d=-1, n=-1` → `x ≈ 0.357`, `y ≈ 2.429`.

**Gợi ý:** Tính các định thức: `D = a*d - b*c`, `Dx = m*d - b*n`, `Dy = a*n - m*c`. Nếu `D ≠ 0` → nghiệm duy nhất `x = Dx/D, y = Dy/D`; nếu `D = 0` và `Dx = Dy = 0` → vô số nghiệm; còn lại vô nghiệm.

---

### Bài 33 – Điểm Thuộc Đường Tròn
**Đề bài:** Nhập vào tọa độ tâm (x0, y0) và bán kính R của một đường tròn. Sau đó nhập vào tọa độ điểm A(xa, ya) bất kỳ và kiểm tra xem điểm A có thuộc đường tròn hay không.

**Ví dụ:** Tâm `(0, 0)`, R = 5, điểm `A(3, 4)` → `Điểm A nằm trên đường tròn`.

**Gợi ý:** Tính khoảng cách `d = sqrt((xa-x0)² + (ya-y0)²)`. So sánh với R: `d < R` nằm trong, `d == R` nằm trên, `d > R` nằm ngoài. Nên dùng so sánh gần đúng với số thực (ví dụ `abs(d - R) < 1e-9`).

---

## Chương 3 – Vòng Lặp Cơ Bản

> Nhắc nhanh: `for i in range(start, stop, step)` để duyệt dãy số; `while` lặp khi điều kiện còn đúng; `break` thoát, `continue` sang vòng tiếp theo.

### Bài 34 – In Các Số Lẻ Nhỏ Hơn n
**Đề bài:** Nhập n, in ra tất cả số lẻ trong [1, n].

**Ví dụ:** `n = 9` → `1 3 5 7 9`.

**Gợi ý:** `for i in range(1, n+1, 2)` sẽ duyệt trực tiếp 1, 3, 5, ...; hoặc duyệt 1..n và kiểm tra `i % 2 == 1`.

---

### Bài 35 – Tính Tổng Từ 1 Đến n
**Đề bài:** Nhập n, tính `S = 1 + 2 + ⋯ + n`.

**Ví dụ:** `n = 10` → `Tổng từ 1 đến 10 = 55`.

**Gợi ý:** Cách 1 — dùng vòng `for i in range(1, n+1)` cộng dồn. Cách 2 — dùng công thức Gauss `n*(n+1)//2`.

---

### Bài 36 – Tổng Các Số Chẵn
**Đề bài:** Nhập n, tính tổng các số chẵn trong [1, n].

**Ví dụ:** `n = 10` → `Tổng các số chẵn từ 1 đến 10 = 30`.

**Gợi ý:** Duyệt bằng `range(2, n+1, 2)` cộng dồn; hoặc dùng công thức `2 + 4 + ... + 2k = k*(k+1)` với `k = n//2`.

---

### Bài 37 – Tổng Các Số Lẻ
**Đề bài:** Nhập vào số n nguyên dương và in ra màn hình tổng các số lẻ từ 1 đến n.

**Ví dụ:** `n = 10` → `Tổng các số lẻ từ 1 đến 10 = 25`.

**Gợi ý:** Duyệt bằng `range(1, n+1, 2)` cộng dồn. Mẹo kiểm chứng: tổng k số lẻ đầu tiên = k².

---

### Bài 38 – Tính Giai Thừa n!
**Đề bài:** Nhập n, tính `n! = 1 × 2 × ⋯ × n`.

**Ví dụ:** `n = 5` → `5 giai thừa = 120`.

**Gợi ý:** Khởi tạo `fact = 1`, rồi `for i in range(1, n+1): fact *= i`. Lưu ý `0! = 1`. Có thể viết đệ quy để luyện (sẽ gặp lại ở chương sau).

---

### Bài 39 – Tính Lũy Thừa aⁿ
**Đề bài:** Nhập cơ số a và số mũ n, in ra kết quả aⁿ.

**Ví dụ:** `a = 2, n = 10` → `2 lũy thừa 10 = 1024`.

**Gợi ý:** Cách 1 — dùng toán tử `**`: `a ** n`. Cách 2 — khởi tạo `res = 1`, lặp n lần `res *= a`. Cả hai đều cho kết quả, nhưng cách 2 giúp hiểu bản chất phép lũy thừa.

---

### Bài 40 – Tổng Các Số Chia Hết Cho 3 Hoặc 5
**Đề bài:** Nhập M và N (M < N), tính tổng các số trong [M, N] chia hết cho 3 hoặc 5.

**Ví dụ:** `M = 10, N = 20` → `Kết quả: 75` (10+12+15+18+20).

**Gợi ý:** Duyệt `for i in range(M, N+1)`, kiểm tra `i % 3 == 0 or i % 5 == 0` thì cộng dồn. (Có thể tối ưu bằng nguyên lý bù trừ: tổng chia hết 3 + tổng chia hết 5 − tổng chia hết 15 — luyện tư duy toán.)

---

*Chúc bạn luyện tập tốt!*
