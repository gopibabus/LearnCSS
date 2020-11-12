# 🔥Flexbox

<img src="./assets/images/flexbox.png" alt="flexbox" width="700px">

[🌍 Important Reference ⭐️⭐️⭐️⭐️⭐️](https://css-tricks.com/snippets/css/a-guide-to-flexbox/)

* **Flexbox** is a modern Layout mode in CSS.
* **flex** is a value for the display property.
* Replaces **floats** and is much more elagant to work with.
* Aligns items in both Horizontal(row) and Vertical(column) manner.
* Flex items can be re-ordered via CSS.

<img src="./assets/images/flexbox_view.png" alt="flexbox" width="700px">

## ⚡Flex Container Properties

```css
display: flex;
```

> The element behaves like a block element and lays out its content according to the flexbox model.

[🌍 Reference](https://developer.mozilla.org/en-US/docs/Web/CSS/display)

```css
display: inline-flex;
```

> The element behaves like an inline element and lays out its content according to the flexbox model. It is equivalent to **inline flex**.

[🌍 Reference](https://developer.mozilla.org/en-US/docs/Web/CSS/display)

```css
/* The direction text is laid out in a line */
display: row;

/* The direction in which lines of text are stacked */
flex-direction: column;

/* Like <row>, but reversed */
flex-direction: row-reverse;

/* Like <column>, but reversed */
flex-direction: column-reverse;

/* Global values */
flex-direction: inherit;
flex-direction: initial;
flex-direction: unset;
```

> The flex-direction CSS property sets how flex items are placed in the flex container defining the main axis and the direction (normal or reversed).

[🌍 Reference](https://developer.mozilla.org/en-US/docs/Web/CSS/flex-direction)

```css
flex-wrap: nowrap; /* Default value */
flex-wrap: wrap;
flex-wrap: wrap-reverse;

/* Global values */
flex-wrap: inherit;
flex-wrap: initial;
flex-wrap: unset;
```

> The flex-wrap CSS property sets whether flex items are forced onto one line or can wrap onto multiple lines. If wrapping is allowed, it sets the direction that lines are stacked.

[🌍 Reference](https://developer.mozilla.org/en-US/docs/Web/CSS/flex-wrap)

```css
/* Basic keywords */
align-items: normal;
align-items: stretch;

/* Positional alignment */
/* align-items does not take left and right values */
align-items: center; /* Pack items around the center */
align-items: start; /* Pack items from the start */
align-items: end; /* Pack items from the end */
align-items: flex-start; /* Pack flex items from the start */
align-items: flex-end; /* Pack flex items from the end */

/* Baseline alignment */
align-items: baseline;
align-items: first baseline;
align-items: last baseline; /* Overflow alignment (for positional alignment only) */
align-items: safe center;
align-items: unsafe center;

/* Global values */
align-items: inherit;
align-items: initial;
align-items: unset;
```
> The CSS align-items property sets the align-self value on all direct children as a group. In Flexbox, it controls the alignment of items on the Cross Axis. In Grid Layout, it controls the alignment of items on the Block Axis within their grid area.

[🌍 Reference](https://developer.mozilla.org/en-US/docs/Web/CSS/align-items)

```css
/* Basic positional alignment */
/* align-content does not take left and right values */
align-content: center;     /* Pack items around the center */
align-content: start;      /* Pack items from the start */
align-content: end;        /* Pack items from the end */
align-content: flex-start; /* Pack flex items from the start */
align-content: flex-end;   /* Pack flex items from the end */

/* Normal alignment */
align-content: normal;

/* Baseline alignment */
align-content: baseline;
align-content: first baseline;
align-content: last baseline;

/* Distributed alignment */
align-content: space-between; /* Distribute items evenly
                                 The first item is flush with the start,
                                 the last is flush with the end */
align-content: space-around;  /* Distribute items evenly
                                 Items have a half-size space
                                 on either end */
align-content: space-evenly;  /* Distribute items evenly
                                 Items have equal space around them */
align-content: stretch;       /* Distribute items evenly
                                 Stretch 'auto'-sized items to fit
                                 the container */

/* Overflow alignment */
align-content: safe center;
align-content: unsafe center;

/* Global values */
align-content: inherit;
align-content: initial;
align-content: unset;
```
> The CSS **align-content** property sets the distribution of space between and around content items along a flexbox's cross-axis or a grid's block axis. **aligin-content** depends on **flex-wrap** and cross axis

[🌍 Reference](https://developer.mozilla.org/en-US/docs/Web/CSS/align-content)

## ⚡Flex Item Properties

```css
/* Evenly distribute items */
flex: 1

/* One value, unitless number: flex-grow */
flex: 2;

/* Keyword values */
flex: auto;
flex: initial;
flex: none;

/* One value, width/height: flex-basis */
flex: 10em;
flex: 30%;
flex: min-content;

/* Two values: flex-grow | flex-basis */
flex: 1 30px;

/* Two values: flex-grow | flex-shrink */
flex: 2 2;

/* Three values: flex-grow | flex-shrink | flex-basis */
flex: 2 2 10%;

/* Global values */
flex: inherit;
flex: initial;
flex: unset;
```
> The flex CSS shorthand property sets how a flex item will grow or shrink to fit the space available in its flex container.

[🌍 Reference](https://developer.mozilla.org/en-US/docs/Web/CSS/flex)

```css
/* <integer> values */
order: 5;
order: -5;

/* Global values */
order: inherit;
order: initial;
order: unset;
```
> The order CSS property sets the order to layout an item in a flex or grid container. Items in a container are sorted by ascending order value and then by their source code order.

[🌍 Reference](https://developer.mozilla.org/en-US/docs/Web/CSS/order)

```css
/* Positional alignment */
justify-content: center;     /* Pack items around the center */
justify-content: start;      /* Pack items from the start */
justify-content: end;        /* Pack items from the end */
justify-content: flex-start; /* Pack flex items from the start */
justify-content: flex-end;   /* Pack flex items from the end */
justify-content: left;       /* Pack items from the left */
justify-content: right;      /* Pack items from the right */

/* Baseline alignment */
/* justify-content does not take baseline values */

/* Normal alignment */
justify-content: normal;

/* Distributed alignment */
justify-content: space-between; /* Distribute items evenly
                                   The first item is flush with the start,
                                   the last is flush with the end */
justify-content: space-around;  /* Distribute items evenly
                                   Items have a half-size space
                                   on either end */
justify-content: space-evenly;  /* Distribute items evenly
                                   Items have equal space around them */
justify-content: stretch;       /* Distribute items evenly
                                   Stretch 'auto'-sized items to fit
                                   the container */

/* Overflow alignment */
justify-content: safe center;
justify-content: unsafe center;

/* Global values */
justify-content: inherit;
justify-content: initial;
justify-content: unset;
```
> The CSS justify-content property defines how the browser distributes space between and around content items along the main-axis of a flex container, and the inline axis of a grid container.

[🌍 Reference](https://developer.mozilla.org/en-US/docs/Web/CSS/justify-content)

```css
/* Keyword values */
align-self: auto;
align-self: normal;

/* Positional alignment */
/* align-self does not take left and right values */
align-self: center; /* Put the item around the center */
align-self: start; /* Put the item at the start */
align-self: end; /* Put the item at the end */
align-self: self-start; /* Align the item flush at the start */
align-self: self-end; /* Align the item flush at the end */
align-self: flex-start; /* Put the flex item at the start */
align-self: flex-end; /* Put the flex item at the end */

/* Baseline alignment */
align-self: baseline;
align-self: first baseline;
align-self: last baseline;
align-self: stretch; /* Stretch 'auto'-sized items to fit the container */

/* Overflow alignment */
align-self: safe center;
align-self: unsafe center;

/* Global values */
align-self: inherit;
align-self: initial;
align-self: unset;
```
> The align-self CSS property overrides a grid or flex item's align-items value. In Grid, it aligns the item inside the grid area. In Flexbox, it aligns the item on the cross axis.

[🌍 Reference](https://developer.mozilla.org/en-US/docs/Web/CSS/align-self)
