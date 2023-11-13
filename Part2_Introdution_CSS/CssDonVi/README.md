# CSS Units

## Absolute units - Đơn vị tuyệt đối
### px
-> 1px dựa theo độ phân giải màn hình  
->> Kích thước cố định
### pt
### cm
### mm
### inch
### pc

## Relative units - Đơn vị tương đối
đều cần nơi phụ thuộc vào
### %
`->phụ thuộc vào thẻ chứa nó, như <body> -> phụ thuộc vào trình duyệt`
### rem
`->phụ thuộc vào thẻ html`  
```html
<div class="text-rem"> hihi </div>
```
```css
html{
    font-size: 100px;
}

.test-rem{
    font-size: 1rem;
}
```
### em
`-> phụ thuộc vào thẻ gần nhất chứa nó có thuộc tính css, vd font-size`
```html
<!DOCTYPE html>
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="style.css">
    <title>Tiêu đề</title>
</head>

<body>
    <h1>CSS units</h1>
    <div class="box-absolute"></div>
    <div class="box-relative"></div>
    <div class="text-rem"> hihi </div>
    <div class="text-em"> size em</div>
    </div>
</body>

</html>
```
=> thẻ gần nhất chứa nó và có thuộc tính css là html với fontsize 100px ở trên
```html
<div class="text-em" style="font-size: 15px;">
        <p style="font-size: 2em;">test em</p>
</div>
```

### vw
`viewport width: độ rộng của trình duyệt`
!!! khác với % vì % phụ thuộc vào thẻ chứa nó, còn vw, vh thì phụ thuộc vào kích thước trình duyệt
### vh
`viewport height : độ cao`

```css
.box-vw-vh{
    width:100vw ;
    height: 10vh;
    background-color: blue;
}
```
lúc này sẽ dựa vào trình duyệt mà boxvwvh sẽ có độ cao 10 và 100 chiều rộng theo trình duyệt
### vmin
### vmax
### ex
### ch


# Chú Ý
Thường thì sẽ sử dụng rem:
luôn phụ thuộc vào html -> dễ kiểm soát hơn
nên set font-size html như này:
```css
html{
    font-size: 100%;
}
```
->vậy thì 1rem sẽ bằng 16px

```
Con số 62.5% là gì?
Mặc định font-size của thẻ html là 16px - tương ứng với 100%. Khi ấy, 1rem sẽ bằng 16px. Vậy khi muốn đặt font-size tương ứng với 10px thì ta sẽ đặt bằng bao nhiêu rem?

Đương nhiên, theo mặc định 10px đổi sang rem sẽ là 10/16 = 0.625, như vậy để CSS bằng đơn vị rem ra được kích cỡ tương ứng 10px ta sẽ CSS là font-size: 0.625rem.

👉 Khá hại não khi phải quy đổi như vậy. Vì vậy, chúng ta có thể quy đổi tỉ lệ tại thẻ html với CSS font-size: 62.5%. Kết quả thu được, 1rem = 10px, 1.6rem = 16px, 2rem = 20px, 2.4rem = 24px.

Đơn vị rem được sử dụng với font-size trong rất nhiều website. Cách quy đổi font-size: 62.5% cũng có thể được coi là một mẹo giúp chúng ta dễ dàng sử dụng đơn vị rem hơn.
```