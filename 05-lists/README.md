# Danh sách trong HTML

## Giới thiệu
HTML cung cấp ba loại danh sách khác nhau để tổ chức thông tin: danh sách không có thứ tự (unordered list), danh sách có thứ tự (ordered list), và danh sách mô tả (description list).

## Các loại danh sách

### 1. Danh sách không có thứ tự (Unordered List)
```html
<ul>
    <li>Mục thứ nhất</li>
    <li>Mục thứ hai</li>
    <li>Mục thứ ba</li>
</ul>
```

### 2. Danh sách có thứ tự (Ordered List)
```html
<ol>
    <li>Bước 1</li>
    <li>Bước 2</li>
    <li>Bước 3</li>
</ol>
```

### 3. Danh sách mô tả (Description List)
```html
<dl>
    <dt>HTML</dt>
    <dd>Ngôn ngữ đánh dấu siêu văn bản</dd>
    <dt>CSS</dt>
    <dd>Ngôn ngữ tạo kiểu cho trang web</dd>
</dl>
```

## Thuộc tính đặc biệt

### Cho danh sách có thứ tự (ol)
- `type`: Kiểu đánh số (1, A, a, I, i)
- `start`: Số bắt đầu
- `reversed`: Đảo ngược thứ tự

```html
<ol type="A" start="3">
    <li>Mục C</li>
    <li>Mục D</li>
</ol>
```

## Danh sách lồng nhau
```html
<ul>
    <li>Mục 1
        <ul>
            <li>Mục 1.1</li>
            <li>Mục 1.2</li>
        </ul>
    </li>
    <li>Mục 2</li>
</ul>
```

## Ứng dụng phổ biến
1. Menu điều hướng
2. Danh sách các bước hướng dẫn
3. Cấu trúc sitemap
4. Danh sách sản phẩm
5. FAQ (Câu hỏi thường gặp)

## Lưu ý quan trọng
- Chỉ sử dụng `<li>` trong `<ul>`, `<ol>`, hoặc các thẻ list khác
- Sử dụng danh sách phù hợp với nội dung (có thứ tự/không có thứ tự)
- Có thể tùy chỉnh dấu đầu dòng bằng CSS (list-style-type)
- Danh sách có thể lồng nhau nhiều cấp
- Danh sách mô tả thích hợp cho các cặp thuật ngữ và định nghĩa