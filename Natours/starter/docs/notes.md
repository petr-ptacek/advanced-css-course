# Notes - Natours

## Look at

- `clip-path`
- `backface-visibility`
- `animation`

## CSS Specificity

1) Inline styles
2) IDs
3) Classes, pseudo-classes, attribute
4) Elements, pseudo-elements

- A selector that contains 1 ID is more specific than one with 1000 classes
- A selector that contains 1 class is more specific than one with 1000 elements
- The universal selector `*` has no specificity value `(0,0,0,0)`

### Tip: Specify the `box sizing`
```css
*,
*::before,
*::after {
  margin: 0;
  padding: 0;
  box-sizing: inherit;
}

body {
  box-sizing: border-box;
}

```