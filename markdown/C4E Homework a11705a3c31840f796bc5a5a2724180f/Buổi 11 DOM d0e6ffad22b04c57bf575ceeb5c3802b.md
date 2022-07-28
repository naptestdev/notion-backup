# Buổi 11: DOM

### 1. Chứng minh nhân dân

Tạo hình thẻ CMND bằng HTML, CSS

Thẻ CMND cần có ít nhất những thông tin sau:

- Tên
- Ngày sinh
- Giới tính
- Ảnh đại diện

![Untitled](Buo%CC%82%CC%89i%2011%20DOM%20d0e6ffad22b04c57bf575ceeb5c3802b/Untitled.png)

- Ở dưới sẽ có 3 nút bấm để thay đổi tên, ngày sinh, ... khi bấm vào nút người dùng sẽ được prompt lấy thông tin thay đổi, và dùng innerText để thay đổi giá trị trên CMND
- Ảnh đại diện: tạo một input (type file) và display lên bằng cách như sau: [https://stackoverflow.com/questions/61302149/why-use-url-createobjecturlblob-instead-of-image-src](https://stackoverflow.com/questions/61302149/why-use-url-createobjecturlblob-instead-of-image-src)

![Untitled](Buo%CC%82%CC%89i%2011%20DOM%20d0e6ffad22b04c57bf575ceeb5c3802b/Untitled%201.png)

- Nếu ảnh đại diện không vừa size có thể tham khảo thuộc tính object-fit cover

### 2. Tic Tac Toe

Tạo giao diện tic tac toe bằng HTML CSS

Tạo hàm checkWinner rồi alert kết quả khi có người thắng (hoặc hoà)

Gợi ý, sử dụng array dưới dạng sau: 

```jsx
[
	[0, 0, 0],
	[0, 0, 0],
	[0, 0, 0]
]
```