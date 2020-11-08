# 🔥rem & vh units

## ⚡em & rem units

> 💡It is recommended to use rem units than px units because rem units can scale relative to parent elements.

<img src="./assets/images/rem.png" alt="rem" width="700px">

```css
#box-1 {
	font-size: 20px;
}

/* em unit multiply it's value with parent element value */

#box-1 p {
	font-size: 1.5em; /* 20 * 1.5 = 30px */
	padding: 1em;
	/* 20 * 1 should be 20px but in reality it is 30px,
	   so we should not use em
	 */
}

#box-1 ul {
	font-size: 1.5 em; /* size is not controlled */
}

/* rem unit multiply it's value with root element(<html>) value */
html {
	font-size: 10px;
}

#box-2 h3 {
	font-size: 2rem; /* 2 * 10 = 20px */
}

#box-2 p {
	font-size: 1.6rem; /* 1.6 * 10 = 16px */
	line-height: 2rem; /* 2 * 10 = 20px */
}
```

> 💡It is recommended to use rem units than em units for responsive designs and accessibility reasons.

## ⚡vh & vw units

<img src="./assets/images/vh.png" alt="view height">

```css
header {
	background: #333 url('https://source.unsplash.com/daily') no-repeat center
		center/cover;
	color: #fff;
	/* Divide total viewport height in to 100 horizontal pieces */
	height: 100vh;
	/* By default images or content occupies total width of view port. */
	width: 100vw;
	text-align: center;
	padding: 2rem;
	padding-top: 15rem;
}

header h1 {
	font-size: 3rem;
	color: burlywood;
}

header p {
	margin: 1rem 0;
	color: indianred;
}

.btn {
	display: inline-block;
	text-decoration: none;
	background: burlywood;
	color: #333;
	padding: 0.75rem 2rem;
}

section {
	padding: 2rem;
}

@media (max-width: 450px) {
	header {
		padding-top: 5rem;
	}
}
```
