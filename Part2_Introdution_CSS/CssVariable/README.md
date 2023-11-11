## đặt tên biến:
--name-var: thucangan;
var(--name-var)
```css
:root{
    --text-color: red;
    /* global */
}
h1{
    --text-style-underline: underline;
    /* local */
    text-decoration:var(--text-style-underline);
    color: var(--text-color);
}
h2{
    color: var(--text-color);
}
h3{
    color: var(--text-color);
}
```