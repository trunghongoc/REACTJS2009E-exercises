# Bài tập buổi 15, thứ 2 (16-11-2020)

## Bài 1
Hãy dùng bootstrap 4 để tạo bảng với yêu cầu:

Có thể `add`, `edit`, và `delete`, `select all`

### Có cấu trúc như sau
![](https://github.com/trunghongoc/REACTJS2009E-exercises/blob/main/unit-15/imgs/table/editable.png "")

Khi nhấn vào nút `edit` sẽ chuyển sang chế độ edit của row chứa nút vừa click
- Dòng có id bằng 3 là 1 dòng đang ở trạng thái edit
- Ở trạng thái edit, nút `edit` bị ẩn đi, thay vào đó là 2 nút: `save` và `cancel`, có thể chỉnh sửa mọi  thông tin ngoại trừ `id`
- Khi nhấn nút `save` thì quay về dạng hiển thị ban đầu với nội dung mới (nội dung vừa chỉnh sửa), ẩn nút `save` và `cancel` đi, hiển thị nút `edit`
- Khi nhấn nút `cancel` thì quay về dạng hiển thị ban đầu với nội dung cũ (nội dung trước khi chỉnh sửa), ẩn nút `save` và `cancel` đi, hiển thị nút `edit`
- Khi nhấn nút `delete` ở 1 dòng nào đó, thì xóa dòng đó khỏi bảng
- Khi nhấn nút `delete` của cả bảng (nút bên góc trên, bên phải của bảng, bên cạnh nút add) thì sẽ phải xóa các dòng đang được `selected`
- Khi nhấn nút `add` thì thêm 1 dòng mới vào cuối bảng ở trạng thái `edit`, trong đó phải tạo `id` sao cho không bao giờ bị trùng `id` với các dòng khác


## Bài 2
Làm lại các bài menu buổi 14 cho đến khi được thì thôi, bắt buộc phải làm được bài timeline và menu 2 cấp

## Bài 3
Trong 1 trận đấu pokemon, bạn được phép chọn tối đa 5 pokemon mà mình muốn

Mỗi pokemon có chỉ số `HP` và `ATK` khác nhau, cụ thể như data bên dưới

```javascript
const pokemons = [
    { id: 1, name: 'Charmander', hp: 39, atk: 52 },
    { id: 2, name: 'Pikachu', hp: 35, atk: 55 },
    { id: 3, name: 'Squirtle', hp: 44, atk: 48 },
    { id: 4, name: 'Bulbasaur', hp: 45, atk: 49 },

    { id: 5, name: 'Mew', hp: 100, atk: 100 },
    { id: 6, name: 'Pidgey', hp: 40, atk: 45 },
    { id: 7, name: 'Abra', hp: 25, atk: 20 },
    { id: 8, name: 'Snorlax', hp: 160, atk: 110 },

    { id: 9, name: 'Caterpie', hp: 45, atk: 30 },
    { id: 10, name: 'Dratini', hp: 41, atk: 64 },
    { id: 11, name: 'Eevee', hp: 55, atk: 55 },
    { id: 12, name: 'Jigglypuff', hp: 115, atk: 45 }
]
```

### Hình minh họa (đang select Squirtle)
![](https://github.com/trunghongoc/REACTJS2009E-exercises/blob/main/unit-15/imgs/pokemon/click-to-squirtle.png "")

### Đang select Pidgey
![](https://github.com/trunghongoc/REACTJS2009E-exercises/blob/main/unit-15/imgs/pokemon/click-to-pidgey.png "")

### Khi đã nhấn add Pidgey
![](https://github.com/trunghongoc/REACTJS2009E-exercises/blob/main/unit-15/imgs/pokemon/added-pidgey.png "")
- Nút chuyển màu (không click được nữa)
- Không thể add lại Pidgey, muốn add lại phải xóa Pidgey đi
- Icon của Pidgey sẽ mờ đi, và không cho phép click vào nữa

### Khi chọn pokemon thứ 5 (đã đủ số pokemon)
Show text sau: `You have selected 5 Pokemons.`
![](https://github.com/trunghongoc/REACTJS2009E-exercises/blob/main/unit-15/imgs/pokemon/add-max-pokemon.png "")

### Khi nhấn xóa 1 pokemon nào đó trong danh sách 5 pokemon
- Hình pokemon vừa xóa sẽ sáng trở lại
- Có thể xóa pokemon vị trí bất kỳ
- Sau khi xóa 1 pokemon, ví dụ xóa pokemon thứ 2 trong danh sách thì pokemon thứ 3 sẽ vào vị trí pokemon thứ 2, 4 vào 3, và 5 vào 4 (các vị trí trống phải là các vị trí cuối danh sách)

### Khi double click vào "Double click to edit"
- Có thể chỉnh sửa text như hình:
![](https://github.com/trunghongoc/REACTJS2009E-exercises/blob/main/unit-15/imgs/pokemon/click-to-edit.png "")
- Khi nhấn enter thì thoát chế độ chỉnh sửa và hiển thị text mới

### Hãy dùng font sau cho bài 3
```css
@import url('https://fonts.googleapis.com/css?family=Roboto:300|Shadows+Into+Light');
```