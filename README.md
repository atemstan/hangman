# Hangman (Đoán chữ) — C

## Cách chạy



Chương trình đọc từ vựng từ file `abc.txt` (mỗi dòng 1 từ, để cùng thư mục với file
chạy). Nếu không có file này, chương trình tự dùng 1 từ mặc định để không bị lỗi.

## Cách chạy test

Chưa có unit test trong bài này.

## Các quyết định thiết kế

- Dữ liệu ván chơi được gom vào 1 struct `HangmanGame`.
- Chữ cái không phân biệt hoa/thường (chuyển hết về chữ thường trước khi so sánh).
- Nhập sai (rỗng, nhiều hơn 1 ký tự, không phải chữ cái, đoán trùng) thì không bị trừ
  lượt và không làm crash chương trình.
- Ván sau không random trùng từ vừa chơi ở ván trước.
- Từ vựng giả định chỉ gồm chữ cái và khoảng trắng.

## Còn thiếu so với đề bài

- Chưa có file `abc.txt` với ≥30 từ.
- Code logic và giao diện đang để chung 1 file, chưa tách thành 2 file riêng (dù các
  hàm logic không gọi printf/scanf trực tiếp).
- Chưa có unit test (đề yêu cầu ≥5 test).
- Chưa làm các phần nâng cao A1–A6.

## Việc tiếp theo nếu có thêm thời gian

1. Tạo file `abc.txt` với ≥30 từ.
2. Tách file thành `game_logic.c/.h` và `main.c`.
3. Viết ≥5 unit test cho: đoán đúng, đoán sai, đoán trùng, thắng, thua.
4. Làm thêm A1 (độ khó) và A2 (gợi ý).

## Dùng AI

*(Ghi rõ phần nào bạn dùng AI hỗ trợ, phần nào tự viết.)*
