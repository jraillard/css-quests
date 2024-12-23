# CSS units memo 

- `px` : hardcoded pixel value

&rarr; Usage = Should **only** be used for elements that will not be resized depending on screen size. **Majorly used for font sizing**.

- `em` : pixels ratio relative to parent element font size

&rarr; Usage = Need to scale element based on parent element (whether it's size is). **Majorly used for font sizing**.

- `rem` : same as EM but relative to root element (top div for instance)

&rarr; Usage = Use it first and then EM for more granularity. **Majorly used for font sizing**.

:bulb: For instance, default font size is 16px. Then 1em would equals = 16px (1*16), 2em = 32px, .5em = 8px, etc.

- `vw` : relative to viewport width

&rarr; Usage = Margins, padding, spacing, width / heights.

- `vh` : relative to viewport height

&rarr; Usage = Usage = Margins, padding, spacing, width / heights.

:bulb: For instance with a mobile device (480px x 800px): 1VW = 1% of viewport width = 4.8px.

- `%` : similar to VW & VH but relative on parent element not viewport width / heigth

&rarr; Usage = Usage = Margins, padding, spacing, width / heights.

-  `fr` : allocates one share of the available space

&rarr; Means that if two elements are set to **1fr** and **3fr** respectively, the space is divided into 4 equals shares; the first element occupies 1/4 and the second element 3/4 of any leftover space.

# Tips and tricks

:one: If two elements are set to **0fr** et one to **1fr**, only the last will be displayed but you're still having three elements (such as rows) : 

```css
    /* Here we define 3 rows but only the third content will be displayed taking the space a the three one */
    grid-templates-rows: 0fr 0fr 1fr;
```

See this [sample](/games/gridgarden/level26.md) for a basic usage.
