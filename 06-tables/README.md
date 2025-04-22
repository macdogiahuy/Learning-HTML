# Bảng trong HTML

## Giới thiệu
Bảng trong HTML được sử dụng để hiển thị dữ liệu dưới dạng các hàng và cột. Bảng thích hợp cho việc trình bày dữ liệu có tính tổ chức như thông tin sản phẩm, bảng giá, lịch trình, v.v.

## Cấu trúc cơ bản
```html
<table>
    <thead>
        <tr>
            <th>Tiêu đề cột 1</th>
            <th>Tiêu đề cột 2</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Dữ liệu 1</td>
            <td>Dữ liệu 2</td>
        </tr>
    </tbody>
</table>
```

## Các thẻ chính

1. **Thẻ cấu trúc bảng**
   - `<table>`: Định nghĩa một bảng
   - `<thead>`: Nhóm các hàng tiêu đề
   - `<tbody>`: Nhóm nội dung chính của bảng
   - `<tfoot>`: Nhóm các hàng chân bảng

2. **Thẻ hàng và ô**
   - `<tr>`: Định nghĩa một hàng
   - `<th>`: Ô tiêu đề
   - `<td>`: Ô dữ liệu

## Thuộc tính quan trọng

### Gộp ô
1. **colspan**: Gộp các cột
```html
<td colspan="2">Ô này chiếm 2 cột</td>
```

2. **rowspan**: Gộp các hàng
```html
<td rowspan="3">Ô này chiếm 3 hàng</td>
```

### Thuộc tính bảng
- `border`: Đường viền bảng
- `cellpadding`: Khoảng cách giữa nội dung và viền ô
- `cellspacing`: Khoảng cách giữa các ô

## Ví dụ mở rộng
```html
<table border="1">
    <thead>
        <tr>
            <th>Sản phẩm</th>
            <th>Giá</th>
            <th>Số lượng</th>
        </tr>
    </thead>
    <tbody>
        <tr>
            <td>Sản phẩm A</td>
            <td>100.000đ</td>
            <td>5</td>
        </tr>
        <tr>
            <td>Sản phẩm B</td>
            <td>200.000đ</td>
            <td>3</td>
        </tr>
    </tbody>
    <tfoot>
        <tr>
            <td colspan="2">Tổng cộng:</td>
            <td>8</td>
        </tr>
    </tfoot>
</table>
```

## Lưu ý quan trọng
1. Sử dụng bảng CHỈ để hiển thị dữ liệu dạng bảng, không dùng để tạo layout
2. Luôn sử dụng `<thead>`, `<tbody>`, và `<tfoot>` để cấu trúc bảng rõ ràng
3. Sử dụng `<th>` cho các ô tiêu đề để tăng tính ngữ nghĩa
4. Cân nhắc sử dụng CSS để tạo kiểu cho bảng thay vì thuộc tính HTML
5. Thêm thuộc tính `scope` cho `<th>` để cải thiện khả năng truy cập
6. Sử dụng `<caption>` để thêm tiêu đề cho bảng