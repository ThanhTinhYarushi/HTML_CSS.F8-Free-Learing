# Basic

## 1. .class
`-> Chọn tất cả thẻ có class-name  `
## 2. .class1.class2
`-> Chọn thẻ có 2 class đó (Class1class2) ` 
## 3. .class1 .class2
`-> class 2 phải là con class 1`  
`=> Chọn tất cả các thẻ có class = "name2" là con cuat 1 phần tử có class "name1"`  
## * 
`-> chọn tất cả thẻ`
## 4. element
`-> Chọn tất cả thẻ element(vd h1,h2,...)`
## 5. element.class
`-> Chọn các thẻ element có class  `
## 6. elment, elment
`Ví dụ có 3 thẻ html và có các class khác nhau nhưng mỗi thẻ lại có giống nhau và đều có 1 điểm chung`
`Ví dụ 3 thẻ đều cùng 1 màu và khác font-style`
```html
    <div>
        <h2 class="title1">Ví dụ về element, element</h2>
        <h2 class="title2">Ví dụ về element, element</h2>
        <h2 class="title3">Ví dụ về element, element</h2>
    </div>
```
```css
.title1, .title2, .title3{
    color:darkolivegreen;
}
.title1{
    font-style: italic;
}
.title2{
    text-decoration: line-through;
}
.title3{
    text-decoration: underline;
}
```
`Cach 2`
```html
<h2 class="title1 red-color">Ví dụ về element, element</h2>
        <h2 class="title2 red-color">Ví dụ về element, element</h2>
        <h2 class="title3 red-color">Ví dụ về element, element</h2>
```
```css
.red-color{
    color: red;
}
```
## 7. element1 element2
-> element2 sẽ là con của element1
## 8 . element > element
-> Chọn con trực tiếp của ele bên trái
```html
<div>
        <h2 class="title9">Ví dụ ele > ele</h2>
        <div class="box9">
            <h2 class="title9">đây là con trực tiếp, Ví dụ ele > ele</h2>
            <div>
                <h2 class="title9">Ví dụ ele > ele</h2>
            </div>
        </div>
</div>
```
```css
.box9 > .title9{
    color: aqua;
}
```
## 9. ele + ele
-> chọn các thẻ liền kề phía sau

```html css
<div>
        <h3 class="title10">Ví dụ về element + element</h3>
        <h3 class="title10">Ví dụ về element + element</h3>
        <h3 class="title10">Ví dụ về element + element</h3>
        <h3 class="title10">Ví dụ về element + element</h3>
        <h3 class="title10">Ví dụ về element + element</h3>
        <h3 class="title10">Ví dụ về element + element</h3>
        <h3 class="title10">Ví dụ về element + element</h3>
        <h3 class="title10">Ví dụ về element + element</h3>
        <h3 class="title10">Ví dụ về element + element</h3>
        <h3 class="title10">Ví dụ về element + element</h3>
    </div>
.title10 + .title10{
    color: brown;
}
```
## 10. ele ~ ele
-> chọn các thẻ liền kề anh em