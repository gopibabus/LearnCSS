# 🔥Media Queries

<img src="./assets/images/media_queries.png" alt="media queries" width="700px">

## ⚡Syntax for Media Queries

```css
/* Smart Phone */
@media (max-width: 500px) {
	body {
		background: red;
	}

	#smartphone h1 {
		display: block;
	}
}

/* Tablets */
@media (min-width: 501px) and (max-width: 768px) {
	body {
		background: blue;
	}

	#tablet h1 {
		display: block;
	}
}

/* Normal */
@media (min-width: 769px) and (max-width: 1200px) {
	body {
		background: green;
	}

	#normal h1 {
		display: block;
	}
}

/* Wide Screen */
@media (min-width: 1201px) {
	body {
		background: purple;
	}

	#widescreen h1 {
		display: block;
	}
}

/* Landscape*/
@media (max-height: 500px) {
	body {
		background: orange;
	}

	#landcape h1 {
		display: block;
	}
}
```

> [⚽ DEMO](/place/to/media/queries/server)

## ⚡Load Custom CSS with condition

```html
<link
	rel="stylesheet"
	media="screen and (max-width: 768px)"
	href="mobile.css"
/>
```
