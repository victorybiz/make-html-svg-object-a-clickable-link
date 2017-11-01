# Make HTML SVG object a clickable link
This works on the SVG and on the fallback image.

```css
a.svg {
  position: relative;
  display: inline-block; 
}
a.svg:after {
  content: ""; 
  position: absolute;
  top: 0;
  right: 0;
  bottom: 0;
  left:0;
}
```

```html
<a href="#" class="svg">
  <object data="file-name.svg" type="image/svg+xml">
    <img src="file-name.jpg" />
  </object>
</a>
```
