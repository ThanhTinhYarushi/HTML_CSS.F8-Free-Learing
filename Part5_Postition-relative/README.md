## css position

### relative -> tuong doi

```css
margin-top: 100px;
/* đẩy xuóng dưới */
position: relative;
top: 100px;
/* đè lên  */
```

vị trí tương đối sẽ lấy chính mình làm gốc toạ độ

### absolute -> tuyet doi

lấy thẻ cha gần nhất có thuộc tính position làm gốc toạ độ

```html
<div class="box">
  <div class="box-child"></div>
</div>
```

```css
.box {
  width: 100%;
  height: 120px;
  background-color: #333;
  position: relative;
}
.box-child {
  width: 50px;
  height: 50px;
  background-color: ivory;
  position: absolute;
  top: 50px;
  right: 200px;
  border: 2px solid red;
  box-sizing: border-box;
}
```

- làm mờ

```css
.box-child {
  background-color: rgba(255, 255, 255, 0.5);
  position: absolute;
  top: 0;
  bottom: 0;
  right: 0;
  left: 0;
}
```

#### TH2

```html
<div class="box">
  <div class="box2">
    <div class="box-child"></div>
  </div>
</div>
```

```css
.box2 {
    width: 200px;
    height: 60px;
    background-color: aquamarine;
    position: relative;



    /* cach 2*/
    position: absolute;
    box 2 lam con box 1 va la cha box-child
}
```

### fixed -> phu thuoc khung trinh duyet

dùng để tạo header hoặc element cố định

```css
.header {
  width: 100%;
  height: 100px;
  background-color: darkslategrey;
  position: fixed;
  top: 0;

  /* có thể không đặt width */
  right: 0;
  left: 0;
}
```

### sticky -> bam dinh

```css
.header-sticky {
  margin-top: 30px;
  width: 100%;
  height: 40px;
  background-color: firebrick;
  position: sticky;
  position: -webkit-sticky;
  top: 0;
}
```

### chú ý

nếu thẻ nào phụ thuộc dùng absolute, cố định dùng fixed
