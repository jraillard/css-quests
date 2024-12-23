# Grid memo

- `grid mode` &rarr; apply to parent div / container to manage sub items as a grid (two dimensions row **AND** column)
```css
 display: grid;
```

- `grid-column-start` property in order to ***define specific grid item start position within grid columns*** with an integer starting from 1 to columns + 1

- `grid-column-end` property in order to ***define specific grid item end position within grid columns*** with an integer as value starting from 1 to columns + 1. It can be inferior to the start value.
  

- `grid-row-start` property in order to ***define specific grid item start position within grid rows*** with an integer starting from 1 to rows + 1

- `grid-row-end` property in order to ***define specific grid item end position within grid rows*** with an integer as value starting from 1 to rows + 1. It can be inferior to the start value.
 
:bulb: See following display for visuals : 
![grid indexes](/games/gridgarden/grid-indexes.png)

- `span` on `grid-column-end` can be used in order to ***define the column width instead of grid lines positions***

&rarr; For instance the next would create a space with column 2 and three (ie index 2 to 4): 
```css
 grid-column-start: 2;
 grid-column-end: span 2;
```

:bulb: If span is on grid-column-start, grid-column-end would be ignored as it would result in span starting from index 1

- `span` could also works on `grid-row-[start |end]` **the same way but for rows**

- `grid-column` property in order to ***combine both grid-column-start and grid-column-end*** with both values separated by a slash.

```css
  grid-column: gridColumnStartValue / gridColumnEndValue;
```

- `grid-row` property in order to ***combine both grid-row-start and grid-row-end*** with both values separated by a slash.

```css
  grid-row: gridRowStartValue / gridRowEndValue;
```

- `grid-area` property in order to **combine both grid-row and grid-column** into one single property.

```css
  grid-area: gridRowStartValue / gridColumnStartValue / gridRowEndValue / gridColumnEndValue;
```

- `order` property in order to **override item order** with an integer. Default value is 0 for all items.

- `repeat` function `grid-template-columns` for property in order to **simplify identical widths definition**.

:bulb: Also works with `grid-template-rows` & `grid template`

- `grid-template` property in order to **combine both grid-template-rows and grid-template-columns values** 

```css
    grid-template: gridTemplateRowsValue / gridTemplateColumnsValue
``` 