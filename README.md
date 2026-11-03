### Phần 1. Phân tích
Sử dụng tab Network và bật Disable Cache để kiểm tra thời gian tải. Quan sát Waterfall để tìm tài nguyên tải chậm, Request lỗi 404 và hình ảnh có dung lượng lớn.

### Phần 2. Triển khai
Thực hiện 3 bước tối ưu:
1. **Sửa lỗi 404:** Kiểm tra và sửa đường dẫn tài nguyên bị lỗi.
2. **Nén hình ảnh:** Giảm dung lượng ảnh, ưu tiên định dạng WebP.
3. **Bật Browser Cache:** Lưu tài nguyên tĩnh để tăng tốc độ tải trang.

Đảm bảo CSS và JavaScript quan trọng được tải thành công với mã 200 OK.

### Phần 3. Kiểm thử
Mã 304 Not Modified cho biết tài nguyên không thay đổi nên trình duyệt sử dụng bản lưu trong Cache, giúp tiết kiệm băng thông và tăng tốc độ tải trang.
