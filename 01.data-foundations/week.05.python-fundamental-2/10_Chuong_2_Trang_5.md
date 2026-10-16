# CẨM NANG PYTHON TOÀN TẬP

**CHƯƠNG – 2 | Trang – 5/5**

## 2. CÁC CÂU LỆNH ĐIỀU KHIỂN LUỒNG (tiếp theo)

### ★ Thực hành tốt (Best Practices)

- Giữ điều kiện đơn giản, dễ đọc.
- Dùng tên biến rõ nghĩa.
- Tránh lồng if-else quá sâu; dùng early exit hoặc function.
- Thụt lề nhất quán (khuyến nghị 4 spaces).
- Kiểm tra tất cả các trường hợp điều kiện có thể.

**Các lỗi thường gặp**

- Dùng `=` thay vì `==` trong điều kiện.
- Quên dấu hai chấm (`:`) ở cuối if, for, while, def, v.v.
- Thụt lề sai gây lỗi.
- Loop vô hạn (ví dụ: quên cập nhật biến trong while).
- Dùng quá nhiều điều kiện lồng nhau.

### ★ So sánh các câu lệnh Control Flow

| Câu lệnh | Mục đích | Thực thi | Lặp lại | Dùng khi nào |
|---|---|---|---|---|
| `if` | Kiểm tra điều kiện | Một khối | Không | Muốn chạy code nếu điều kiện True |
| `if-else` | Chọn giữa hai hướng | Một khối | Không | Muốn chạy một trong hai lựa chọn |
| `if-elif-else` | Chọn giữa nhiều hướng | Một khối | Không | Có nhiều điều kiện khác đi |
| `for loop` | Duyệt qua sequence | Khối nhiều lần | Có | Biết trước số lần lặp |
| `while loop` | Lặp khi điều kiện True | Khối nhiều lần | Có | Không biết trước số lần lặp |
| `break` | Thoát loop | Dừng loop | – | Khi điều kiện thỏa và loop nên dừng |
| `continue` | Bỏ qua vòng hiện tại | Bỏ qua vòng hiện tại | – | Muốn bỏ qua vòng lặp hiện tại |
| `pass` | Không làm gì | Không làm gì | – | Cần một câu lệnh về mặt cú pháp |

### ★ Ví dụ thực tế (Real-Life Analogy)

| Khái niệm | Ví dụ thực tế |
|---|---|
| `if` | Nếu trời mưa, mang theo dù. |
| `if-else` | Nếu trời mưa, mang dù, ngược lại thì tận hưởng ngày nắng. |
| `for loop` | Mỗi ngày trong tuần, học 2 tiếng. |
| `while loop` | Khi nào công việc chưa xong, tiếp tục làm. |
| `break` | Ngừng đọc sách khi buồn ngủ. |
| `continue` | Bỏ qua show TV yêu thích để làm bài tập. |
| `pass` | Giữ chỗ ngồi (chưa làm gì cả). |

### ★ Flowchart (Ví dụ)

**Kiểm tra một số là dương, âm hay bằng 0.**

```text
          Bắt đầu
             ↓
          [n > 0?]
        Có ↘     ↓ Không
          Dương [n < 0?]
               Có ↘   ↓ Không
                 Âm   Bằng 0
                        ↓
                    Kết thúc
```

### Luyện tập nhỏ (Tự làm)

1. Viết chương trình kiểm tra một số có chia hết cho cả 5 và 7 hay không.
2. Viết chương trình tính tổng n số tự nhiên đầu tiên bằng for loop.
3. Viết chương trình hỏi số liên tục cho đến khi người dùng nhập 0, rồi hiển thị số lượng đã nhập.

**Ghi chú cuối**

- Nắm vững control flow để xây dựng logic cho chương trình.
- Luyện tập các chương trình nhỏ mỗi ngày.
- Càng luyện tập, bạn càng tự tin hơn!
