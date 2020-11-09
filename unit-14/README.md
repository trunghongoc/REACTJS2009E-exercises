# Bài tập buổi 14, thứ 2 (09-11-2020)

## Bài 1
Hãy tạo 1 menu có 2 cấp như hình bên dưới
Xem các hình ảnh trong https://github.com/trunghongoc/REACTJS2009E-exercises/tree/main/unit-14/imgs/shallow-menu

### Có cấu trúc menu như sau
![](https://github.com/trunghongoc/REACTJS2009E-exercises/blob/main/unit-14/imgs/shallow-menu/structure.png "")

### Khi không click vào 1 item nào cả, thì menu ở trạng thái `fold`
![](https://github.com/trunghongoc/REACTJS2009E-exercises/blob/main/unit-14/imgs/shallow-menu/menu-fold.png "")

### Khi hover vào 1 item nào đó trong menu, vd hover vào `Dashboard`
![](https://github.com/trunghongoc/REACTJS2009E-exercises/blob/main/unit-14/imgs/shallow-menu/menu-hover-dashboard.png "")

### Khi hover vào 1 item nào đó trong menu, vd: hover vào `Sales`
![](https://github.com/trunghongoc/REACTJS2009E-exercises/blob/main/unit-14/imgs/shallow-menu/menu-hover-sales.png "")

### Khi click vào 1 item nào đó, vd click vào `Dashboard` thì sẽ mở các menu con của `Dashboard`, click thêm lần nữa thì `fold`
![](https://github.com/trunghongoc/REACTJS2009E-exercises/blob/main/unit-14/imgs/shallow-menu/menu-dashboard-click.png "")

### Vd click vào `Users`
![](https://github.com/trunghongoc/REACTJS2009E-exercises/blob/main/unit-14/imgs/shallow-menu/menu-users-click.png "")

### Khi hover vào 1 menu con, vd hover vào 1 mục trong `Users`:
![](https://github.com/trunghongoc/REACTJS2009E-exercises/blob/main/unit-14/imgs/shallow-menu/menu-user-click-hover-item.png "")

### Lưu ý
- Xem cấu trúc menu tại https://github.com/trunghongoc/REACTJS2009E-exercises/blob/main/unit-14/menu/shallow.js
- Cố gắng thêm hiệu ứng vào

## Bài 2
Hãy tạo 1 menu đa cấp như hình bên dưới
(Xem hình ảnh ở https://github.com/trunghongoc/REACTJS2009E-exercises/tree/main/unit-14/imgs/deep-menu)

### Cấu trúc menu
![](https://github.com/trunghongoc/REACTJS2009E-exercises/blob/main/unit-14/imgs/deep-menu/structure.png "")

### Ở chế độ `fold`
![](https://github.com/trunghongoc/REACTJS2009E-exercises/blob/main/unit-14/imgs/deep-menu/nothing.png "")

### hover vào home
![](https://github.com/trunghongoc/REACTJS2009E-exercises/blob/main/unit-14/imgs/deep-menu/hover-home.png "")

### hover vào news
![](https://github.com/trunghongoc/REACTJS2009E-exercises/blob/main/unit-14/imgs/deep-menu/hover-news.png "")

### hover vào blog
![](https://github.com/trunghongoc/REACTJS2009E-exercises/blob/main/unit-14/imgs/deep-menu/hover-blog.png "")

#### hover vào blog, sau đó hover vào missions
![](https://github.com/trunghongoc/REACTJS2009E-exercises/blob/main/unit-14/imgs/deep-menu/hover-blog-mission.png "")

#### hover vào blog, sau đó hover vào missions, sau đó hover vào our team
![](https://github.com/trunghongoc/REACTJS2009E-exercises/blob/main/unit-14/imgs/deep-menu/hover-blog-our-team.png "")

#### hover vào blog, sau đó hover vào missions, sau đó hover vào our team, sau đó hover vào 1 người bất kỳ
![](https://github.com/trunghongoc/REACTJS2009E-exercises/blob/main/unit-14/imgs/deep-menu/hover-blog-our-team-gleb.png "")

### Lưu ý
- Mỗi item được hover sẽ được chuyển màu sang màu cam
- Những item cha (cấp 1) nào đang được active, `isActive = true`, thì sẽ hiển thị như `ABOUT US`
- Xem cấu trúc menu tại https://github.com/trunghongoc/REACTJS2009E-exercises/blob/main/unit-14/menu/deep.js
- Cố gắng thêm hiệu ứng vào

## Bài 3
Hãy tạo 1 array là danh sách của timeline, sau đó tạo giao diện từ array vừa tạo theo yêu cầu là hình bên dưới

![](https://github.com/trunghongoc/REACTJS2009E-exercises/blob/main/unit-14/imgs/timeline/vertical-timeline.png "")