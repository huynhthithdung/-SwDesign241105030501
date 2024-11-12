# Phân tích ca sử dụng Login
- Các thành phần chính :
    + User
    + UI
    + Authenticator
    + PayrollDatabase
- Biểu đồ sequence cho ca dử dụng Login:
  ![](https://www.planttext.com/api/plantuml/png/T54zJiCm6DrzYZV2q0jaG4L2WYw8WKXT7IV2LXEdE5-gTaGTcRX1AyG0KWSa92Hdw91Un2VW2jYXGvkApNxV-_lidsOxh8WRgekSSK6bGLnbXYLbhLDk5eX7J9IQJ9dZiYQPQLA2UnfBEV64Lndk-C9FywlzdR5WWC65bqQubSvkfg3sGsFtiblg1-W_QDQkKFWJOUA1zvh5eo0w2ebmxPgD0idsooj9zKpO4Jl8UsKYZDkrGA6qF31XFHO6fy7tnjbNp5ppX8cpMy9Z7O1vi2Ffcazn6XuM_aTtvjDNleJeEiZIsU_EnxuH4cVNwdo_VtYy23VADKlT1JqV-h1XfjFmLRy0003__mC0)
  
- Biểu đồ lớp cho ca dử dụng Login:
  ![](https://www.planttext.com/api/plantuml/png/b59BQiCm4Dth5BDqeBv05oNzBRe814eECB6cZc0i1Squ8PIUB8iUALU8bDXrxPP2jT4my_IUtfDEny-vA4Pj6pPCRmeQ8Bfwes1Tf4fTyCPKZ2Am4ehmRY2jiasrnuPkuLMZy_MrkqsmVOXsr8MQTDN1YzcFqR8xystqyQNuqkbbuBDNYcJ_eEeGlp1U4DR9bl6m816igMYkUuz9u5rmTX2_RtL3Nbs56dhVW4EJYca8Dp0D894-XC24Vk1TuY46vYTKNADGpxn3TZQnFYO7MG5P_YrmUQ6ol4l1cPHThaOkpDXJdazkO-RaRVuBPm000F__0m00)
  
- Giải thích:
  + User: Người dùng của hệ thống, có thể là nhân viên hoặc quản trị viên.Cần đăng nhập để truy cập các chức năng của hệ thống PayRoll như quản lí thời gian làm việc hoặc xử lý bảng lương.
  + UI: Nơi người dùng nhập tên đăng nhập và mật khẩu.
  + Authenticator: Lớp thực hiện việc xác thực thông tin đăng nhập của người dùng, lấy thông tin từ UI và gửi yêu cầu đến PayRollDatabase để xác minh tính hợp lệ.Nếu thông tin chính xác         người dùng sẽ được     đăng nhập thành công, nếu không quyền truy cập sẽ từ chối. 
  + PayrollDatabase: Cơ sở dữ liệu lưu giữ thông tin người dùng, bao gồm tên đăng nhập và mật khẩu.
#  Phân tích ca sử dụng Maintain Employee Information
- Các thành phần chính:
  + User
  + UI
  + EmployeeManager
  + PayrollDatabase
- Biểu đồ sequence cho ca sử dụng Maintain Employee Information:
  ![](https://www.planttext.com/api/plantuml/png/h9GzJiCm5CTtd-9TW0jaG4KKGIMA65gfgvj6jKNYH8bJqH4nC7041beGGYgg662A1mQVn2VW2Zo73dNQLAdK354IlV-7Vq_Ah_ffPPAcCez2ajrm0McS1K2eB-CKJaOH5poJASKtak0Oztb2XOH-ntazYv8mdWP1bmew3jpHQpfDup1iKqc7D0i8SLpXw1ZDFEWQzGn3RjHz3f4fFd8GJBy8c72z4AJViNEEq8CBEor0CgCU7UdsX2jcYcK24ps3iL5B3YEZFY54tKDEQ2YXn_GYMez5D_N42U3rNw1oJ0_EgqOryehGUbMmUAjuoVIt68F4JMotgkYsrXhekOzoFA_5WxPr9ImN1-CgVgZdiNsU2GQ-_KA24BDEIuAbiNJgCNjuz335V4zUVerbOsoNfdYRrc7RwDM4NYyrnIjCZBghiMtSpU6rmslVdQv3Ez1g1_gBRlJQkSLEsq6DdTu5tA9DOpnbvW6nx0hV0uSOaHRUx1_n3m00__y30000)
- Biểu đồ lớp cho ca sử dụng Maintain Employee Information:
  ![](https://www.planttext.com/api/plantuml/png/R599JiGm4Bpx5NqC4lb0XD0W0L8EaP3GFA07cs1XkoEtCwDeu6KSU19VmCuoMS2Ns9NghkgoVxw-TnpGXzOQmU_QWITM85uCCiEUbOUpWBXoQEEXb0Le5nQ8GwiAU0vUktg4crXw8YzNC82XMhlige03aL7enASOPUwarKvpy1XeqWEmwB1M3xOnr2bLkbTAnKVISgxSbnUwrDmOx1x9smjl-5EhS8y14rfXCuByHgTACKU9p0xVoUyVbSb3rJkQ7HxHQ8b1zTtZ1dk1nOG3hMqIgHzWILfhF67doPZKwe3n1iwp-Ka-qqFwgpc6vblADVodr5_dpKUUhnCNw_pp_3RcAcAqQRUPNMopI9oDTx5JJgRtz0i00F__0m00)
  
- Giải thích:
  + User: Người dùng chính có quyền thực hiện bảo trì và cập nhật thông tin của nhân viên trong hệ thống. Họ có thể thêm, chỉnh sửa hoặc xóa thông tin nhân viên.
  + UI:Giao diện cung cấp các biểu mẫu (forms) và chức năng để tìm kiếm, hiển thị, và chỉnh sửa thông tin nhân viên. Nó cho phép Administrator nhập thông tin mới hoặc cập nhật thông tin hiện có của nhân viên.
  + EmployeeManager:Lớp xử lý các yêu cầu của người dùng liên quan đến quản lý thông tin nhân viên. Lớp này thực hiện việc kết nối giữa UI và cơ sở dữ liệu, xử lý logic và kiểm tra tính hợp lệ của dữ liệu trước       khi gửi đến cơ sở dữ liệu.
  + PayrollDatabase:Cơ sở dữ liệu lưu trữ thông tin chi tiết của nhân viên, bao gồm họ tên, địa chỉ, thông tin liên hệ, và các thuộc tính liên quan khác. PayrollDatabase thực hiện truy vấn, cập nhật, thêm mới         hoặc xóa thông tin nhân viên theo yêu cầu từ EmployeeManager.

# Phân tích ca sử dụng Maintain Purchase Order
- Các thành phần chính:
  + User
  + UI
  + PurchaseOrderManager
  + PayrollDatabase
- Biểu đồ sequence cho ca sử dụng Maintain Purchase Order:
  ![](https://www.planttext.com/api/plantuml/png/Z5CnJiCm5DrzYdS1Bf01TK222hLqe1AhwqPDrCI97ASI8s9WO69Yf15YG50n04AAXmv1tCCdu0fyDqKYfPHwiBwT_zx_x_tuqynRcUPAvt74id4eePBC1-D29mhzp5SifQ-X25CkDVhjnh6NAn7mp3zIGrzrkEIZbVmUFrL95ErnpGUKnsWvJkpi4fM7ZZKt68JMdEU8RVcGu_tgev2qs_9D8wYcSeGuvwpVNa08wk70vKlem9hB_y2DQjt0bhCKasgAaJMp44DhdX0HmyKtTWbQL5idpiF-HkGwp8AhwOE7GzTt3AquTFKe0ufiMP3QSP2mbUo_cpacq2qcrfoH7TKBmJLDy3SXZpIwjfpdo0WWaP8Jzp54zUmkNYK3hQrxhotu8HiYI20fXCZToPPtQKsvhP2JgX34GFEH3JytzUL6slWNbXOCgY9nyPHC4Ew6-H7LNgD_N0Esis5ZkSYQwv3vSiXQjBctz0K00F__0m00)

- Biểu đồ lớp cho ca sử dụng Maintain Purchase Order:
  ![](https://www.planttext.com/api/plantuml/png/R58xRiCm3Drr2exka0juA38K1J84BP3q08obE49bqI3b147HatNeaNg5oXybLcilieZt-DuZzVFrlPQ07Bh6ANct7fZ4WAeSYi2R68OF1V5RGHSl6rs2zM5MyTYO4dQ1hQ-dSXkf5sATbG4SrTON3oKSY9n1hpvLajbC8W3QIklm-jfnTK8nBwmDFnCtFUzCLa-mseGCyeG1UyWMsmaX9xfiZGZMfcZ6C_b9hMxwMQij-eZbcwCpEgincFzwiOg3v2pJoAdO_6Law5aICLuFW3tjkhPrTWbwTufN9kTw-KFiV3CPvv7O6t-aGj9bt5S-cGL5Ig4M75RaZvQRCSK0l7TDxeQ7ibeznbMgkCt-RsceQd7I0peFfjRHPFyaVm400F__0m00)
  
- Giải thích:
- 
  + User:Người dùng là người tương tác với hệ thống,có thể là Administrator (quản trị viên) hoặc một nhân viên có quyền hạn quản lý đơn đặt hàng.
  + UI:UI cung cấp giao diện để người dùng tương tác với hệ thống, bao gồm các màn hình để nhập thông tin đơn đặt hàng, hiển thị kết quả và thông báo cho người dùng.
  + PurchaseOrderManager:Lớp này chịu trách nhiệm xử lý các thao tác liên quan đến đơn đặt hàng mua, bao gồm việc xác minh và gửi đơn đặt hàng tới nhà cung cấp.
  + PayrollDatabase:Cơ sở dữ liệu này lưu trữ thông tin về các đơn đặt hàng và nhà cung cấp, giúp hệ thống quản lý thông tin và xử lý các giao dịch liên quan đến đơn đặt hàng.


# Phân tích ca sử dụng Run Payroll
- Các thành phần chính:
  + User
  + UI
  + PayrollManager
  + PayrollDatabase
- Biểu đồ sequence cho ca sử dụng Run Payroll:
  ![](https://www.planttext.com/api/plantuml/png/Z5AxJiCm5Dtz5NS4gVn01bG99AX44GELM1qtIYmIktBSIXqH0mCZCw81iO0gEZ35GmTB-Gz_0R_0TH-GFbHrYMwkZyyzv_Z-c6aprrJfVfQI_9OBK3AFW52cfO9E7YdImrFEU8yA3PtMokyL7IgPfcqgQBo6N1oTKar3caU4U2uuEaQA0DhEl43CgOGkT-P1WBPZaK1QJQf2nAJJcW7nGW3d2BX7GEBC8txjjuX1eypGbMzO_bsfiLychXptwk21CtSW4lkA9RSVee73dNc6r8uoxA04ra1yDK5T8iPIEVEvaB7gCO0pPyPyXv9LV8rX6KK05wvy7zOfQjB86dgRX6k58-UcTfDiYlZdc2MkfIt4KZeSXFWYiJDFsKOOsEYxSdguZxsJMVp2lu9UImS6TYI1LGNaVWMwpdn1wlFlx-FxnXPipYk0rOPi4UNtODlgXBQGlXwXUUOxf1c9hb_-Nm000F__0m00)

- Biểu đồ lớp cho ca sử dụng Run Payroll:
  ![](https://www.planttext.com/api/plantuml/png/b59BJiCm4Dtx5BCi4hb05gWBGCeY4XBY09Du21QE9_ZJAgeu6GkEn1LmKgTj6h8WcoHltlEyUUEVh--jysXzQBLmxyg0PKSWQetEmOiZ2mS1ySaWn9z2vg2Clq0CjfJ3ixVAD0dkedJFLivW0CsDCfkR72fcJMWIREaZaFDFs5lMUgZlM4dnAIOFHN8089NhDFQ9-iYsFT6FX8RyGzjfxedkqUDGBR5BHVV6-vASmuOsxV4zELmqJIrAD95bJmPsg9L4JxCc4S2npsAq6dKTTEHFmr7IfHYZG7AeD2L-wEIPF9vz9RYDsOx5IRXcV11N61TvM2PJc5V-myavgCXDnwnGrqt_n_1ukRBiBcvOn2KFN_FOnTKMBXZJV69BHWvNznS00F__0m00)

- Giải thích:
  + User:Người dùng có quyền truy cập vào hệ thống,người này thực hiện thao tác tính toán bảng lương.
  + UI:Giao diện để người dùng nhập và xem thông tin liên quan đến bảng lương, bao gồm các thông tin về nhân viên, số giờ làm việc, và các khoản trừ khác.
  + PayrollManager:Lớp này chịu trách nhiệm thực hiện tính toán lương cho tất cả nhân viên, bao gồm các khoản lương cơ bản, thưởng, thuế, và các khoản trừ.
  + PayrollDatabase:Lưu trữ thông tin về các nhân viên, lương của họ, các khoản thưởng, khoản trừ, cũng như các giao dịch đã được xử lý trong hệ thống.


# Phân tích ca sử dụng Select Payment Method
- Các thành phần chính :
  + User
  + UI
  + PaymentMethodManager
  + PayrollDatabase
 
- Biểu đồ sequence cho ca sử dụng Select Payment Method:
  ![](https://www.planttext.com/api/plantuml/png/Z9AnJiCm441tVyNz03-G0LMY4dI8n1A9zUfOiKLwZX8pC7TWG0ny08A8YQ5IaLZ00uDH_iDVm2zmAHtIggqwsMVVlNi--TT_Zng7jRkPbQAvDWIrRHG8bCxMa3Mg5XNV6cag90VPP2EynDkP8fSgfssU8c6nbSy9jItBCJgSOgE4w8bmSigW1DBedw4mQ24tqTyHI1tz0q6bksNNKW6EupV92v86PqDB8fkigfcIm0LNpMcLTGzbzEzu565WS7PimrqFJU0y-eKvL0q_Z-5rBILsCTRiuOpOAdujAY3DYpj8bze25Tqo-YS3UVYaGcp1zhjVXLR-zs3EeE5UpNvU6nDtEdomrpIqjj-_i9RiJyH8KTv_fpy0003__mC0)

- Biểu đồ lớp cho ca sử dụng Select Payment Method:
  ![](https://www.planttext.com/api/plantuml/png/Z58nRiCm3Dpr2euEK7_0Gv6XYmS31O8-W8bOHwWi6QBi80ZwiWvzKhzGsfLRsqsHQg5qu977epxUthSSCSIkiOfVZ8FWcK0TB3B34rE0Ym8vENJoA7K1niKPuh2X0dOn65Sdk1NgoGUzW06ihutBDWNilRU4Bi5CbWxn4SyDkLXHF7gTDMEO-4BflT7gLKsooYGAG1jkBPuNTCucnbTEJN4tDY6zRBDPAUIZFrN4Z3M9X37-gM5HgK8dkU5RLO_MQ8nqOwgL4TYl23F7x-269y8Ctje7ZBX7sU3bP_XXYwLxzlDwmg-mJJbT-rli_tgF7oJFxsKbIhOotAuPewwwbRBdijMMd1w-uYS0003__mC0)

- Giải thích :
  + User:Người dùng có quyền truy cập vào hệ thống, người này thực hiện việc chọn phương thức thanh toán cho bản thân hoặc cho nhân viên.    
  + UI:Giao diện để người dùng chọn phương thức thanh toán (chẳng hạn như chuyển khoản ngân hàng, tiền mặt, séc, v.v.) và hiển thị các tùy chọn phương thức thanh toán cho người dùng.
  + PaymentMethodManager:Lớp này chịu trách nhiệm xử lý lựa chọn phương thức thanh toán của người dùng. Nó sẽ lưu trữ và cập nhật thông tin phương thức thanh toán đã chọn vào hệ thống.
  + PayrollDatabase:Cơ sở dữ liệu lưu trữ thông tin của người dùng, bao gồm các phương thức thanh toán đã chọn và các thông tin liên quan đến tiền lương.
