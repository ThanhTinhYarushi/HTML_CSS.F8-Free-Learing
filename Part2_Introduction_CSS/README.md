# CSS
## Có 3 cách
`Internal`  
    Bên Trong
`External`   
    Bên ngoài
`Inline`  
    Trong thẻ  
## Class & id
`HTML & Css cơ bản: id vs class`
```html
        <!-- Class -> . -->
        <!-- Id -> # -->
        <h1 id="first-heading">CSS selector</h1>
        <h1 id="second-heading">CSS selector</h1>
        <h1 id="third-heading">CSS selector</h1>
        <h2 class="second-heading">ID & CLASS</h2>
        <h2 class="second-heading">ID & CLASS</h2>
        <h2 class="second-heading">ID & CLASS</h2>
```
```css
#first-heading{
    color: green;
}
#second-heading{
    color: red;
}
#third-heading{
    color:rebeccapurple;
}

.second-heading{
    color:pink;
}
```
## Độ ưu tiên
`- Internal, External:`
-> Cái nào viết mới hơn sẽ ưu tiên hơn
`- Inline : 1000`
`- #id : 100`
`- class : 10`
`- tag : 1`
`- Equal specificity`
-> Sự giống nhau khi gọi element, ai mới hơn lại đc ưu tiên, hoặc áp dụng class + id để có 110 đ ... v.v ..
`- Universal selector and inherited`
-> tất cả thẻ chung được áp dụng nhưng độ ưu tiên nhỏ nhất.
`- important`
        `!important`
            ->`Áp dụng cao nhất`