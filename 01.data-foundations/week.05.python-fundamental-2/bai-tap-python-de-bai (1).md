# Hơn 100 bài tập Python - Đề bài

## Bài tập Python Level 1

### Bài 1
Viết chương trình tìm tất cả các số chia hết cho 7 nhưng không phải bội số của 5, nằm trong đoạn 2000 và 3200 (tính cả 2000 và 3200). Các số thu được sẽ được in thành chuỗi trên một dòng, cách nhau bằng dấu phẩy.

**Gợi ý:** Sử dụng vòng lặp for để duyệt qua tất cả các số trong đoạn từ 2000 đến 3200. Dùng if để kiểm tra chia hết cho 7 và không phải bội 5.

### Bài 2
Viết một chương trình có thể tính giai thừa của một số cho trước. Ví dụ, số cho trước là 8 thì kết quả đầu ra phải là 40320.

**Gợi ý:** Chọn cách để người dùng nhập số vào.

### Bài 3
Với số nguyên n nhất định, hãy viết chương trình để tạo ra một dictionary chứa (i, i*i) như là số nguyên từ 1 đến n (bao gồm cả 1 và n) sau đó in ra dictionary này. Ví dụ: n=8 thì đầu ra: {1: 1, 2: 4, 3: 9, 4: 16, 5: 25, 6: 36, 7: 49, 8: 64}.

**Gợi ý:** Viết lệnh yêu cầu nhập số nguyên n.

### Bài 4
Viết chương trình chấp nhận một chuỗi số, phân tách bằng dấu phẩy từ giao diện điều khiển, tạo ra một danh sách và một tuple chứa mọi số. Ví dụ: Đầu vào 34,67,55,33,12,98 thì đầu ra là: ['34', '67', '55', '33', '12', '98'] và ('34', '67', '55', '33', '12', '98').

**Gợi ý:** Dùng quy tắc chuyển đổi kiểu dữ liệu.

### Bài 5
Định nghĩa một class có ít nhất 2 method: getString (nhận chuỗi do người dùng nhập) và printString (in chuỗi sang chữ hoa). Ví dụ: quantrimang.com → QUANTRIMANG.COM.

**Gợi ý:** Sử dụng __init__ để xây dựng các tham số.

### Bài 6
Viết một method tính giá trị bình phương của một số.

**Gợi ý:** Sử dụng toán tử **.

### Bài 7
Viết chương trình để in tài liệu về một số hàm Python tích hợp sẵn như abs(), int(), input() và thêm tài liệu cho hàm bạn tự định nghĩa.

**Gợi ý:** Sử dụng __doc__.

### Bài 8
Định nghĩa một lớp gồm có tham số lớp và có cùng tham số instance.

**Gợi ý:** Khi định nghĩa tham số instance, cần thêm nó vào __init__. Có thể khởi tạo đối tượng với tham số bắt đầu hoặc thiết lập giá trị sau.

### Bài 9
Tính tuổi dựa trên ngày tháng năm sinh nhập vào (dạng y/m/d).

**Gợi ý:** Sử dụng module datetime. Trừ năm sinh cho năm hiện tại.

### Bài 10
Viết chương trình nhập số giờ làm mỗi tuần, thù lao trên mỗi giờ làm tiêu chuẩn, tính ra số tiền thực lĩnh. Số giờ tiêu chuẩn mỗi tuần là 44 giờ, mỗi giờ vượt chuẩn được trả gấp rưỡi.

---

## Bài tập Python Level 2

### Bài 1
Viết chương trình tính Q = √([(2 × C × D) / H]). Với C = 50, H = 30. D là dãy giá trị tùy biến nhập vào, phân cách bằng dấu phẩy. Ví dụ: D = 100,150,180 → đầu ra 18,22,24.

**Gợi ý:** Làm tròn thành giá trị gần nhất.

