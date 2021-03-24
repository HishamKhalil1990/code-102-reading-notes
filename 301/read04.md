# CSS GRID
### Grid is a two-dimensional grid-based layout system. aims to design page based on a grid-based user interfaces. most browsers either shipped native or unprefixed supporting the CSS Grid.
### For basic terminology, Grid consists of 6 parts:
1. Grid container
    - it is the element on which `display: grid` is applied and contains the Grid items
2. Grid item
    -it is the direct child of the Grid container
3. Grid line
    - it is the dividing line that make up the structure of the Grid horizantally or vertically
4. Grid cell
    - it is the space between two adjacent rows and two adjacent columns Grid lines
5. Grid track
    - it is the space space between two adjacent Grid lines
6. Grid area
    - it is the total space surrounded by four grid lines
### some of parent properties:
- `display: grid | inline-grid;`
- `grid-template-columns: 40px 50px auto 50px 40px;`
- `grid-template-rows: 25% 100px auto;`
- `grid-area: header;`
- `grid-template: none | <grid-template-rows> / <grid-template-columns>;`
- `column-gap: <line-size>;`
- `grid-row-gap: <line-size>;`
- `justify-items: start;`
- `align-content: start; `
- `grid-auto-flow: row | column | row dense | column dense;`
### some of children properties:
- `grid-column-start: 2;`
- `grid-row-start:2`
- `grid-column: 3 / span 2;`
- `grid-row: third-line / 4;`
- `grid-area: header;`
- `justify-self: start;`
- `align-self: end;`
- `place-self: center stretch;`
### Using fluid width columns which break Grid into more or less columns as space is available the contents distribution can be controlled to get a good shape
### Grids are a good solution to animate arranged contents without affecting the contents places in the page layout