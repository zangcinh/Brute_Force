# Tổng quan
Thực hành tại trang web `https://pmisydney.org/`

![image](https://github.com/user-attachments/assets/3e8f47e9-3c9d-4366-8d3f-4dab4f14b47d)

# Thực hiện

- Vào phần member login

![image](https://github.com/user-attachments/assets/a4856911-d11c-4160-8f3e-c098381d6b08)

- Chọn forgot password và nhập 1 username bất kì

![image](https://github.com/user-attachments/assets/75e0bc6b-9170-48fe-9c54-4f569717fca5)

- Sẽ có một mã xác thực 6 chữ số gửi đến mail của người dùng tên admin
![image](https://github.com/user-attachments/assets/8a27550b-ff06-446a-9c7b-8ec52552a10b)


- Xem request ta thấy có hiện tên mail người dùng trên URL => rò rỉ thông tin
![image](https://github.com/user-attachments/assets/bb9c2cba-c493-4112-a003-eeb9a577854b)

![image](https://github.com/user-attachments/assets/1526dd63-942b-4997-9ca2-4c2d6f335557)


- Đây là request khi nhập mã xác minh, nếu đúng response sẽ trả về `true`, ngược lại sẽ trả về `invalid code`, `incorrect code`
![image](https://github.com/user-attachments/assets/a675e6ea-a151-468e-8be5-35ab7eaf43cc)

![image](https://github.com/user-attachments/assets/e3e332a3-6cc4-4029-910e-968a148c074e)

![image](https://github.com/user-attachments/assets/81d95928-ec27-4c8e-bb8e-482bfeaa96fd)

- Tổng quan, ban đầu trang web có những lỗi như rò rỉ thông tin trên URL, không giới hạn số lần nhập và thời gian mã xác minh lúc đầu là 72h. 1 tiếng sau khi trang web bị brute thì đã đổi thành 2 tiếng, sang sáng hôm sau đã giới hạn số lần nhập và thêm capcha xác minh 
