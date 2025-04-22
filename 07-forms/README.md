# Form trong HTML

## Giới thiệu
Form là phương tiện để thu thập thông tin từ người dùng trong HTML. Form có thể chứa nhiều loại trường nhập liệu khác nhau như text, password, checkbox, radio button, v.v.

## Cú pháp cơ bản
```html
<form action="/submit" method="post">
    <input type="text" name="username">
    <input type="submit" value="Gửi">
</form>
```

## Các thẻ chính trong Form

### 1. Thẻ form
```html
<form action="url-xử-lý" method="get|post">
    <!-- Các trường nhập liệu -->
</form>
```
- `action`: URL xử lý dữ liệu form
- `method`: Phương thức gửi dữ liệu (GET hoặc POST)

### 2. Các loại input phổ biến
```html
<!-- Text -->
<input type="text" name="username" placeholder="Nhập tên">

<!-- Password -->
<input type="password" name="password">

<!-- Radio buttons -->
<input type="radio" name="gender" value="male"> Nam
<input type="radio" name="gender" value="female"> Nữ

<!-- Checkboxes -->
<input type="checkbox" name="hobbies" value="reading"> Đọc sách
<input type="checkbox" name="hobbies" value="sports"> Thể thao

<!-- Number -->
<input type="number" name="age" min="0" max="100">

<!-- Email -->
<input type="email" name="email">

<!-- Date -->
<input type="date" name="birthday">

<!-- File -->
<input type="file" name="photo">

<!-- Submit button -->
<input type="submit" value="Gửi">

<!-- Reset button -->
<input type="reset" value="Xóa form">
```

### 3. Textarea
```html
<textarea name="message" rows="4" cols="50">
    Nội dung mặc định
</textarea>
```

### 4. Select và Option
```html
<select name="city">
    <option value="hn">Hà Nội</option>
    <option value="hcm">TP.HCM</option>
    <option value="dn">Đà Nẵng</option>
</select>
```

### 5. Label
```html
<label for="username">Tên đăng nhập:</label>
<input type="text" id="username" name="username">
```

## Thuộc tính quan trọng

1. **Thuộc tính chung**
   - `name`: Tên trường (bắt buộc để gửi dữ liệu)
   - `id`: Định danh duy nhất
   - `value`: Giá trị mặc định
   - `disabled`: Vô hiệu hóa trường
   - `required`: Bắt buộc nhập
   - `placeholder`: Gợi ý nhập liệu

2. **Thuộc tính đặc biệt**
   - `min`, `max`: Giới hạn giá trị số
   - `pattern`: Mẫu regex kiểm tra
   - `maxlength`: Độ dài tối đa
   - `accept`: Loại file được chấp nhận (cho input type="file")

## Nhóm trường với Fieldset
```html
<fieldset>
    <legend>Thông tin cá nhân</legend>
    <label for="name">Họ tên:</label>
    <input type="text" id="name" name="name">
    <!-- Các trường khác -->
</fieldset>
```

## Lưu ý quan trọng
1. Luôn sử dụng thẻ `<label>` cho các trường nhập liệu
2. Đặt thuộc tính `name` cho các trường cần gửi dữ liệu
3. Sử dụng `required` cho các trường bắt buộc
4. Dùng `placeholder` để hướng dẫn người dùng
5. Kiểm tra dữ liệu ở cả client và server
6. Nhóm các trường liên quan bằng `fieldset`
7. Đặt `type` phù hợp để tận dụng validation của trình duyệt
8. Sử dụng `autocomplete` khi cần thiết