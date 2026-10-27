## PHẦN 1. PHÂN TÍCH

AutoFilter được xem như công cụ Google Search của bảng tính vì giúp tìm kiếm và lọc dữ liệu theo điều kiện mà không cần xem từng dòng.

Ví dụ em có thể lọc nhật ký hệ thống theo mã độc, mức độ nguy hiểm hoặc thời gian xảy ra sự cố để nhanh chóng tìm ra các cảnh báo cần xử lý.

## PHẦN 2. TRIỂN KHAI

1.  Word – Báo cáo sự cố an ninh mạng
    

Em tạo báo cáo Incident Report cho trung tâm NetGuard, gồm các nội dung:

-   Giới thiệu: Mục đích và phạm vi báo cáo.
    
-   Thông tin sự cố: Thời gian, hệ thống bị ảnh hưởng và mức độ nguy hiểm.
    
-   Phân tích sự cố: Loại mã độc, nguyên nhân và hậu quả.
    
-   Biện pháp xử lý: Cô lập hệ thống, loại bỏ mã độc và khôi phục dữ liệu.
    
-   Phòng ngừa: Đề xuất biện pháp bảo vệ hệ thống.
    

Em sử dụng Heading 1 và Heading 2 để phân cấp tiêu đề, sau đó mở Navigation Pane để quản lý nội dung. Em tạo mục lục tự động (Auto TOC) và cập nhật toàn bộ mục lục trước khi lưu để số trang và liên kết tiêu đề chính xác.

2.  Excel – Tra cứu và đối soát mã độc
    

Em sử dụng hai bảng dữ liệu:

-   Cơ sở dữ liệu virus: Mã độc, tên mã độc, mức độ nguy hiểm và cách xử lý.
    
-   Nhật ký hệ thống: Thời gian, mã cảnh báo, mã độc và trạng thái xử lý.
    

Em dùng hàm VLOOKUP kết hợp TRIM để loại bỏ khoảng trắng thừa và tra cứu chính xác tên mã độc.

Ví dụ công thức:

=VLOOKUP(TRIM(C2),$F$2:$H$100,2,FALSE)

Trong đó, C2 là mã độc cần tra cứu; cột F chứa mã độc trong cơ sở dữ liệu, cột G chứa tên mã độc. Tham số FALSE giúp tìm kiếm chính xác.

Em bật AutoFilter để lọc các cảnh báo theo tên mã độc, mức độ nguy hiểm hoặc trạng thái xử lý. Dữ liệu cần có hàng tiêu đề rõ ràng, không gộp ô và không để hàng trống giữa các bản ghi.

3.  PowerPoint – Chiến lược phòng thủ 3 tầng
    

Em thiết kế slide trình bày chiến lược phòng thủ an ninh mạng theo sơ đồ phân cấp gồm:

-   Tầng 1 – Phòng ngừa: Sử dụng tường lửa, phần mềm diệt virus và cập nhật hệ thống.
    
-   Tầng 2 – Phát hiện: Giám sát nhật ký hệ thống, phát hiện hành vi bất thường và cảnh báo mã độc.
    
-   Tầng 3 – Ứng phó: Cô lập thiết bị bị nhiễm, loại bỏ mã độc và khôi phục dữ liệu.
    

Em sử dụng sơ đồ phân cấp để thể hiện mối liên hệ giữa ba tầng. Font chữ Montserrat hoặc Inter giúp nội dung rõ ràng khi trình chiếu.
## Em kết luận như sau :

Qua bài tập, em biết cách xây dựng báo cáo sự cố bằng Word, tra cứu mã độc bằng VLOOKUP kết hợp TRIM và lọc nhật ký bằng AutoFilter. Đồng thời, em hiểu cách trình bày chiến lược phòng thủ 3 tầng bằng PowerPoint để giúp khách hàng dễ hiểu và lựa chọn biện pháp bảo vệ phù hợp.
