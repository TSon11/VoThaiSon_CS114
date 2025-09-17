
# HỆ THỐNG PHÂN LOẠI RÁC THẢI

Mô hình có khả năng phân loại rác tự động – giải pháp tối ưu cho vấn đề nhân công. \
Ngôn ngữ lập trình: Python


## Mục lục
+ Giới thiệu môn học
+ Thành viên	
+ Thông tin đồ án

## Giới thiệu môn học
+ Tên môn học: Máy học - Machine learning
+ Mã môn học: CS114
+ Mã lớp: CS114.O11.KHCL
+ Năm học: HK1 (2023 - 2024)
+ Giảng viên: Phạm Nguyễn Trường An, PGS.TS Lê Đình Duy
## Thành viên
| MSSV | Họ và tên     |
| :-------- | :------- | 
| 21521388    | Võ Thái Sơn |
| 21521873 | Đinh Hoàng Tâm Bình |

## Thông tin đồ án
**2.1 Mô tả bài toán** \
**Input**: hình ảnh chứa các đối tượng rác thải thuộc một trong bốn loại: nhựa, thủy tinh, kim loại và giấy. \
Một hình ảnh có thể có nhiều loại rác thải, với kích thước 640 x 640. Có chất lượng tốt, nhìn rõ được các vật thể, không bị mờ hoặc nhiễu.\
**Output**: ma trận đa chiều có kích thước n x 6. \
Với n là số lượng bounding boxes xung quanh vật thể mà mô hình nhận dạng được. Và 6 cột là các thông số của một bounding box bao gồm tọa độ x, y của điểm góc trái trên và điểm góc phải dưới của bounding box; conf thể hiện xác suất vật thể xuất hiện trong bounding box; cls chỉ số lớp của đối tượng được phát hiện.\
\
**2.2 Bộ dữ liệu**\
Dữ liệu được thu thập thủ công bằng cách chụp hình ảnh rác thải sinh hoạt hằng ngày. \
	Bao gồm 230 ảnh trong đó:
+ 181 vật thể là thủy tinh.
+ 209 vật thể là kim loại.
+ 236 vật thể là giấy
+ 279 vật thể là nhựa. \
\
**2.3 Xử lý dữ liệu** 
+ Đánh nhãn và đóng khung dữ liệu: Roboflow
+ Ảnh sẽ được resize về với kích thước 640 x 640 px.\
**2.4 Phương pháp sử dụng** \
Yolov8



