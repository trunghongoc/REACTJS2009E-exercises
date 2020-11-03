# Bài tập buổi 13 02-11-2020

## Bài 1
Hãy tạo 2 ô input nhập số, và 1 button "Tính tổng"
Hãy tính tổng của 2 số nhập vào khi click nút "Tính tổng"

## Bài 2
Tạo 1 thẻ div có kích thước 100px 100px, có màu nền là màu đỏ
Hãy viết hàm click, sao cho khi click vào thẻ div vừa rồi, nếu màu nền đang màu đỏ sẽ chuyển thành màu xanh lá cây, nếu đang màu xanh lá cây sẽ chuyển sang màu đỏ

## Bài 3
Hãy tạo 1 thẻ select có các mục là: Laptop, Điện thoại, Tivi

Laptop bao gồm:
- Macbook
- Dell
- Lenovo
- Asus

Điện thoại bao gồm:
- Apple
- Samsung
- Nokia

Tivi bao gồm:
- LG
- Sony

Khi chọn 1 option (Laptop hoặc Điện thoại hoặc Tivi), hãy show các hãng của option đang chọn lên màn hình để người dùng có thể thấy được dưới dạng ul li hoặc ol li

## Bài 4
Cho array sau
```javascript
const menu = [
    {
        name: 'Home',
        children: [
            {
                name: 'Home 1',
                children: [
                    {
                        name: 'Home 1.1',
                        children: [
                            { name: 'Home 1.1.1' }
                        ]
                    },
                    {
                        name: 'Home 1.2',
                        children: [
                            { name: 'Home 1.2.1' }
                        ]
                    }
                ]
            },
            {
                name: 'Home 2',
                children: [
                    {
                        name: 'Home 2.1'
                    }
                ]
            },
            {
                name: 'Home 3',
                children: [
                    {
                        name: 'Home 3.1'
                    }
                ]
            }
        ]
    },
    {
        name: 'About',
        children: [
            {
                name: 'About 1',
                children: [
                    {
                        name: 'About 1.1',
                        children: [
                            { name: 'About 1.1.1' }
                        ]
                    },
                    {
                        name: 'About 1.2',
                        children: [
                            {
                                name: 'About 1.2.1',
                                children: [
                                    { name: 'About 1.2.1.1' },
                                    { name: 'About 1.2.1.2' },
                                    { name: 'About 1.2.1.3' }
                                ]
                            }
                        ]
                    }
                ]
            },
            {
                name: 'Home 2',
                children: [
                    {
                        name: 'Home 2.1'
                    }
                ]
            }
        ]
    }
]
```

Hãy tạo ra 1 menu bằng array bên trên bằng ul li hoặc ol li,
di chuột vào item cha (menu cha) sẽ show menu con
