# Setup

- Clone project: https://github.com/naptestdev/ecommerce.git cả branch master và admin
- Ở mỗi cái chạy “npm install” ở cả / và /client

### Env ở master branch

- MONGODB_URI là connection uri đến mongodb atlas
    - Import vào atlas từ branch sau [https://github.com/naptestdev/ecommerce/tree/data](https://github.com/naptestdev/ecommerce/tree/data)
    - có 3 file json là banners, categories, products, import vào db với 3 collection đúng tên như trên
    
    Sau khi test một lúc cái mongodb atlas sẽ có những collection như sau 
    
    ![Untitled](Setup%20a5f690fcbd6b4ff2bd61770253fdb448/Untitled.png)
    
- JWT_SECRET_TOKEN như kiểu password, nên dùng thống nhất và có thể dùng một cái UUID là hợp nhất (VD: 9a21b149-b4f1-4aa0-a598-8d411eab5b84)
- CLIENT_ID, CLIENT_SECRET, REFRESH_TOKEN dùng để gửi mail bằng gmail oauth2 không bị đưa vào spam. Hướng dẫn tạo: [https://youtu.be/-rcRf7yswfM](https://youtu.be/-rcRf7yswfM)
- EMAIL: là cái email dùng để send email với oauth 2 như trên
- VNP_TMNCODE và VNP_HASHSECRET dùng VNPay để thanh toán môi trường test
    - Vào [https://sandbox.vnpayment.vn/devreg](https://sandbox.vnpayment.vn/devreg) và tạo một tài khoản (môi trường test)
    - Verify email
    - Chờ một mail chứa title như sau “Thông tin tích hợp cho Merchant Cổng TT VNPAY” - Save lại email đó để sử dụng **vnp_TmnCode và vnp_HashSecret**

### Cái .env hiện tại đang xài

![Untitled](Setup%20a5f690fcbd6b4ff2bd61770253fdb448/Untitled%201.png)

## .env ở admin

- Chỉ cần MONGODB_URI và JWT_SECRET_TOKEN giống hệt ở master branch