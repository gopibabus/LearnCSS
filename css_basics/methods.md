# 🔥CSS Methodologies

Following are popular Methodologies for organizing CSS:

1. BEM
2. SMACSS
3. CSS Modules
4. Styled Components

## BEM(Block, Element, Modifier)

The Block, Element, Modifier methodology (commonly referred to as BEM) is a popular naming convention for classes in HTML and CSS. Developed by the team at Yandex, its goal is to help developers better understand the relationship between the HTML and CSS in a given project.

```css
/* Block component */
.btn {}

/* Element that depends upon the block */
.btn__price {}

/* Modifier that changes the style of the block */
.btn--orange {}
.btn--big {}
```

[🌍 Tutorial Reference](https://css-tricks.com/bem-101/)

[🌍 Official Website](http://getbem.com/naming/)

[🌍 Official Website2](https://en.bem.info/)

## SMACSS (Scalable and Modular Architecture for CSS)

At the very core of SMACSS is categorization. By categorizing CSS rules, we begin to see patterns and can define better practices around each of these patterns.

There are five types of categories:
* Base
* Layout
* Module
* State
* Theme

**Base rules** are the defaults. They are almost exclusively single element selectors but it could include attribute selectors, pseudo-class selectors, child selectors or sibling selectors. Essentially, a base style says that wherever this element is on the page, it should look like this.

* _base.scss
* _mixin.scss
* _normalize.scss
* _variables.scss

**Layout rules** divide the page into sections. Layouts hold one or more modules together.

* __header.scss
* __nav.scss
* __sitebar.scss
* __footer.scss
* ___section.scss

**Modules** are the reusable, modular parts of our design. They are the callouts, the sidebar sections, the product lists and so on.

* ___blocks.scss
* ___buttons.scss
* ___componentes.scss
* ___typography.scss

**State rules** are ways to describe how our modules or layouts will look when in a particular state. Is it hidden or expanded? Is it active or inactive? They are about describing how a module or layout looks on screens that are smaller or bigger. They are also about describing how a module might look in different views like the home page or the inside page.

**Theme rules** are similar to state rules in that they describe how modules or layouts might look. Most sites don’t require a layer of theming but it is good to be aware of it.

[🌍 Reference](https://medium.com/oceanize-geeks/scalable-modular-architecture-for-css-2d7c6c6ffdcd)

[🌍 Official Website](http://smacss.com/)

## CSS Modules

> **CSS modules are CSS files** in which all class names and animation names are scoped locally by default. CSS Modules is not an official spec or an implementation in the browser but rather a process in a build step (with the help of Webpack or Browserify) that changes class names and selectors to be scoped (i.e. kinda like namespaced).

?> Instead of writing plain HTML, we need to write all of our markup in a JavaScript file, like **index.js**.

```css
import styles from "./styles.css";

element.innerHTML =
  `<h1 class="${styles.title}">
     An example heading
   </h1>`;
```

Generated HTML:

```html
<h1 class="_styles__title_309571057">
  An example heading
</h1>
```

[🌍 Reference](https://css-tricks.com/css-modules-part-1-need/)

[🌍 Offical Website](https://github.com/css-modules/css-modules)

## Styled Components

> **Styled components** are a **CSS-in-JS tool** that bridges the gap between components and styling, offering numerous features to get you up and running in styling components in a functional and reusable way.

Styled components include the following features:
* Automatic vendor prefixing
* Unique class names
* Elimination of dead styles

```js
import styled from "styled-components";

// Styled component named StyledButton
const StyledButton = styled.button`
  background-color: black;
  font-size: 32px;
  color: white;
`;

function Component() {
  // Use it like any other component.
  return <StyledButton> Login </StyledButton>;
}
```

[🌍 Official Website](https://styled-components.com/)

[🌍 Reference](https://www.smashingmagazine.com/2020/07/styled-components-react/)

[🌍 Using styled-components alongside css-modules](https://medium.com/@baphemot/using-styled-components-alongside-css-modules-4d83b378bc17)
