# 🔥CSS Tricks

### 😃CSS combinator * + * { }

<iframe width="1080" height="520" src="https://www.youtube.com/embed/cuEHx9DoWI4" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

### 😃:focus-within

```css
.cta:hover,
.cta:focus-within {
    transform:scale(1.1);
}
```

[🌐 Reference](https://developer.mozilla.org/en-US/docs/Web/CSS/:focus-within)

[🌐 Reference](https://css-tricks.com/almanac/selectors/f/focus-within/)

<iframe width="1080" height="520" src="https://www.youtube.com/embed/2-xdcDsqsAs" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

### 😃all:unset

?> The **all property in CSS** resets all of the selected element’s properties.

```css
.module {
  all: unset;
}
```

> [🌐 Reference](https://css-tricks.com/almanac/properties/a/all/)

<iframe width="1080" height="520" src="https://www.youtube.com/embed/0GcTUor2ANw" frameborder="0" allow="accelerometer; autoplay; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>

### 😃@supports

?> The **@supports** CSS at-rule lets you specify declarations that depend on a browser's support for one or more specific CSS features.

```css
@supports (display: grid) {
  div {
    display: grid;
  }
}
@supports not (display: grid) {
  div {
    float: right;
  }
}
```

> [🌐 Reference](https://developer.mozilla.org/en-US/docs/Web/CSS/@supports)

### 😃CSS Scroll Snap

?> **CSS Scroll Snap** is a module of CSS that introduces scroll snap positions, which enforce the scroll positions that a scroll container’s scrollport may end at after a scrolling operation has completed.

```css
/*.one and .two are child elements of body*/

body {
  scroll-snap-type:y mandatory;
  overflow-y: scroll;
}

.one {
  background-color: red;
  color:white;
  text-align: center;
  height: 100vh;
  scroll-snap-align: start;
}

.two {
  background-color: skyblue;
  color:black;
  text-align: center;
  height: 100vh;
  scroll-snap-align: start;
}
```

> [🌐 Reference](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Scroll_Snap)

> [🌐 Video Reference](https://www.youtube.com/watch?v=Xs4uzHm_8-o)