# Phân tích ca sử dụng Login
- Các thành phần chính :
    + User: Người dùng của hệ thống, có thể là nhân viên hoặc quản trị viên.Cần đăng nhập để truy cập các chức năng của hệ thống PayRoll như quản lí thời gian làm việc hoặc xử lý bảng lương.
    + UI: Nơi người dùng nhập tên đăng nhập và mật khẩu.
    + Authenticator: Lớp thực hiện việc xác thực thông tin đăng nhập của người dùng, lấy thông tin từ UI và gửi yêu cầu đến PayRollDatabase để xác minh tính hợp lệ.Nếu thông tin chính xác         người dùng sẽ được đăng nhập thành công, nếu không quyền truy cập sẽ từ chối. 
    + PayrollDatabase: Cơ sở dữ liệu lưu giữ thông tin người dùng, bao gồm tên đăng nhập và mật khẩu.
- Biểu đồ sequence cho ca dử dụng Login:
  ![](https://www.planttext.com/api/plantuml/png/T54zJiCm6DrzYZV2q0jaG4L2WYw8WKXT7IV2LXEdE5-gTaGTcRX1AyG0KWSa92Hdw91Un2VW2jYXGvkApNxV-_lidsOxh8WRgekSSK6bGLnbXYLbhLDk5eX7J9IQJ9dZiYQPQLA2UnfBEV64Lndk-C9FywlzdR5WWC65bqQubSvkfg3sGsFtiblg1-W_QDQkKFWJOUA1zvh5eo0w2ebmxPgD0idsooj9zKpO4Jl8UsKYZDkrGA6qF31XFHO6fy7tnjbNp5ppX8cpMy9Z7O1vi2Ffcazn6XuM_aTtvjDNleJeEiZIsU_EnxuH4cVNwdo_VtYy23VADKlT1JqV-h1XfjFmLRy0003__mC0)
  
