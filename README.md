# BaiTap6

Bài tập 6: Hệ quản trị CSDL
Chủ đề: Câu lệnh Select
Yêu cầu bài tập: 
1. Hãy nêu các bước để import được dữ liệu trong sv_tnut.sql vào sql server của em
2. dữ liệu đầu vào là tên của sv; sđt; ngày, tháng, năm sinh của sinh viên (của sv đang làm bài tập này)
3. nhập sql để tìm xem có những sv nào trùng hoàn toàn ngày/tháng/năm với em?
4. nhập sql để tìm xem có những sv nào trùng ngày và tháng sinh với em?
5. nhập sql để tìm xem có những sv nào trùng tháng và năm sinh với em?
6. nhập sql để tìm xem có những sv nào trùng tên với em?
7. nhập sql để tìm xem có những sv nào trùng họ và tên đệm với em.
8. nhập sql để tìm xem có những sv nào có sđt sai khác chỉ 1 số so với sđt của em.
9. BẢNG SV CÓ HƠN 9000 ROWS, HÃY LIỆT KÊ TẤT CẢ CÁC SV NGÀNH KMT, SẮP XẾP THEO TÊN VÀ HỌ ĐỆM, KIỂU TIẾNG  VIỆT, GIẢI THÍCH.
10. HÃY NHẬP SQL ĐỂ LIỆT KÊ CÁC SV NỮ NGÀNH KMT CÓ TRONG BẢNG SV (TRÌNH BÀY QUÁ TRÌNH SUY NGHĨ VÀ GIẢI NHỮNG VỨNG MẮC)

# Bài Làm
# Hãy nêu các bước để import được dữ liệu trong sv_tnut.sql vào sql server của em
Sử dụng SQL Server Management Studio (SSMS)
Mở SSMS và kết nối đến server của bạn.
![image](https://github.com/user-attachments/assets/39995204-2976-40e3-a980-2bd44d59ec70)

Tạo một database mới tên btap6
![image](https://github.com/user-attachments/assets/927620b0-0bb3-4d13-b17e-793edbaeeec8)

Chọn menu File > Open > File, chọn file sv_tnut.sql.
![image](https://github.com/user-attachments/assets/f515d385-c03e-44ba-b195-a876138c1577)

Đổi tên file thành btap6 rồi chạy
![image](https://github.com/user-attachments/assets/8d1b23a1-4a54-4661-85a7-081d714a1929)

# 2 dữ liệu đầu vào 
Tên của sv          : Nguyễn Tiến Thắng 
Ngày-Thắng_năm sinh : 09-02-2003
SỐ điện thoại       :  0388834522.

# 3 Nhập sql để tìm xem có những sv nào trùng hoàn toàn ngày/tháng/năm .
 SELECT * FROM SV
WHERE ns = '2003-02-09';

![image](https://github.com/user-attachments/assets/8b936918-283c-4cd7-b5e2-e9e8bf4d2d12)

# 4. nhập sql để tìm xem có những sv nào trùng ngày và tháng sinh
SELECT * FROM SV
WHERE DAY(ns) = 9 AND MONTH(ns) = 2;

![image](https://github.com/user-attachments/assets/ae38babe-be80-4d1d-9df9-2140ca4031fa)

# 5. nhập sql để tìm xem có những sv nào trùng tháng và năm sinh
SELECT * FROM SV
WHERE MONTH(ns) = 2 AND YEAR(ns) = 2003;

![image](https://github.com/user-attachments/assets/73a0bf51-6ec9-4ae4-97cd-68c5fed2978f)

# 6. nhập sql để tìm xem có những sv nào trùng tên với em

SELECT * FROM SV
WHERE ten = N'Thắng';

![image](https://github.com/user-attachments/assets/3b10fb05-a95f-4b64-9972-778761456493)

# 7. nhập sql để tìm xem có những sv nào trùng họ và tên đệm với em.
SELECT * FROM SV
WHERE hodem = N'Nguyễn Tiến';

8. nhập sql để tìm xem có những sv nào có sđt sai khác chỉ 1 số so với sđt của em.
   
10. BẢNG SV CÓ HƠN 9000 ROWS, HÃY LIỆT KÊ TẤT CẢ CÁC SV NGÀNH KMT, SẮP XẾP THEO TÊN VÀ HỌ ĐỆM, KIỂU TIẾNG  VIỆT, GIẢI THÍCH.
11. HÃY NHẬP SQL ĐỂ LIỆT KÊ CÁC SV NỮ NGÀNH KMT CÓ TRONG BẢNG SV (TRÌNH BÀY QUÁ TRÌNH SUY NGHĨ VÀ GIẢI NHỮNG VỨNG MẮC)


