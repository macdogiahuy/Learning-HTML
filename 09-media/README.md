# Media trong HTML

## Giới thiệu
HTML5 cung cấp các thẻ `<audio>` và `<video>` để nhúng nội dung đa phương tiện vào trang web mà không cần plugin bổ sung.

## Thẻ Video

### Cú pháp cơ bản
```html
<video src="video.mp4" controls>
    Trình duyệt của bạn không hỗ trợ video HTML5.
</video>
```

### Với nhiều nguồn video
```html
<video controls>
    <source src="video.mp4" type="video/mp4">
    <source src="video.webm" type="video/webm">
    <source src="video.ogg" type="video/ogg">
    Trình duyệt của bạn không hỗ trợ video HTML5.
</video>
```

### Thuộc tính quan trọng
1. **controls**: Hiển thị điều khiển video
2. **autoplay**: Tự động phát
3. **loop**: Phát lặp lại
4. **muted**: Tắt tiếng
5. **poster**: Ảnh hiển thị trước khi phát
6. **width** và **height**: Kích thước video
7. **preload**: Tùy chọn tải trước

```html
<video controls autoplay muted
       width="640" height="360"
       poster="thumbnail.jpg"
       preload="auto">
    <source src="video.mp4" type="video/mp4">
</video>
```

## Thẻ Audio

### Cú pháp cơ bản
```html
<audio src="audio.mp3" controls>
    Trình duyệt của bạn không hỗ trợ audio HTML5.
</audio>
```

### Với nhiều nguồn audio
```html
<audio controls>
    <source src="audio.mp3" type="audio/mpeg">
    <source src="audio.ogg" type="audio/ogg">
    Trình duyệt của bạn không hỗ trợ audio HTML5.
</audio>
```

### Thuộc tính quan trọng
1. **controls**: Hiển thị điều khiển audio
2. **autoplay**: Tự động phát
3. **loop**: Phát lặp lại
4. **muted**: Tắt tiếng
5. **preload**: Tùy chọn tải trước

## Định dạng hỗ trợ

### Video
- **MP4** (.mp4)
- **WebM** (.webm)
- **Ogg** (.ogv)

### Audio
- **MP3** (.mp3)
- **WAV** (.wav)
- **Ogg** (.ogg)
- **AAC** (.aac)

## Nhúng video từ dịch vụ bên ngoài

### YouTube
```html
<iframe width="560" height="315"
        src="https://www.youtube.com/embed/VIDEO_ID"
        frameborder="0"
        allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture"
        allowfullscreen>
</iframe>
```

### Vimeo
```html
<iframe width="560" height="315"
        src="https://player.vimeo.com/video/VIDEO_ID"
        frameborder="0"
        allow="autoplay; fullscreen; picture-in-picture"
        allowfullscreen>
</iframe>
```

## Lưu ý quan trọng

1. **Tối ưu hóa**
   - Nén file media trước khi sử dụng
   - Cung cấp nhiều định dạng khác nhau
   - Sử dụng thuộc tính preload phù hợp

2. **Khả năng tiếp cận**
   - Thêm phụ đề cho video
   - Cung cấp bản ghi cho audio
   - Thêm văn bản thay thế

3. **Hiệu suất**
   - Không tự động phát media khi không cần thiết
   - Cân nhắc kích thước file
   - Sử dụng CDN cho file lớn

4. **Tương thích**
   - Luôn cung cấp nội dung thay thế
   - Kiểm tra hỗ trợ trên các trình duyệt
   - Sử dụng các định dạng phổ biến

5. **Bảo mật**
   - Cẩn thận với autoplay
   - Kiểm soát nguồn media
   - Xem xét vấn đề bản quyền