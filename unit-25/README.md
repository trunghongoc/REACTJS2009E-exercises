# Bài tập buổi 25, thứ 7 (26-12-2020)

## Bài 1
- Hãy tạo mock json server (dùng package https://www.npmjs.com/package/json-server) để tạo các bảng sau
  - Bảng `provinces` (tỉnh thành)
  - Bảng `districts` (quận, huyện)
  - Bảng `wards` (xã, phường)
  - Xem mock data ở file: https://github.com/trunghongoc/REACTJS2009E-exercises/blob/main/unit-25/resources/address.js

- Yêu cầu về `routes`
- Khi request với method GET đến url `/provinces`, thì sẽ lấy hết tất cả `provinces` và trả về cho client
- Khi request với method GET đến url `/province/:id` thì sẽ tìm `province` có `id` là id trên url và trả về cho client, nếu không tìm thấy thì trả về `null`

- Khi request với method GET đến url `/districts`, thì sẽ lấy hết tất cả `districts` và trả về cho client
- Khi request với method GET đến url `/districts/:id` thì sẽ tìm `district` có `id` là id trên url và trả về cho client, nếu không tìm thấy thì trả về `null`
- Khi request với method GET đến url `/provinces/:id/districts`, thì sẽ tìm tất cả `districts` có `provinceId` bằng `id` trên url và trả về cho client

- Khi request với method GET đến url `/wards`, thì sẽ lấy hết tất cả `wards` và trả về cho client
- Khi request với method GET đến url `/wards/:id` thì sẽ tìm `wards` có `id` là id trên url và trả về cho client, nếu không tìm thấy thì trả về `null`
- Khi request với method GET đến url `/districts/:id/wards`, thì sẽ tìm tất cả `wards` có `districtId` bằng `id` trên url và trả về cho client

- Đối với api lấy về 1 danh sách, thì trả về 1 array, nếu không tìm thấy bản ghi nào thì là array rỗng


## Bài 2
- Sử dụng ant design để tạo form `register` với yêu cầu sau đây

  - name: bắt buộc nhập, tối đa 32 ký tự, phải chuẩn hóa chuỗi (xóa hết dấu cách thừa)
  - userName: chỉ được phép chứa các ký tự a-z (thường), 0-9 và dấu gạch dưới. Bắt buộc nhập.
  - address: bắt buộc chọn, khi chọn tỉnh mới có thể chọn huyện, khi chọn huyện mới có thể chọn xã. Với api đã xây dựng ở bài 1
    - Vd:
      - ![](https://github.com/trunghongoc/REACTJS2009E-exercises/blob/main/unit-25/imgs/select-address.png "")
  - avatar: phải preview được, phải là hình ảnh. Sử dụng component sau
    - Vd:
      - ![](https://github.com/trunghongoc/REACTJS2009E-exercises/blob/main/unit-25/imgs/upload-avatar.png "")
  - email: phải có định dạng email, bắt buộc nhập
  - password: bắt buộc nhập, tối thiểu 6 ký tự

- Đồng thời hãy viết validate cho form vừa tạo
- Khi nhấn submit, nếu data hợp lệ, hãy gửi toàn bộ data đến url sau với method POST `/register` với cấu trúc data
```js
{
  name: String,
  userName: String,
  provinceId: Number,
  districtId: Number,
  wardId: Number,
  avatar: File | undefined,
  email: String,
  password: String
}
```

