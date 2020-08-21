# CSS Displays

This repo contains simple exmples of the following css displays:
 - float
 - flexbox
 - grid

To view each, uncomment out to corresponding `<link>` line in the html file. 

## Float
Places an element on the left or right side of its container, allowing text and inline elements to wrap around it. Use when working with just one or a few elements within a container. 

Use the [clear](https://developer.mozilla.org/en-US/docs/Web/CSS/clear) property to "reset" the document (i.e. allow proceeding elements to be placed under the floated items).

[DOCS](https://developer.mozilla.org/en-US/docs/Web/CSS/float)

[CODEPEN EXAMPLE](https://codepen.io/tim-corley/pen/QWNKWrR)


## Flexbox
A one-dimensional layout method for laying out items in rows or columns. Items flex to fill additional space and shrink to fit into smaller spaces.

Define flex (`display: flex;`) on the parent container and all child elements will automatically become flex items. If using `inline-flex` on container element it sets the width to the contents (i.e. flex items).

 - use `flex-direction` property to determine ordering of content

 - use `flex-wrap` property to wrap items to new row

flex can be used to control:
- alignment
- direction
- order
- size

aligning items in a flex container:
- **justify-content**: aligns items on the main axis
- **align-items**: aligns items on the cross axis

```css
.box {
  /* place items in center of container*/
  display: flex;
  align-items: center;
  justify-content: center;
}
```

[DOCS](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Flexible_Box_Layout)

[CODEPEN EXAMPLE](https://codepen.io/tim-corley/pen/vYGXYQj)

## Grid

Used to divide a page into major regions or to define the relationship in terms of size, position, and layer, between parts of a control built from HTML primitives. A grid layout enables an author to align elements into columns and rows.

**explicit grid**

use: `grid-template-columns` & `grid-template-rows`

```css
/*creates a grid with 3 columns & 2 rows*/
.grid-container {
  display: grid;
  grid-template-columns: 100px 100px 100px;
  grid-template-rows: 100px 100px;
}
```

can use `fr` as unit within the grid-template values, represents the fraction of available space in the grid container.

```css
grid-template-columns: 1fr 2fr 1fr;
/*use repeat*/
grid-template-columns: 50px repeat(2, 1fr);
```

**implicit grid**

use implicit grid when working with dynamic / unknown data

`grid-auto-rows` & `grid-auto-columns`

add **gutters** (space between grids) with `gap`

```css
gap: 10px;
/* set gutter for rows then columns*/
gap: 10px 20px;
```

[DOCS](https://developer.mozilla.org/en-US/docs/Web/CSS/CSS_Grid_Layout)

[CODEPEN EXAMPLE](https://codepen.io/tim-corley/pen/RwaGwEJ)

---

more css layout examples: https://codepen.io/collection/AQkgKB?grid_type=list

# CSS Animations 

## Tools

 - [cubic-bezier](https://cubic-bezier.com/#.17,.67,.83,.67)
 - [easings](https://easings.net/)
 - [bounceJS](http://bouncejs.com/)
 - [svg-omg](https://jakearchibald.github.io/svgomg/)
 - [greensock](https://greensock.com/)
 - [snap.svg](http://snapsvg.io/)
 - [codepen](https://codepen.io/)