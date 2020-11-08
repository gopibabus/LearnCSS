# 🔥The Cascade

The CSS Cascade algorithm uses the following order:

1. Origin & Importance
2. Specificity
3. Order of Appearance

These are based on author declarations(our order of writing styles)

1. Linked Style Sheets
2. Embedded Styles (the **style** attribute in html element)
3. Inline Styles

These are things we write. It could be from our stylesheet, Javascript adding an inline style, or event from **@import**. Whatever the situation, we have control over styles. And all fall under **Order of Appearance**

### Order of Appearance

!> Which color would following divs be?

```css
.red {
color: red;
}

.blue {
color: blue;
}
```

```html
<div class="red blue">
<div class="blue red">
```

?> **ANSWER**: blue color is applied.

### Origin & Importance

!> Which color would following divs be?

```css
.red {
color: red !important;
}

.blue {
color: blue;
}
```

```html
<div class="red blue">
<div class="blue red">
```

?> **ANSWER**: red color is applied.

When **!important** comes to play?

1. Important **user** declarations.🤔
2. Important **author** declarations.
3. **Author** declarations.
4. **User** declarations.
5. **User Agent** declarations.

?> Order Of Precedence

1. Author Declarations
1. User Declarations
1. User Agent Declarations

?> Order Of Precedence when animations & transitions come to play:

1. important user declarations
1. important author declarations
1. animations
1. transitions
1. Author declarations
1. User declarations
1. User agent declarations

### Specificity

**Specificity** is one of the ways that the browser decides which declaration to use on a given element (if there are 2 or more conflicting styles). The higher the specificity, the more important that selector is considered to be, so it will win.

!> Which color would following divs be?

```css
.red.blue {
color: purple;
}

.red {
color: red;
}

.blue {
color: blue;
}
```

```html
<div class="red blue">
<div class="blue red">
```

?> **ANSWER**: purple color is applied.

!> It is better to avoid **specificity** from CSS and keep it flat i.e, use only one class to apply styles to a given element in the DOM.

!> If we avoid **specificity**, then there is no way **Origin and Importance** matters.

!> So ultimately we are depending on **Order of Appearance** 😃, which is way cleaner way to write CSS.

!> The caveat of writing flat css classes is that every style we write are avialable in global scope.
