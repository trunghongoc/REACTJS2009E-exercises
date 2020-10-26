# Bài tập buổi 11, thứ 2 26-10-2020

## Bài 1
Viết 1 hàm trả về 1 array, nhận vào 2 tham số, tham số thứ 1 là ký tự cần lặp, tham số thứ 2 là số lần lặp

vd: đầu vào ('ahihi', 3)

Thì Kết quả là:
```javascript
['ahihi', 'ahihi', 'ahihi']
```
Yêu cầu, viết ít nhất 2 cách khác nhau

## Bài 2
Viết 1 hàm để đảo ngược 1 mảng, không được dùng hàm `array.reverse()`

Vd input:
```javascript
['a', 1, '9', 'apple']
```
Thì output phải là:
```javascript
['apple', '9', 1, 'a']
```

## Bài 3
Xóa đi các giá trị được xem là sai

Vd intput:
```javascript
[0, 1, false, 2, undefined, '', 3, null]
```
Thì output là:
```javascript
[1, 2, 3]
```

## Bài 4
Tạo ra 1 array gồm các object có key và value tương ứng cặp array ban đầu

Vd intput:
```javascript
const data = [['a', 1], ['b', 2]]
```
Thì output là:
```javascript
{ a: 1, b: 2 }
```

## Bài 5
Sắp xếp mảng tăng dần

Vd intput:
```javascript
[6, 4, 0, 3, -2, 1]
```
Thì output là:
```javascript
[-2, 0, 1, 3, 4, 6]
```

## Bài 6
Kiểm tra input đầu vào có phải là object hay không?

Vd:
```javascript
const data = { a: 1 }
return true
```
```javascript
const data = [1, 2, 3]
return false
```

## Bài 7
Viết 1 hàm trả về các key (của 1 object) khác các key truyền vào
Vd:
```javascript
const obj = { a: 1, b: 2, c: 3, d: 4 }
// truyền vào a, c
return { b: 2, d: 4 }
```

## Bài 8
Viết hàm nhập vào 1 array có nhiều hơn 5 phần tử
Xóa phần tử số 2, 3 trong array
Return mảng sau khi đã xóa

## Bài 9
Viết hàm nhập vào 1 array có cấu trúc như ví dụ sau:
```javascript
const students = [
    { id: 1, name: 'Nguyễn Thị Tèo', score: 9.2 },
    { id: 2, name: 'Phạm Văn Bưởi', score: 2.3 },
    { id: 3, name: 'Hoàng Văn Nam', score: 3.7 },
    { id: 4, name: 'Vũ Ngọc Duy', score: 6.9 },
    { id: 5, name: 'Nguyễn Minh Nhật', score: 5.2 },
    { id: 6, name: 'Phí Duy Quân', score: 9.6 },
    { id: 7, name: 'Trần Minh Minh', score: 6.1 }
]
```
Hãy tạo 1 array mới, với cấu trúc sau:
```javascript
['Pass', 'Fail', 'Fail', 'Pass', 'Pass', 'Fail', 'Pass']
```
Điều kiện `Pass`:
- Điểm trên `5.0` và không có chữ `Duy` là tên đệm

## Bài 10
Cho array có cấu trúc như input bài 9

Hãy tìm các students có điểm là số mà tổng số nút của phần trước dấu thập phân và phần sau dấu thập phân cộng lại lớn hơn 5

Vd: 6.9 -> 6 + 9 = 5 (không lấy)

3.7 -> 3 + 7 = 0 (không lấy)
5.2 -> 5 + 2 = 7 (lấy)
