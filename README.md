BÀI TẬP VỀ NHÀ 05, Môn Hệ quản trị csdl.

SUBJECT: Trigger on mssql

A. Trình bày lại đầu bài của đồ án PT&TKHT:
1. Mô tả bài toán của đồ án PT&TKHT, 
   đưa ra yêu cầu của bài toán đó
2. Cơ sở dữ liệu của Đồ án PT&TKHT :
   Có database với các bảng dữ liệu cần thiết (3nf),
   Các bảng này đã có PK, FK, CK cần thiết
 
B. Nội dung Bài tập 05:
1. Dựa trên cơ sở là csdl của Đồ án
2. Tìm cách bổ xung thêm 1 (hoặc vài) trường phi chuẩn
   (là trường tính toán đc, nhưng thêm vào thì ok hơn,
    ok hơn theo 1 logic nào đó, vd ok hơn về speed)
   => Nêu rõ logic này!
3. Viết trigger cho 1 bảng nào đó, 
   mà có sử dụng trường phi chuẩn này,
   nhằm đạt được 1 vài mục tiêu nào đó.
   => Nêu rõ các mục tiêu 
4. Nhập dữ liệu có kiểm soát, 
   nhằm để test sự hiệu quả của việc trigger auto run.
5. Kết luận về Trigger đã giúp gì cho đồ án của em.

HƯỚNG DẪN CÁCH LÀM:

Hướng dẫn làm phần A: 
 - Chỉ cần nêu ra y/c của đồ án.
 - Không cần chụp quá trình làm ra db, tables.
 - Chỉ cần đưa ra db gồm các bảng nào,
   mỗi bảng có các trường nào, kiểu dữ liệu nào,
   và pk, fk, ck của các bảng.

Hướng dẫn làm phần B:
1. Sv tạo repo mới trên github, cho phép truy cập public.
2. Tạo file Readme.md, đầu file để thông tin cá nhân sv.
3. Tiếp theo đưa phần A vào file Reame.md .
3. Các thao tác làm trên csdl bằng phần mềm ssms.
4. Chụp ảnh màn hình quá trình làm.
5. Paste ngay vào Readme.md, 
   rồi gõ mô tả ảnh này làm gì, nhập gì, hay đạt được điều gì...
6. Có thể thêm những nhận xét hoặc kết luận
   cho việc bản thân đã hiểu rõ thêm về 1 vấn đề gì đó.
7. Lặp lại các step 4 5 6 cho đến khi hoàn thành yêu cầu của phần B.
8. Xuất các file sql chứa cấu trúc và data, up lên cùng repo.
9. Link đến repo cần mở được trực tiếp nội dung, 
   Paste link này vào file excel online ghim trên nhóm.
   Thầy sẽ dùng tool để check các link này.

DEADLINE: 23H59:59 NGÀY 23/04/2025 
Trình bày lại đầu bài đồ án PT&TKHT
1.Yêu cầu của đồ án: Phân tích thiết kế hệ thống quản lý hiệu sách
2.Cơ sở dữ liệu của hệ thống quản lý hiệu sách
Tạo database mang tên Ql_Sach
![Image](https://github.com/user-attachments/assets/58916859-1781-4552-b3c5-16785ae98f3d)
Tạo bảng Theloai
![Image](https://github.com/user-attachments/assets/6af6c5fc-e031-4d28-a8ee-99dca6529959)
Tạo bảng Sach
![Image](https://github.com/user-attachments/assets/5aa18373-0c24-4b5d-8a05-841211934edf)
Tạo bảng Tacgia
![Image](https://github.com/user-attachments/assets/1015bfc4-8bae-4f8c-a3e3-70785d8fda7a)
Tạo bảng Sachtacgia
![Image](https://github.com/user-attachments/assets/ac566ab5-3813-44ac-99c9-cb3699795045)
Tạo bảng Docgia
![Image](https://github.com/user-attachments/assets/c611d03c-47ab-40e8-b04d-789eefb96aee)
Tạo bảng Nhanvien
![Image](https://github.com/user-attachments/assets/d54fb74f-df3d-4c00-9407-e13cbad73d60)
Tạo bảng Phieumuon
![Image](https://github.com/user-attachments/assets/0cbcd755-941e-45c5-a193-c93fb8aa1087)
Tạo bảng Chitietmuon
![Image](https://github.com/user-attachments/assets/e890e127-0f3a-4853-92ae-9dd822fc9df1)
Tạo bảng Taikhoan
![Image](https://github.com/user-attachments/assets/f69bda81-6930-4224-bbb4-9cc2afe10876)
Sau đó thêm các khóa ngoại và tạo bảng liên kết quản lý hiệu sách 

B. Nội dung Bài tập 05:
Tạo csdl cho hệ thống quản lý hiệu thuốc
Bổ sung thêm trường phi chuẩn: bổ sung Trường TongSoSach giúp:
  Truy vấn nhanh số lượng sách từng thể loại
 Tăng hiệu năng khi hiển thị danh sách
Viết trigger cho bảng Sach để đạt được mục tiêu

Ấn vào dấu + của bảng Sach rồi ấn new trigger

Viết trigger để đạt được mục tiêu
![Image](https://github.com/user-attachments/assets/6e5c8e51-2025-4448-9fa5-1d7d476f0283)
Nhập dữ liệu kiểm thử
![Image](https://github.com/user-attachments/assets/36f69426-dc4f-4a8c-b44e-993b5873e0e9)
Kết luận trigger này đã làm gì cho đồ án
Trigger này giúp tự động cập nhật số lượng sách theo thể loại, tối ưu hiệu suất truy vấn và đảm bảo dữ liệu luôn chính xác.




