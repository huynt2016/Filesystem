#Hệ thống thư mục trong Linux
##I.Các loại định dạng thư mục hệ thống Linux
###1.Journaling
####a.Khái niệm

- Journaling là một hệ thống nhật kí cung cấp khả năng kiểm soát và phục hồi lỗi cho hệ thống lưu trữ dữ liệu.
- Tuy nhiên, nhược điểm của việc sử dụng journaling là phải “đánh đổi” hiệu suất trong việc ghi dữ liệu với tính ổn định của hệ thống.

####b.Cơ chế

<img src="http://i.imgur.com/q9JS7sl.png">

###2.Bảng so sánh các loại định dạng

| File system | Kích thước file tối đa  | Kích thước ổ đĩa tối đa| Journaling | Ghi chú |
|-------------|-------------------------|------------------------|------------|---------|
| EXT2 | 2TB | 32TB | Không | Đã lạc hậu |
| EXT3 | 2TB | 32TB | Có | Hệ thống cài đặt chuẩn cho Linux trong nhiều năm |
| EXT4 | 16TB | 1EB | Có | Hệ thống cài đặt mới cho Linux |
| ReiserFS | 8TB | 16TB | Có | Có tốc độ xử lý nhanh với những file có kích thước dưới 4KB |
| XFS | 8EB | 8EB | Có | Sử dụng cho hệ thống lớn, lên đến hàng trăm TB |
| JFS | 4PB | 32PB | Có | Không còn được hỗ trợ và duy trì |

- Đơn vị: GiB = Gibibyte (1024 MiB) :: TiB = tebibyte (1024 GiB) :: PIB = Pebibyte (1024 Tib) :: EIB = Exbibyte (1024 PIB)

##II.Cấu trúc thư mục hệ thống
##III.Các câu lệnh thực thi với thư mục, tập tin trong Linux
