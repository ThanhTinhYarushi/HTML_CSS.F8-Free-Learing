## background-image
```css
.header{
        width: 100%;
        height: 100vh;
        background-image: url(https://image2.tin247.news/pictures/2023/06/14/azj1686688230.jpg);
        /* background-repeat: no-repeat; */
        background-size: 250px auto;
                        /*width height*/
    }
```

### linear-gradient

background-image: linear-gradient( 0, blue, yellow)  
- tham số đầu là hướng xoay
- thứ 2 là màu dưới
- thứ 3 là màu trên
- muốn đổi hướng xoay thì 180deg, 90deg, -90deg, ...
- mặc định nếu không có tham số thứ nhất thì sẽ là 180deg

* có thể áp dụng linear-gradient với url: -> sử dụng rgba()
```css
background-image: linear-gradient( 0, rgba(255, 255, 0, 0.5), rgba(53, 77, 211, 0.54)),
            /* url(https://s3.getstickerpack.com/storage/uploads/sticker-pack/han-hyo-joo/sticker_10.png?aef76da60ed39ce78a5224e6f0ba9fc0&d=200x200) , */
            url(https://image2.tin247.news/pictures/2023/06/14/azj1686688230.jpg);
``` 

## background-size
### background-size: contain;
chia tỷ lệ càng lớn càng tốt trong vùng chứa của nó mà không cắt xén hình ảnh/ hay che khất hình ảnh.  
`nói chung là lấy chiều bức ảnh dài nhất` 
### background-size: cover;
-> giống như contain nhưng nó có thể cắt hình ảnh, `sẽ toàn màn hình`
`
Chia tỷ lệ hình ảnh (trong khi vẫn giữ nguyên tỷ lệ của nó) đến kích thước nhỏ nhất có thể để lấp đầy vùng chứa (nghĩa là: cả chiều cao và chiều rộng của nó đều che phủ hoàn toàn vùng chứa), không để lại khoảng trống. Nếu tỷ lệ của nền khác với phần tử, hình ảnh sẽ bị cắt theo chiều dọc hoặc chiều ngang.
`