# Level 21 : align-content

Introducing the `align-content` property in order to **managed space between multiple lines** with several values : 
- `flex-start`: Lines are packed at the top of the container.
- `flex-end`: Lines are packed at the bottom of the container.
- `center`: Lines are packed at the vertical center of the container.
- `space-between`: Lines display with equal spacing between them.
- `space-around`: Lines display with equal spacing around them.
- `stretch`: Lines are stretched to fit the container.

:warning: Not to confuse with `align-items` that allow **line(s)** alignment. Meaning `align-content` as no effect with only one line of content where `align-items` because it treat items as a whole.

:bulb: If there's for instance 3 lines and we apply align-items: center; then all the three lines would be centered vertically to the container. align-content: center; will cause three lines to be packed and then centered.

# Exercise

:clipboard: 15 green frogs already wraped in 3 lines. Their lilypad are on top of the container.

:bulb: Basically just apply : 

```css
flex-wrap: wrap;
align-content: flex-start;
```
