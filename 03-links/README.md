# Liên kết trong HTML

## Giới thiệu
Thẻ `<a>` (anchor) được sử dụng để tạo liên kết trong HTML, cho phép người dùng di chuyển giữa các trang web hoặc đến các phần khác nhau trong cùng một trang.

## Cú pháp cơ bản
```html
<a href="url">Nội dung liên kết</a>
```

## Các loại liên kết

1. **Liên kết ngoài (External Links)**
```html
<a href="https://www.example.com">Truy cập website</a>
```

2. **Liên kết nội bộ (Internal Links)**
```html
<a href="/trang-chu.html">Trang chủ</a>
```

3. **Liên kết trong trang (Anchor Links)**
```html
<a href="#section1">Đến phần 1</a>
```

4. **Liên kết Email**
```html
<a href="mailto:email@example.com">Gửi email</a>
```

5. **Liên kết điện thoại**
```html
<a href="tel:+84123456789">Gọi điện</a>
```

## Thuộc tính quan trọng

- `href`: Địa chỉ liên kết
- `target`: Cách mở liên kết (`_blank`, `_self`, `_parent`, `_top`)
- `title`: Mô tả khi di chuột qua
- `rel`: Mối quan hệ với trang đích

## Ví dụ
```html
<a href="https://google.com" target="_blank" title="Mở Google">
    Truy cập Google trong tab mới
</a>
```

## Lưu ý quan trọng
- Luôn sử dụng `target="_blank"` và `rel="noopener noreferrer"` khi mở liên kết trong tab mới
- Đảm bảo văn bản liên kết có ý nghĩa (tránh dùng "Click here")
- Sử dụng đường dẫn tương đối cho liên kết nội bộ
- Tạo sự khác biệt trực quan cho liên kết (màu sắc, gạch chân)