### Bài 2
Viết chương trình có 2 chữ số X, Y nhận giá trị từ đầu vào và tạo ra mảng 2 chiều. Giá trị phần tử hàng i cột j = i × j. Ví dụ: X, Y = 3, 5 → [[0,0,0,0,0],[0,1,2,3,4],[0,2,4,6,8]].

### Bài 3
Viết chương trình nhận chuỗi từ phân tách bởi dấu phẩy, in theo thứ tự bảng chữ cái. Ví dụ: without,hello,bag,world → bag,hello,without,world.

### Bài 4
Viết chương trình nhận các dòng nhập vào, chuyển thành chữ in hoa và in ra. Ví dụ: Hello world → HELLO WORLD.

### Bài 5
Viết chương trình nhận chuỗi từ tách biệt bởi khoảng trắng, loại bỏ trùng lặp, sắp xếp theo bảng chữ cái.

**Gợi ý:** Sử dụng set và sorted().

### Bài 6
Viết chương trình nhận chuỗi số nhị phân 4 chữ số phân tách bởi dấu phẩy, kiểm tra chia hết cho 5, in kết quả. Ví dụ: 0100,0011,1010,1001 → 1010.

### Bài 7
Viết chương trình tìm tất cả các số trong đoạn 1000 đến 3000 sao cho tất cả các chữ số đều chẵn. In thành chuỗi cách nhau bởi dấu phẩy.

### Bài 8
Viết chương trình nhận một câu, đếm số chữ cái và chữ số. Ví dụ: hello world! 123 → Chữ cái: 10, Chữ số: 3.

### Bài 9
Viết chương trình nhận một câu, đếm chữ hoa và chữ thường. Ví dụ: Quản Trị Mạng → Chữ hoa: 3, Chữ thường: 8.

### Bài 10
Viết chương trình tính a + aa + aaa + aaaa với a là số nhập vào. Ví dụ: a = 1 → 1234.

### Bài 11
Sử dụng danh sách để lọc các số lẻ từ danh sách người dùng nhập vào. Ví dụ: 1,2,3,4,5,6,7,8,9 → 1,3,5,7,9.

### Bài 12
Viết chương trình tính số tiền thực của tài khoản ngân hàng dựa trên nhật ký giao dịch (D = gửi tiền, W = rút tiền). Ví dụ: D 300, D 300, W 200, D 100 → 500.

### Bài 13
Viết chương trình nhập dãy số nguyên, kiểm tra khả đối xứng, nếu có thì biến đổi thành dãy đối xứng.

### Bài 14
Viết chương trình nhập mảng hai chiều A (m hàng, n cột):

a. Tìm giá trị lớn nhất và nhỏ nhất trên mỗi cột.

b. Tìm phần tử lớn nhất và nhỏ nhất cùng chỉ số hàng, cột.

c. Đếm số phần tử bằng phần tử lớn nhất.

---

## Bài tập Python Level 3

