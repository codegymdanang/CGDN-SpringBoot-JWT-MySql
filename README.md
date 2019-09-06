# CGDN-SpringBoot-JWT-MySql
## Bắt đầu với file WebSecurityConfig. Nơi mình sẽ khai báo các webservice nào bắt buộc phải login và cái nào không. Đồng thời 
mình nhúng JwtAuthenticationEntryPoint và  jwtRequestFilter vào sử dụng
+ Mục đích của JwtAuthenticationEntryPoint là để reject tất cả các request mà không authenticate vào hệ thống. Nếu 1 request mà không
đăng nhập thì sẽ ném về lỗi 403
+ Mục đích của jwtRequestFilter kiểm tra tất cả các request truyền lên server có hợp lệ hay không bằng việc kiểm tra token trên header
+ JwtTokenUtil có nhiệm vụ sinh ra token dự vào key mình cung cấp trong file application.properties
