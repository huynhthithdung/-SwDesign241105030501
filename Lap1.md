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
- 
   +)	Tầng giao diện người dùng(Presentation):
  
      Chức năng:Tầng này quản lý việc tương tác với người dùng , bao gồm hiển thị thông tin,
                  nhận đầu vào và cung cấp phản hồi cho người dùng.
  
      Thành phần:Các giao diện người dùng như trang web, ứng dụng di động, hoặc giao diện desktop.
  
      Ý nghĩa: Tầng này tách biệt giao diện và logic nghiệp vụ, giúp dễ dàng thay đổi
               cách hiển thị thông tin mà không ảnh hưởng đến logic xử lý của hệ thống.
  
   +)Tầng ứng dụng:
  
      Chức năng: Xử lý các quy tắc nghiệp vụ, như tính toán tiền lương,
                 xác thực và xử lý dữ liệu chấm công, cũng như xử lý thanh toán.
  
      Thành phần: Các controller và dịch vụ như PayrollService, TimeTrackingService.
  
      Ý nghĩa: Tầng này đảm nhận logic nghiệp vụ, đảm bảo rằng các quy trình xử lý nghiệp vụ có thể được tái sử dụng
                 và thay đổi dễ dàng mà không ảnh hưởng đến các tầng khác.

  +) Tầng dữ liệu:
  
      Chức năng: Quản lý việc truy xuất, lưu trữ, và cập nhật dữ liệu trong cơ sở dữ liệu.

     Thành phần: Các thành phần truy cập dữ liệu như Repository và DAO (Data Access Object).

     Ý nghĩa: Tách biệt việc quản lý dữ liệu giúp dễ dàng thay đổi cách
              thức lưu trữ (chẳng hạn như thay đổi từ SQL sang NoSQL) mà không ảnh hưởng đến các tầng khác.

  
package:
  ![](https://www.planttext.com/api/plantuml/png/X98z2eCm68Rtd2AuUmCHXNOGEaYBK-aGqeyIZ2OaQI4KJzQXH-eLwa-fCLRh5B-yoVFoaDVZcMX3bBbM7EcIrLW93KWIMf8Bu21NeA4sn31Hunsne09yHxZzZjjASc41Yko4ewZ8udYOvyGgmRa_teCKoZZJPgIaKd96ro07K3T6eJlyMNguvS00_hdVeB73XXY2Kqf1wuKEtKMQ6Q5iTyluvpNv5nlwhAJQLXEvOHZFHI3NSv_mH237UBy_zU0mlcec8ASWcabsWPEW9zi1kx44wdFtuDu0003__mC0)
  
