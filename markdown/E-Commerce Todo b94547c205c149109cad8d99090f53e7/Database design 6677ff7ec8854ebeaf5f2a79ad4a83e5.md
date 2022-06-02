# Database design

Các collections

- users (chứa các user được đăng ký)
    - email
    - password
    - username
    - emailVerified
    - address
        - fullName
        - phoneNumber
        - city
        - district
        - exactAddress
- products
    - category (ref đến collection “categories”)
    - images: array các link
    - description
    - name
    - price (giá tiền đã sale)
    - originalPrice (giá tiền gốc)
    - stock
    - ratings (trung bình ratings)
    - ratingsCount (đếm số người đã rate)
- reviews
    - user (ref đến collection “users”)
    - product (ref đến collection “products”)
    - ratings
    - comment
- carts
    - user (ref đến collection “users”)
    - products: array
        - product (ref đến collection “products”)
        - quantity
- orders
    - user (ref đến collection “users”)
    - products: array
        - product
        - quantity
    - amount (giá tiền của đơn hàng)
    - address: object
    - status: trạng thái của đơn hàng, có các enum từ 0-3
        - 0: Pending
        - 1: Delivering
        - 2: Completed
        - 3: Cancelled
- categories
    - name
    - image
- banners (chứa các thông tin ảnh quảng cáo ở trang chủ)
    - name
    - image

### Ref trong mongodb có cách define như sau

![Untitled](Database%20design%206677ff7ec8854ebeaf5f2a79ad4a83e5/Untitled.png)

khi query dùng hàm `***populate***` để JOIN cái ref đó