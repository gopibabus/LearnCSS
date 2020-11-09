# 🔥CSS Methodologies

?> A lot of the ideas that are presented in the following are modular ways to organize your CSS, with variations on how to approach and name your classes.

Following are popular Methodologies for organizing CSS:

1. BEM
2. SMACSS
3. Cube CSS
4. OOCSS
5. Atomic CSS
6. CSS Modules
7. Styled Components

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

## Cube CSS (Composition Utility Block)

> **CUBE CSS** takes most of its inspiration from **BEM**. Core of BEM is blocks, whereas with CUBE CSS, the core is CSS.

* **Composition**: These are classes which define the foundational layout, the content skeleton if you will. I imagine this being your grid and flexbox classes.
* **Utility**: Largely these are just utility classes (.wrapper, .inline, .centre etc.). They do "one thing, and do it well". Makes sense. Not sure I'm a fan of the use of colours as utility glasses; I'd rather use variables for that. In fact, personally I feel like CSS variables are a form of utility class, so would group those two together.
* **Block**: Pretty much how it is in BEM, a block == a component. Ideally you have very little of these; how you specifically deal with sub-rules is up to you.
* **Exception**: Exceptions make use of data-attributes. I like that a lot. They let you manipulate blocks, reversing card order (for example) or highlighting a specific card, and they don't leave you fighting the cascade too much.

[🌍 Official Website](https://piccalil.li/blog/cube-css/)

## OOCSS (Object Oriented CSS)

> Repeating patterns in your stylesheets lend themselves to the creation of objects which can be sub-typed or super-typed. These patterns can be polymorphic, thus infinitely reusable through inheritance. In a nutshell - object oriented.

[🌍 Reference](https://anotheruiguy.gitbooks.io/sassintherealworld_book-i/content/rules-to-live-by/oocss.html)

## Atomic CSS

> Atomic CSS is for developers who see the benefits of styling "outside of style sheets" — who want to write markup and styles in one place while benefiting from a Atomic architecture. It is a switch of priorities. You don't maintain style sheets but components. Atomic CSS can live side-by-side with traditional style sheets. In cases where Atomic CSS doesn't seem the most pragmatic, you can always supplement with inline styles or external stylesheets. Use the right tool for the job.

?> **Example**: Tailwind CSS

[🌍 Official Website]([link](https://acss.io))

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
