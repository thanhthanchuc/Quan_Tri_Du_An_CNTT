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
3.  #### Stability Testing

    - Khái niệm: Stability Testing Là kỹ thuật test nhằm xác minh sự ổn định của phần mềm qua việc kiểm tra khả năng chạy liên tục của ứng dụng trong hoặc hơn khoảng thời gian có thể chấp nhận được. Đây là 1 kỹ thuật non-functional, với mục đích đòi hỏi khả năng chịu tải của phần mềm tới mức tối đa. Trong quá trình xác định nó hoạt động tốt thế nào dưới tải ở mức chấp nhận được, mức đỉnh, các tải được tạo ra đột ngột, với số lượng dữ liệu lớn được xử lý… Stability testing được thực hiện để kiểm tra hiệu quả của 1 sản phẩm được phát triển vượt qua mức hoạt động bình thường, hay tới 1 điểm dừng. Có ý nghĩa quan trọng hơn là trong việc xử lý lỗi, độ tin cậy của phần mềm, khả năng chịu tải và khả năng mở rộng của 1 sản phẩm dưới tải lớn chứ không phải là kiểm tra cách hoạt động của hệ thống trong các hoàn cảnh bình thường.

    Stability testing còn được gọi là Load hoặc endurance testing.

    Stability testing cho phép bạn kiểm tra:

    *   Ước lượng độ tin cậy trong sự ổn định của hệ thống của bạn đang thử nghiệm
    *   Đảm bảo rằng hệ thống của bạn có thể xử lý các chương trình lớn
    *   Theo dõi hiệu quả của hệ thống của bạn
    *   Kiểm tra hệ thống ổn định theo yêu cầu