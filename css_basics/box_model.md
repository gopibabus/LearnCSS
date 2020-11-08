# 🔥CSS Box Model

### Box Sizing

```css
.element {
  box-sizing : border-box;
}
```

> Above **box-sizing** property tells the browser to account for any border and padding in the values you specify for an element's width and height. If you set an element's width to 100 pixels, that 100 pixels will include any border or padding you added, and the content box will shrink to absorb that extra width. This typically makes it much easier to size elements.

> **Margin** is spacing between elements. So it is not included as part of **border-box**.

Best way to include **border-box** in to our project:

```css
*,
*::before,
*::after {
  box-sizing : border-box;
}
```

> Above **border-box** style is applied to all elements in our DOM.

[🌍 Reference](https://developer.mozilla.org/en-US/docs/Web/CSS/box-sizing)

### Element Width

There is **no need to add width on every element**. Without adding width to element, it can auto adjust to different view ports. Use width when it is required along with **border-box** property.

```css
.content {
  box-sizing: border-box;
  width: 100%;
  border: 10px solid red;
  padding: 10px;
  margin-top: 10em;
  background: white;
  box-shadow: 0 0 3em rgba(0,0,0,.15);
}
```

[🌍 Example](https://codepen.io/kevinpowell/pen/592bb3d9c8f61e2e53444890ec1e0c65)

### Element Height

Setting heights is dangerous relative to responsive layouts. So it is better to avoid setting **height** on elements. If you have a requirement to set height, it is ideal to use **min-height**. If you have to change element height, it is better to use **padding** property instead of using **height** property.

```css
.content {
  background: white;
  margin: 0 1em;
  padding: 10em 3em;
  box-shadow: 0 0 3em rgba(0,0,0,.15);
  width: 100%;
}
```
