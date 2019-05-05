# 总结常见CSS布局的各种实现方法

## 居中布局

+ [inline-block](./居中布局/center-inline-block.html)
+ [position](./居中布局/center-position.html)
+ [flex](./居中布局/center-flex.html)
+ [table](./居中布局/center-table.html)

HTML 结构如下：

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
