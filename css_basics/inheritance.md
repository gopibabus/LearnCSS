# 🔥Inheritance

> Anything related to **TYPOGRAPHY** is inherited. Everything we see on the page is a child of **html** element, so they inherit those properties.

* font-size
* font-family
* font-weight
* line-height
* text-decoration
* color
* text-align
* text-transform etc.,

```css
html {
  font-family: 'really-nice-font', sans-serif;
  font-size: 1.125rem;
  font-weight: 400;
  line-height: 1.7;
}
```

> Anything related to **LAYOUT** is not inherited.

* margin
* padding
* height
* width
* position etc.,

> Following elements not inherited any properties, because of **browser defaults**

* \<button\>
* \<input\>
* \<optgroup\>
* \<select\>
* \<textarea\>

we can manually make above mentioned elements to inherit parent properties:

```css
button,
input,
optgroup,
select,
textarea {
  font-family: inherit;
}

a {
  color: inherit;
}

h2, h3, h4 {
  font-weight: inherit;
}
```

> Font size that we applying on every element in HTML DOM are relative to **html** element. So try to make sure properties like font-size are constant and are not changed on **html** element in our applications.

> TIP: Make sure to **enable browser styles** from **settings in firefox developer tools**.

[🌍 Typography Reference](https://cssreference.io/typography/)

[🌍 Inheritance Reference](https://developer.mozilla.org/en-US/docs/Web/CSS/inheritance)

[🌍 Inheritance Reference 2](https://developer.mozilla.org/en-US/docs/Learn/CSS/Building_blocks/Cascade_and_inheritance)

[🌍 Inheritance Sitepoint](https://www.sitepoint.com/css-inheritance-introduction/)
