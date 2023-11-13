# Padding, Margin, Box-sizing
-> padding border đều làm tăng kích thước của elements
## Padding
có nghĩa là đệm thêm
```css
.box1{
    background-color: #333;
    padding-top: 10px;
    padding-left: 10px;
    padding-right: 10px;
    padding-bottom: 10px;
    /* Viết Tắt sẽ đệm cả 4 hướng */
    padding: 10px;
    padding: 10px 12px; -> cái đầu bên trên/dưới, cái sau trái phải
    padding: 10px 12px 8px; -> cái đầu bên trên, cái sau bên trái phải, cái cuối bên dưới
    padding: 10px 12px 8px 6px; -> theo chiều kim đồng hồ

}
```

## Border
-> là lớp được định nghĩa là lớp vỏ của 1 elements, khi inspect sẽ thấy nét liền
```css
.box1{
    background-color: #333;
    padding: 10px;
/*************************************
 *           CƠ BẢN BORDER           *
 * BORDER-WIDTH -> CHIỀU RỘNG BORDER *
 *       BORDER-STYLE -> STYLE       *
 *       BORDER-COLOR -> COLOR       *
 *************************************/
    border-width: 10px;
    border-style: solid;
    border-color: red;
}
```

********************************************************************
 *                          /* VIẾT DÀI */                           *
 *                      BORDER-TOP-WIDTH: 10PX;                      *
 *                     BORDER-RIGHT-WIDTH: 12PX;                     *
 *                     BORDER-BOTTOM-WIDTH: 8PX;                     *
 *                     BORDER-LEFT-WIDTH: 12PX;                      *
 * /* CHỈ TOP -> BORDER STYLE SOLID CÓ KIỂU WIDTH MẶC ĐỊNH LÀ 20PX*/ *
 *                      BORDER-TOP-WIDTH: 10PX;                      *
 *                     BORDER-RIGHT-WIDTH: 0PX;                      *
 *                     BORDER-BOTTOM-WIDTH: 0PX;                     *
 *                      BORDER-LEFT-WIDTH: 0PX;                      *
 ********************************************************************

/***************************
 *        VIẾT NGẮN        *
 * BORDER: 10PX SOLID RED; *
 ***************************/