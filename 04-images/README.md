# Hình ảnh trong HTML

## Giới thiệu
Thẻ `<img>` được sử dụng để hiển thị hình ảnh trong trang web. Đây là thẻ tự đóng (không cần thẻ đóng).

## Cú pháp cơ bản
```html
<img src="đường-dẫn-ảnh" alt="mô tả ảnh">
```

## Thuộc tính quan trọng

1. **src (bắt buộc)**
   - Đường dẫn đến file hình ảnh
   - Có thể là đường dẫn tương đối hoặc tuyệt đối
   ```html
   <img src="images/photo.jpg">
   <img src="https://example.com/photo.jpg">
   ```

2. **alt (bắt buộc)**
   - Văn bản thay thế khi ảnh không tải được
   - Hỗ trợ người dùng khiếm thị
   - Hỗ trợ SEO
   ```html
   <img src="cat.jpg" alt="Một chú mèo đang nằm ngủ">
   ```

3. **width và height (tùy chọn)**
   - Kích thước của ảnh (đơn vị pixel)
   - Nên chỉ định để tránh layout shift
   ```html
   <img src="logo.png" width="200" height="100">
   ```

## Định dạng ảnh phổ biến
- **JPG/JPEG**: Ảnh chụp, hình ảnh có nhiều màu sắc
- **PNG**: Ảnh có nền trong suốt, logo
- **GIF**: Ảnh động đơn giản
- **SVG**: Logo, icon, hình vector
- **WebP**: Định dạng hiện đại, kích thước nhỏ

## Lưu ý quan trọng
- Luôn sử dụng thuộc tính alt
- Tối ưu kích thước ảnh trước khi sử dụng
- Đặt tên file ảnh có ý nghĩa
- Sử dụng đúng định dạng ảnh cho từng mục đích
- Cân nhắc sử dụng thẻ `<figure>` và `<figcaption>` để thêm chú thích cho ảnh
```html
<figure>
    <img src="mountain.jpg" alt="Núi Phú Sĩ trong hoàng hôn">
    <figcaption>Hoàng hôn trên đỉnh Phú Sĩ</figcaption>
</figure>