# 居中布局


HTML 结构统一如下：

```html
<div class="parent">
  <div class="child"></div>
</div>
```

### inline-block

```css
.parent {
  text-align: center;
}
.child {
  display: inline-block;
}
```

### flex

```css
.parent {
  display: flex;
  align-items: center;
  justify-content: center;
}
```

### position

```css
.parent {
  position: relative;
}
.child {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
}
```

### table

```css
.parent {
  display: table-cell;
  text-align: center;
  vertical-align:middle;
}

.child {
  display: inline-block;
  vertical-align: middle;
}
```
