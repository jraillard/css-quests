# Flexbox memo

- `flex mode` &rarr; apply it to parent div / container to manage sub items as one dimension (row **OR** column)
```css
display: flex;
```

- `justify-content` property in order to ***align items horizontally*** with several values : 
  - `flex-start`: Items align to the left side of the container.
  - `flex-end`: Items align to the right side of the container.
  - `center`: Items align at the center of the container.
  - `space-between`: Items display with equal spacing between them.
  - `space-around`: Items display with equal spacing around them.

- `align-items` property in order to ***align items vertically*** with several values : 
  - `flex-start`: Items align to the top of the container.
  - `flex-end`: Items align to the bottom of the container.
  - `center`: Items align at the vertical center of the container.
  - `baseline`: Items display at the baseline of the container.
  - `stretch`: Items are stretched to fit the container.
  
- `flex-direction` property in order to ***handle items order / direction*** with several values : 
  - `row`: Items are placed the same as the text direction.
  - `row-reverse`: Items are placed opposite to the text direction.
  - `column`: Items are placed top to bottom.
  - `column-reverse`: Items are placed bottom to top.

- `order` property in order to ***apply individual order to one element***. Values can be both negative and positive integers. Default value is 0.

- `align-self` property in order to ***align only one item vertically*** with same values as `align-items` : 
  - `flex-start`: Item align to the top of the container.
  - `flex-end`: Item align to the bottom of the container.
  - `center`: Item align at the vertical center of the container.
  - `baseline`: Item display at the baseline of the container.
  - `stretch`: Item are stretched to fit the container.

- `flex-wrap` property in order to **force items on a single line or wrap them in multiples** with several values : 
  - `nowrap`: Every item is fit to a single line.
  - `wrap`: Items wrap around to additional lines.
  - `wrap-reverse`: Items wrap around to additional lines in reverse.

- `flex-flow` property in order to **combine flex-direction and flex-wrap into one single property**.

```css
flex-flow: flexDirectionValue flexWrapValue
```

- `align-content` property in order to **managed space between multiple lines** with several values : 
  - `flex-start`: Lines are packed at the top of the container.
  - `flex-end`: Lines are packed at the bottom of the container.
  - `center`: Lines are packed at the vertical center of the container.
  - `space-between`: Lines display with equal spacing between them.
  - `space-around`: Lines display with equal spacing around them.
  - `stretch`: Lines are stretched to fit the container.

    :warning: Not to confuse with `align-items` that allow **line(s)** alignment. Meaning `align-content` as no effect with only one line of content where `align-items` because it treat items as a whole.

    :bulb: If there's for instance 3 lines and we apply align-items: center; then all the three lines would be centered vertically to the container. align-content: center; will cause three lines to be packed and then centered.

- `place-content` property in order to **combine justify-content and align-content into one single property**.

```css
place-content: justifyContentValue alignContentValue
```

# Tips & Tricks

:one: Managing items whether in rows or column switch also the meaning of horizontal & vertical (ie need of using whether justify-content or align-items)

:two: Managing items whether in right or revert over switch also the meaning of flex-start and flex-end.