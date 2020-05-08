# 🔥CSS Properties and Values

?>⭐Every CSS Style inherits the styles already applied to its parent HTML element.

### ✳Common CSS property and value combinations

- Set font color to white

```css
div {
	color: #ffffff;
}
```

- Set background color to black

```css
div {
	color: #000000;
}
```

- Create 1px thick blue border around element

```css
div {
	border: 1px solid blue;
}
```

- Set font to Arial

```css
div {
	font-family: Arial, sans-serif;
}
```

- Set font size to 16px

```css
div {
	font-size: 16px;
}
```

- Add padding 32px thickness in size

```css
div {
	padding: 32px;
}
```

- Add 16px of margin around the content area

```css
div {
	margin: 16px;
}
```

## ⚡Variables, calc()

### ✳Variables in CSS

<!-- tabs:start -->

#### **Without Variables**

```css
div {
	background-color: black;
}

section div span {
	color: black;
}

a {
	color: black;
}
```

#### **With Variables **

```css
:root {
	--primary-color: black;
}

div {
	background-color: var(--primary-color);
}

section div span {
	color: var(--primary-color);
}

a {
	color: var(--primary-color);
}
```

#### **With Fallback Values **

```css
:root {
	--primary-color: black;
}

div {
	background-color: var(
		--primary-color,
		#333
	); /* #333 if --primary-color is not defined */
}

section div span {
	color: var(
		--primary-color,
		#333
	); /* #333 if --primary-color is not defined */
}

a {
	color: var(
		--primary-color,
		#333
	); /* #333 if --primary-color is not defined */
}
```

<!-- tabs:end -->

!> When the browser encounters an **invalid var()** substitution, the initial or inherited value of the property is used.

[🌐 MDN Documentation](https://developer.mozilla.org/en-US/docs/Web/CSS/Using_CSS_custom_properties)

### ✳calc() CSS function

?> The **calc() CSS function** lets you perform calculations when specifying CSS property values. It can be used anywhere a **length, frequency, angle, time, percentage, number, or integer** is allowed.

```css
div {
	width: calc(10px + 100px);
	width: calc(100% - 30px);
	width: calc(2em * 5);
	width: calc(var(--variable-width) + 20px);
}
```

[🌐 MDN Documentation](https://developer.mozilla.org/en-US/docs/Web/CSS/calc)

## ⚡Shorthand Properties

### ✳background color

<!-- tabs:start -->

#### **Without Shorthand **

```css
div {
	background-color: #000000;
	background-image: url(iamge.png);
	background-repeat: no-repeat;
}
```

#### **Using Shorthand **

```css
div {
    background: #000000 url(image.png) no-repeat;
}
```

<!-- tabs:end -->

> TODO: Document various shorthand properties ☺

## ⚡Pseudo Selectors

* In CSS a pseudo-selector is any selector that starts with a **colon character (:)** and usually appended to the end of the element name.
* Pseudo-selectors **:first and :last** are used for selecting the very first or very last element from a list of children in a parent.
* **:nth-child** for selecting a series of elements belonging to a row or column in a list of elements or even an HTML table.

<img src="./assets/images/pseudo_selectors.png" alt="pseudo_selectors" width="700px">

* The same **nth-child** rules apply to all other nested groups of elements, like **ul and li** for example, and any other arbitrary parent/child combination.
* The **star (*)** selector selects all elements within a parent. for example, **table \*** selects all elements in a table.

?> 🎯 [::before](https://developer.mozilla.org/en-US/docs/Web/CSS/::before) & [::after](https://developer.mozilla.org/en-US/docs/Web/CSS/::after)

[🌐 MDN Documentation](https://developer.mozilla.org/en-US/docs/Web/CSS/Pseudo-classes)
