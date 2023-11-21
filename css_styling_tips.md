# CSS STYLING

## How to Center Text Vertically with CSS

### STEP: 1 (To Center Text using Line Height)

This approach is limited, but can be useful if you have your element set to a fixed height using the height property.

If you set the element's height and line-height to the same value, the text will be vertically centered:

```html
<div class="my-element">hello world</div>
```

```css
.my-element {
  height: 3rem;
  line-height: 3rem;
}
```

output
![outpu](./notes_img/image-91.png)

#### Notes:

There is an important caveat to this approach, though. This only works if your text can fit on one line.

If the text does wrap, you'll see the first line vertically centered. Because you set the line-height to be the same as the element's height, the wrapped line of text now overflows the element.
![](./notes_img/image-94.png)

### STEP: 2 (To Center Text using Flexbox)

A better, more general-purpose solution, is to use a Flexbox layout with align-items set to center.

```html
<div class="my-element">hello world</div>
```

```css
.my-element {
  display: flex;
  flex-direction: row;
  align-items: center;
}
```

output
![](./notes_img/image-96.png)

### STEP: 3 (To Center Text using CSS Grid)

For a single div containing the text to center, you can turn it into a grid layout with one row and one column.

```css
.my-element {
  display: flex;
  flex-direction: row;
  align-items: center;
}
```

output
![](./notes_img/image-98.png)

#### Notes:

Text vertically centered using a 1x1 grid layout