### Bài 1
Viết chương trình kiểm tra tính hợp lệ của mật khẩu theo các quy tắc: ít nhất 1 chữ thường [a-z], 1 chữ số [0-9], 1 chữ hoa [A-Z], 1 ký tự đặc biệt [$#@], độ dài từ 6 đến 12 ký tự. Nhập chuỗi mật khẩu phân tách bởi dấu phẩy, in ra các mật khẩu hợp lệ. Ví dụ: ABd1234@1,a F1#,2w3E*,2We3345 → ABd1234@1.

### Bài 2
Viết chương trình sắp xếp các tuple (tên, tuổi, điểm) theo thứ tự tăng dần. Thứ tự ưu tiên: tên → tuổi → điểm.

**Gợi ý:** Sử dụng itemgetter.

### Bài 3
Xác định một class với generator có thể lặp lại các số trong khoảng 0 đến n mà chia hết cho 7.

**Gợi ý:** Sử dụng yield.

### Bài 4
Một robot di chuyển trong mặt phẳng bắt đầu từ điểm gốc (0, 0). Robot có thể di chuyển theo hướng UP, DOWN, LEFT, RIGHT với số bước nhất định. Hãy tính khoảng cách từ vị trí hiện tại đến điểm gốc sau một loạt các di chuyển. Ví dụ: UP 5, DOWN 3, LEFT 3, RIGHT 2 → 2.

### Bài 5
Viết chương trình tính tần suất xuất hiện các từ từ input, sau đó xuất ra kết quả sau khi sắp xếp theo thứ tự bảng chữ cái.

---

## Bài tập Python khác

### Bài 1
Định nghĩa một hàm có thể tính tổng hai số.

### Bài 2
Định nghĩa một hàm chuyển số nguyên thành chuỗi và in ra.

### Bài 3
Định nghĩa một hàm nhận hai số nguyên trong dạng chuỗi và tính tổng của chúng.

### Bài 4
Định nghĩa một hàm nhận 2 chuỗi từ input và nối chúng lại, in ra kết quả.

### Bài 5
Định nghĩa một hàm có input là 2 chuỗi và in ra chuỗi có độ dài lớn hơn. Nếu bằng nhau thì in cả hai.

### Bài 6
Định nghĩa một hàm nhận input là số nguyên và in "Đây là một số chẵn" hoặc "Đây là một số lẻ".

### Bài 7
Định nghĩa một hàm in ra dictionary chứa key là các số từ 1 đến 3 và các giá trị là bình phương của key.

### Bài 8
Định nghĩa một hàm in ra dictionary chứa key là các số từ 1 đến 20 và giá trị là bình phương của key.

### Bài 9
Định nghĩa một hàm tạo dictionary với key từ 1 đến 20 và giá trị bình phương, chỉ in ra các giá trị.

### Bài 10
Định nghĩa một hàm tạo dictionary với key từ 1 đến 20 và giá trị bình phương, chỉ in ra các key.

### Bài 11
Định nghĩa một hàm tạo và in ra list chứa giá trị bình phương của các số từ 1 đến 20.

### Bài 12
Định nghĩa một hàm tạo list chứa bình phương các số từ 1 đến 20 và in ra 5 mục đầu tiên.

### Bài 13
Định nghĩa một hàm tạo list chứa bình phương các số từ 1 đến 20 và in ra 5 mục cuối cùng.

### Bài 14
Định nghĩa một hàm tạo list chứa bình phương các số từ 1 đến 20 và in ra tất cả trừ 5 mục đầu.

### Bài 15
Định nghĩa một hàm tạo và in ra tuple chứa giá trị bình phương của các số từ 1 đến 20.

### Bài 16
Với tuple (1, 2, 3, 4, 5, 6, 7, 8, 9, 10), hãy in nửa đầu và nửa cuối trên 2 dòng riêng biệt.

### Bài 17
Viết chương trình tạo một tuple chứa các số chẵn từ tuple (1, 2, 3, 4, 5, 6, 7, 8, 9, 10).

### Bài 18
Viết chương trình tạo và in ra tuple chứa các số chẵn từ tuple (1, 2, 3, 4, 5, 6, 7, 8, 9, 10).

### Bài 19
Viết chương trình nhận một chuỗi, in "Yes" nếu chuỗi là "yes" hoặc "YES" hoặc "Yes", ngược lại in "No".

### Bài 20
Viết chương trình lọc các số chẵn trong danh sách [1, 2, 3, 4, 5, 6, 7, 8, 9, 10] bằng hàm filter.

**Gợi ý:** Dùng filter() và lambda.

### Bài 21
Viết chương trình dùng map() để tạo list chứa bình phương của các phần tử trong [1, 2, 3, 4, 5, 6, 7, 8, 9, 10].

**Gợi ý:** Dùng map() và lambda.

### Bài 22
Viết chương trình dùng map() và filter() để tạo list chứa bình phương của các số chẵn trong [1, 2, 3, 4, 5, 6, 7, 8, 9, 10].

### Bài 23
Viết chương trình dùng filter() để tạo danh sách các số chẵn trong đoạn [1, 20].

### Bài 24
Viết chương trình dùng map() để tạo list chứa bình phương các số trong đoạn [1, 20].

### Bài 25
Định nghĩa một class có tên Vietnam với một static method là printNationality.

**Gợi ý:** Dùng @staticmethod.

### Bài 26
Định nghĩa một class có tên Vietnam và một class con có tên Hanoi.

**Gợi ý:** Dùng Subclass(ParentClass).

### Bài 27
Định nghĩa một class Circle được xây dựng từ bán kính, có method tính diện tích hình tròn.

### Bài 28
Định nghĩa một class Hinhchunhat (hình chữ nhật) với chiều dài và chiều rộng, có method tính diện tích.

### Bài 29
Định nghĩa một class Shape và một class con Square. Square có hàm __init__ nhận chiều dài cạnh. Cả hai class đều có hàm area (diện tích mặc định của Shape = 0).

### Bài 30
Đưa ra một RuntimeError exception.

**Gợi ý:** Dùng raise().

### Bài 31
Viết một hàm tính 5/0 và dùng try/except để bắt lỗi.

### Bài 32
Định nghĩa một class exception tùy chỉnh, nhận thông báo lỗi là thuộc tính.

### Bài 33
Viết chương trình in ra username từ một địa chỉ email có dạng username@companyname.com. Ví dụ: QTM@quantrimang.com → QTM.

**Gợi ý:** Dùng \w và regex.

### Bài 34
Tương tự bài 33, nhưng lấy ra companyname từ địa chỉ email.

### Bài 35
Viết chương trình nhận một chuỗi các từ phân tách bằng khoảng trống, in ra các từ chỉ gồm chữ số. Ví dụ: "3 quantrimang.com và 2 python" → ['3', '2'].

**Gợi ý:** Dùng re.findall().

### Bài 36
In ra chuỗi Unicode "Hello world".

**Gợi ý:** Dùng u'string'.

### Bài 37
Viết chương trình đọc một chuỗi ASCII và chuyển sang mã hóa Unicode UTF-8.

**Gợi ý:** Dùng encode().

### Bài 38
Viết comment đặc biệt để chỉ định file nguồn Python sử dụng mã hóa Unicode.

### Bài 39
Viết chương trình tính tổng 1/2 + 2/3 + 3/4 + ... + n/(n+1) với n được nhập từ bàn phím. Ví dụ: n = 5 → 3.55.

**Gợi ý:** Dùng float().

### Bài 40
Viết chương trình tính f(n) với quy tắc: f(n) = f(n-1) + 100 khi n > 0, và f(0) = 0. Ví dụ: n = 5 → 500.

**Gợi ý:** Dùng hàm đệ quy.

### Bài 41
Viết chương trình tính số Fibonacci thứ n với công thức: f(0) = 0, f(1) = 1, f(n) = f(n-1) + f(n-2). Ví dụ: n = 7 → 13.

### Bài 42
Viết chương trình dùng list comprehension để in ra dãy Fibonacci, các số phân tách bằng dấu phẩy. Ví dụ: n = 7 → 0,1,1,2,3,5,8,13.

### Bài 43
Viết chương trình dùng generator để in ra các số chẵn trong khoảng từ 0 đến n. Ví dụ: n = 10 → 0,2,4,6,8,10.

**Gợi ý:** Dùng yield.

### Bài 44
Viết chương trình dùng generator để in ra các số chia hết cho cả 5 và 7 trong khoảng từ 0 đến n. Ví dụ: n = 100 → 0,35,70.

### Bài 45
Viết lệnh assert để xác minh tất cả các số trong danh sách [2, 4, 6, 8] đều là số chẵn.

### Bài 46
Viết chương trình nhận một biểu thức toán học từ người dùng và in ra kết quả. Ví dụ: 35 + 3 → 38.

**Gợi ý:** Dùng eval().

### Bài 47
Viết một hàm tìm kiếm nhị phân (binary search) để tìm một phần tử trong list đã được sắp xếp, trả về chỉ số của phần tử đó.

### Bài 48
Tạo một số thập phân ngẫu nhiên trong khoảng từ 10 đến 100 bằng module random.

**Gợi ý:** Dùng random.random().

### Bài 49
Tạo một số thập phân ngẫu nhiên trong khoảng từ 5 đến 95 bằng module random.

### Bài 50
Viết chương trình xuất ra một số chẵn ngẫu nhiên trong khoảng từ 0 đến 10 (bao gồm cả 0 và 10), sử dụng module random và list comprehension.

**Gợi ý:** Dùng random.choice() để tạo một phần tử ngẫu nhiên từ list.

### Bài 51
Viết chương trình xuất ra một số ngẫu nhiên chia hết cho cả 5 và 7, nằm trong khoảng từ 0 đến 10, dùng module random và list comprehension.

### Bài 52
Viết chương trình tạo một list gồm 5 số ngẫu nhiên trong khoảng từ 100 đến 200.

**Gợi ý:** Dùng random.sample().

### Bài 53
Viết chương trình tạo một list gồm 5 số chẵn ngẫu nhiên trong khoảng từ 100 đến 200.

### Bài 54
Viết chương trình tạo một số ngẫu nhiên nằm giữa 7 và 15.

### Bài 55
Viết chương trình nén và giải nén một chuỗi, sử dụng module zlib.

**Gợi ý:** Dùng zlib.compress() và zlib.decompress().

### Bài 56
Viết chương trình in ra thời gian chạy của phép tính "100 nhân 50" lặp lại 10000 lần.

**Gợi ý:** Dùng timeit().

### Bài 57
Viết chương trình xáo trộn và in ra list [3, 6, 7, 8].

**Gợi ý:** Dùng shuffle().

### Bài 58
Viết chương trình xáo trộn và in ra list [3, 6, 7, 8] sao cho mỗi phần tử đều nằm ở vị trí khác so với ban đầu.

### Bài 59
Viết chương trình tạo một câu gồm ít nhất 2 từ.

### Bài 60
Viết chương trình Python nhập 3 số nguyên dương a, b, c và kiểm tra xem chúng có tạo thành 3 cạnh của một tam giác hay không.

### Bài 61
Viết chương trình Python nhập 3 số nguyên dương a, b, c. Nếu chúng tạo thành tam giác, hãy kiểm tra loại tam giác (đều, cân, vuông, thường).

### Bài 62
Viết chương trình Python nhập một số nguyên n, in ra bảng cửu chương của n.

### Bài 63
Viết chương trình Python nhập một số nguyên dương n, kiểm tra xem n có phải là số nguyên tố hay không.

### Bài 64
Viết chương trình giải phương trình bậc nhất ax + b = 0.

### Bài 65
Viết chương trình giải phương trình bậc hai ax² + bx + c = 0.

### Bài 66
Viết chương trình Python nhập 3 số thực và tìm giá trị lớn nhất trong 3 số đó.

### Bài 67
Viết chương trình Python nhập điểm các môn Toán, Lý, Hóa; tính điểm trung bình và xếp loại học lực.

### Bài 68
Viết chương trình Python tính diện tích tam giác khi biết 3 cạnh (sử dụng công thức Heron).

### Bài 69
Viết chương trình Python nhập n, tính n! (giai thừa của n).

### Bài 70
Viết chương trình Python nhập n, tính tổng S = 1 + 2 + 3 + ... + n.

### Bài 71
Viết chương trình Python nhập n, tính tổng S = 1² + 2² + 3² + ... + n².

### Bài 72
Viết chương trình Python xuất ra tất cả các hoán vị của một danh sách đã cho.

**Gợi ý:** Dùng itertools.permutations().

### Bài 73
Viết chương trình Python nhập n, tính tổng S = 1 + 1/2 + 1/3 + ... + 1/n.

### Bài 74
Viết chương trình Python nhập n, tính tổng S = 1/2 + 1/4 + ... + 1/(2n).
