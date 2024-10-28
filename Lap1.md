1.Phân tích kiến trúc:
- Đề xuất kiến trúc : Kiến trúc  tầng.
   Kiến trúc này chia hệ thống thành ba tầng:
  
    +)	Tầng giao diện người dùng(Presentation Layer)
  
    +)  Tầng ứng dụng(Application Layer)
  
  	+)  Tầng truy cập dữ liệu(Data Access Layer).
  
- Lý do lựa chọn kiến trúc này:
  Mỗi tầng thực hiện chức năng độc lập, cho phép thay đổi một tầng mà không ảnh hưởng đến các tầng khác, đặc biệt hữu ích khi cần bảo trì hoặc nâng cấp hệ thống.Các tầng có thể dễ dàng mở 
  rộng hoặc điều chỉnh để đáp ứng các yêu cầu mới mà không làm thay đổi toàn bộ hệ thống, được tách biệt hỗ trợ kiểm thử đơn vị và kiểm thử tích hợp tốt hơn, đảm bảo logic nghiệp vụ và xử 
  lý dữ liệu chính xác.Các tầng tách biệt theo chức năng giúp hệ thống dễ bảo trì và kiểm tra lỗi, cải thiện năng suất quản lý và bảo trì hệ thống.
- Ý nghĩa từng phần trong kiến trúc:
  
   +)	Tầng giao diện người dùng(Presentation):Đây là tầng chịu trách nhiệm hiển thị thông tin và cung cấp giao diện để người dùng tương tác với hệ thống.
  
   +)Tầng ứng dụng (Application Layer):Tầng trung gian, xử lý các yêu cầu từ tầng giao diện và điều phối nghiệp vụ. Tầng này thực hiện các quy trình logic nghiệp vụ và đảm bảo tính nhất                                           quán của dữ liệu khi có thay đổi.
  
  +) Tầng dữ liệu(Data Access Layer):Tầng chịu trách nhiệm truy xuất, lưu trữ, và quản lý dữ liệu của hệ thống, đảm bảo tính toàn vẹn và nhất quán của dữ liệu.
  
      
  
package:
  ![](https://www.planttext.com/api/plantuml/png/X98z2eCm68Rtd2AuUmCHXNOGEaYBK-aGqeyIZ2OaQI4KJzQXH-eLwa-fCLRh5B-yoVFoaDVZcMX3bBbM7EcIrLW93KWIMf8Bu21NeA4sn31Hunsne09yHxZzZjjASc41Yko4ewZ8udYOvyGgmRa_teCKoZZJPgIaKd96ro07K3T6eJlyMNguvS00_hdVeB73XXY2Kqf1wuKEtKMQ6Q5iTyluvpNv5nlwhAJQLXEvOHZFHI3NSv_mH237UBy_zU0mlcec8ASWcabsWPEW9zi1kx44wdFtuDu0003__mC0)
  
