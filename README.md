# Hangman (Đoán chữ) — C


Chương trình đọc từ vựng từ file `abc.txt` (mỗi dòng 1 từ, để cùng thư mục với file
chạy). Nếu không có file này, chương trình tự dùng 1 từ mặc định để không bị lỗi.


## Các quyết định thiết kế

- Dữ liệu ván chơi được gom vào 1 struct `HangmanGame`.
- Chữ cái không phân biệt hoa/thường (chuyển hết về chữ thường trước khi so sánh).
- Nhập sai (rỗng, nhiều hơn 1 ký tự, không phải chữ cái, đoán trùng) thì không bị trừ
  lượt và không làm crash chương trình.
- Ván sau không random trùng từ vừa chơi ở ván trước.
- Từ vựng giả định chỉ gồm chữ cái và khoảng trắng.

## Việc tiếp theo nếu có thêm thời gian

1. Tạo file `abc.txt` với ≥30 từ.
2. Tách file thành `game_logic.c/.h` và `main.c` để logic độc lập hoàn toàn với I/O.
3. Viết ≥5 unit test cho: đoán đúng, đoán sai, đoán trùng, thắng, thua.
4. Làm thêm các phần nâng cao (độ khó, gợi ý...).
