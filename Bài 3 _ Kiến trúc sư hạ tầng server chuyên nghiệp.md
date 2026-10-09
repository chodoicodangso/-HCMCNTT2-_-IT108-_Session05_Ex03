Sơ đồ IPO  
Input: Thông tin đường dẫn thư mục, tên 3 file cấu hình và vị trí thư mục backup.  
Process: Khởi tạo cấu trúc thư mục → Tạo các file cấu hình → Sao chép đệ quy sang thư mục backup.  
Output: Cây thư mục smart-farm hoàn chỉnh và thư mục sao lưu code\_v1 chứa đầy đủ dữ liệu

Danh sách các câu lệnh **PowerShell** đã sử dụng.

New-Item \-ItemType Directory \-Force \-Path "smart-farm\\data\\logs" , "smart-farm\\code"  
ni \-Type File \-f "smart-farm\\code\\{config.json\\[sensors.py](http://sensors.py)\\.env}"  
cp smart-farm\\code smart-farm\\backup\\code\_v1 \-r \-Force