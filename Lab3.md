# Subsystem context diagrams

- Một số hệ thống con: BankSystem, PrintService, ProjectManagementDatabase subsystems.
  
  + Hệ thống con: BankSystem
    
    ![](https://www.planttext.com/api/plantuml/png/T94xJWCn48RxESKe5HHx0GeK40qIIE7P88g9FGhEPiV2CrlisIWu4bV0tbZ8GD9Plxx_CVBNn-TIZPADmmwq3u8fAYEGivZmIJdLvuLpSHGBidcOr7YeyYh5BJkx9Q4D3onsHKPhKWPOPzvJcl2IfAycA8dOTUUDY6TuBS426IkkQ2efyBVkl-UUtqTM-x7WC-s29mjHe06Bx-Z877CtSWgbUCzqDq5wzlYOI3IVcDCKuEGK5nbmh5hR5aYpfv5cgexWnZ-Z1tJuDVFbBNZFyhgVsyOUeGubBbby-SXl0000__y30000)

  + Hệ thống con PrintService
    
    ![](https://www.planttext.com/api/plantuml/png/T90n2W8n44Nxd6Amqc8lO24MefKWYfLOZCdeHjq4CnF1irbu9AzWDgj21Blay-RzIPxtnvW5WyJchFXa7GJF10gr-01hfl0-Be8_afOvEZnGGqucABX39gLsFZg3uPOOwsH5uMfrYjjXgAfH4SCGbdI9nC8myJgsfWwmxg0AiXlzqveyKn9TKzAa2FPvnRT6zGVGoxTFHG-GeKWoCoFfAWKbSeRAIFsijAcjCUIsdrTzRN-n7z-Od6c_-WK00F__0m00)

  +Hệ thống con ProjectManagementDatabase subsystems.

    ![](https://www.planttext.com/api/plantuml/png/Z94zZi9038LxdyAYWY8Ne5WXHBC54X1H8GgJ69Xbun6sWyJPA3WILo1XWq3yYEr6pzzxVjQS3iUUEQcNnI_O9WXgD4QWpAFYr5YRPvzaa-xDkMY4aGRnb7KNCWR8oMb1bNEayOSp7vBGYWiM7pGJW3eDa-JhFODT_1Fjok2tBACMv24At3fyZ1cNhE4kfXx1VUMF2HFUbcnk5oikhnS7MG6qEzXAQSUDloPQI8OFseMRi5TDdjaNEi3xGibi7VASPLxLVbppFzUhXJsMlFxvCm000F__0m00)

- Hệ thống con (subsystem) là một thành phần độc lập trong hệ thống lớn hơn, thực hiện một chức năng cụ thể hoặc nhóm chức năng liên quan. Mỗi hệ thống con thường có các giao diện (interfaces) giúp nó tương tác với các hệ thống con khác hoặc các phần khác của hệ thống.
 
-  Hệ Thống Con Ngân Hàng (BankSystem): 
    + Mô tả : chịu trách nhiệm quản lý các giao dịch tài chính, bao gồm việc chuyển tiền, truy vấn số dư tài khoản và các giao dịch tài chính khác.
    + Interface - IBankSystem:Giao diện này định nghĩa các phương thức mà hệ thống con BankSystem cần phải triển khai để phục vụ các yêu cầu từ hệ thống chính.
    + Mối Quan Hệ:IBankSystem được sử dụng bởi PayrollController để xử lý các giao dịch thanh toán cho nhân viên.BankSystem được sử dụng bởi PayrollController để xử lý các giao dịch thanh toán cho nhân viên.BankSystem là phần cài đặt của giao diện IBankSystem, thực hiện các chức năng cụ thể của hệ thống ngân hàng.
-  Hệ Thống Con In Ấn (PrintService):
    + Mô Tả:Hệ thống con PrintService chịu trách nhiệm thực hiện in ấn các báo cáo và tài liệu, chẳng hạn như phiếu thanh toán, báo cáo nhân viên, báo cáo tài chính
    + Interface - IPrintService:Giao diện này định nghĩa các phương thức liên quan đến việc in ấn tài liệu trong hệ thống. 
    + Mối Quan Hệ:IPrintService được sử dụng bởi PayrollController để in phiếu thanh toán cho nhân viên hoặc các báo cáo liên quan đến lương.PrintService là phần cài đặt của giao diện IPrintService, giúp thực hiện các công việc in ấn thực tế.
 
- Hệ Thống Con Quản Lý Dự Án (ProjectManagementDatabase)
    + Mô Tả:Hệ thống con ProjectManagementDatabase quản lý dữ liệu của các dự án, bao gồm việc truy vấn thông tin về dự án, cập nhật trạng thái dự án và lưu trữ thông tin liên quan đến các dự án trong cơ sở dữ liệu.
    + Interface - ProjectManagementDatabase:Giao diện này xác định các phương thức mà hệ thống con ProjectManagementDatabase phải cung cấp để thao tác với cơ sở dữ liệu dự án.
    + Mối Quan Hệ:IProjectManagementDatabase được sử dụng bởi ProjectManagementService để truy vấn và cập nhật dữ liệu của các dự án trong hệ thống.
ProjectManagementDatabase là phần cài đặt của giao diện ProjectManagementDatabase, giúp thao tác với cơ sở dữ liệu của các dự án.
  
# Mapping Analysis Class to Design Element

![image](https://github.com/user-attachments/assets/e8c58a1c-4e4f-4994-a91a-764accf770d8)

# Mapping Design Element to Owning Package

![image](https://github.com/user-attachments/assets/99b8e175-e60c-4d4f-8ef9-ea12a131e2d2)

# Architectural Layers and Dependencies

![](https://www.planttext.com/api/plantuml/png/X5J1JW8n4BttAoPUFF43X10GF91W92Wduw6KWMtejhNJ1OdnoppuIVw2xOAukDtrjctVcpTlNhjV7vy3yjpv8bUCjbA3CuJi6iQubXh1PmYA7z0HSBq2ON9hD6fFZ5akjdo3S3LpI66BUsaqJ2Fu2juOmDDYyWoztfdJxyVDaT7U6QNG9Gw7imcCb0phluVl5S6XjKgAkjvDGQ5d8fYQZHJmW6ud1QPaAWKQK5MzCVVyGcYErf3qnXqInIDwoIcbUp-_QzEPQ8yRL_Tr--hHQQwWUJm1zPX9ju9PoFBGOkgSh4DLAb4cBS4I_HvHdx9cPNITJhzvfbsGeLl7XIVOIv-nYs1BQdBAaRSpMmmQLJTj1C6L2l2cJafgDP4kl1Je91AiGXGiNJR1ikZMnkK4e_bY32OiZmDY5xYI-9jnVGurS9bw5meA7OLl229HYoHvr0B_SPOC_pGKm9z3EdBQp3OLCdbUw4Z1euFmvkD5il4YCJP0lOh_Xcy0003__mC0)
