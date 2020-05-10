# 🔥Selectors

## ⚡Targeted Selectors

```css
/* Direct Child */
div > p {
	background-color: #ddd;
}

/* Directly after */
div + P {
	background-color: #333;
	color: #fff;
}

/* By Attribute */
a[target] {
	background-color: red;
	color: #fff;
}

a[target='_self'] {
	background-color: skyblue;
	color: #333;
}

/* Specific Attribute values */
input[type="text"] {
	width: 100%;
	margin-bottom: 5px;
}
```

## ⚡Pseudo Selectors

```css
/* first child */
li:first-child {
	background-color: red;
}

/* last child */
li:last-child {
	background-color: red;
}

/* Position 3 */
li:nth-child(3){
	background-color: purple;
}

/* Every 3rd Child */
li:nth-child(3n+0) {
	background-color: orange;
}

/* Every 3rd Child after 5*/
li:nth-child(3n+5) {
	background-color: blue;
}

/* Every odd number element*/
li:nth-child(odd) {
	background-color: yellow;
}
```

## ⚡before & after Pseudo Selectors

```css
/* after */
/* place content after the element */
.required:after {
	content: '*';
	color: red;
	padding-left: 2px;
}

/* before */
/* place content before the element */
header:before {
	content: '';
	background: url(https://source.unsplash.com/random) no-repeat center center/cover;
	opacity: 0.3;
	position: absolute;
	top: 0;
	left: 0;
	width: 100%;
	height: 100%;
	z-index: -1;
}
```

## ⚡Shadows

### ✳Box Shadows

```css
.container {
	display: flex;
}

.box {
	padding: 1rem;
	margin: 1rem;
	background-color: coral;
	color: #fff;

	/* offset-x, offset-y, color */
	box-shadow: 10px 10px teal;
	/* offset-x, offset-y, blur-radius, color */
	box-shadow: 10px 10px 20px teal;
	/* Negative Values */
	box-shadow: -5px -5px 20px teal;
	/* offset-x, offset-y, blur-radius, spread-radius color */
	box-shadow: 3px 3px 10px 1px teal;
	/* inset, offset-x, offset-y, color */
	box-shadow: inset 3px 3px teal;
	/* Multiple Shadows */
	box-shadow: 3px 3px teal, -3px -3px coral;
}

```

## ⚡Animations

### ✳Keyframes

```css
box {
	background: white;
	width: 200px;
	height: 200px;
	position: relative;
	/* animation-name: animate1;
	animation-duration: 2s;
	animation-iteration-count: 3;
	animation-fill-mode: forwards;
	animation-delay: 2s;
	animation-direction: alternate-reverse;
	animation-timing-function: ease-in-out; */
	animation: animate1 5s forwards 1s ease-in-out;
}

@keyframes animate1 {
	from {
		top: 0;
		width: 200px;
	}

	to {
		width: 600px;
		background-color: blueviolet;
		top: 300px;
	}

	25% {
		top: 0%;
		left:300px;
		background-color: red;
	}

	50% {
		top:300px;
		left:300px;
		background-color: green;
	}

	75%{
		top:300px;
		left:0;
		background-color: aquamarine;
	}

	100%{
		top:0;
		left: 0;
	}
}
```

### ✳Transition

```css
.box {
	background-color: wheat;
	width: 100px;
	height: 100px;
	/* transition-property: background;
	transition-duration: 2s;
	transition-timing-function: ease-in-out;
	transition-delay: 3s; */
	transition: all 2s ease-in-out;
}

.box:hover {
	background: red;
	border-radius: 50%;
	height: 300px;
	width: 300px;
}
```

### ✳Transform

```css

```

