# Quản trị dự án CNTT

###### Nhóm 21

Danh sách thành viên nhóm:

*   Nguyễn Ngọc Thành
*   Nguyễn Văn Thành
*   Nguyễn Đình Tuyên

1.  #### Unit Test

    - Khái niệm: <u>Unit Test</u> là code dùng để test code

    Một số đặc điểm cảu unit test:

    *   Code unit test phải ngắn gọn, dễ hiểu, dễ đọc.
    *   Mỗi unit test là 1 đơn vi riêng biệt, độc lập, không phụ thuộc vào unit khác.
    *   Mỗi unit test là 1 method trong test class, tên method cũng là tên UnitTest. Do đó ta nên đặt tên hàm rõ ràng, nói rõ unit test này test cái gì (Test_A_Do_B), tên method có thể rất dàiii cũng không sao.
    *   Unit Test phải nhanh, vì nó sẽ được chạy để kiểm định lỗi mỗi lần build. Do đó trong unit test nên hạn chế các task tốn thời gian như gọi I/O, database, network,…
    *   Unit Test nên test từng đối tượng riêng biệt. Vd: Unit Test cho Business Class thì chỉnh test chính BusinessClass đó, không nên dụng tới các class móc nối với nó (DataAccess Class chẳng hạn).

    Một số lợi ích của Unit Test:

    *   Nếu viết Unit Test một cách cẩn thận, **code của bạn sẽ ít lỗi hơi**, vì Unit Test sẽ phát hiện lỗi cho bạn.
    *   Phát hiện những hàm chạy chậm và không hiệu quả thông qua thời gian chạy của Unit Test.
    *   Tăng sự tự tin khi code, vì đã có Unit Test phát hiện lỗi.
    *   Khi refactor code, sửa code hay thêm chức năng mới, **Unit Test đảm bảo chương trình chạy đúng**, phát hiện những lỗi tiềm tàng mà ta bỏ lỡ.
2.  #### Acceptance Test

    - Khái niệm: <u>Acceptance Testing</u> - Kiểm thử chấp nhận, là một kỹ thuật kiểm thử được thực hiện để xác định hệ thống phần mềm có đạt được những yêu cầu kỹ thuật hay không.

    - Mục đích: Để đánh giá hệ thống với những yêu cầu của doanh nghiệp và xác nhận nếu hệ thống đáp ứng được những tiêu chí yêu cầu để chuyển đến người dùng cuối.

    Kiểm thử chấp nhận có nhiều dạng như sau:

    *   Kiểm thử chấp nhận người dùng
    *   Kiểm thử chấp nhận doanh nghiệp
    *   Kiểm thử Alpha
    *   Kiểm thử Beta