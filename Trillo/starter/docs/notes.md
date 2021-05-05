## Look at

### `box-shadow`

```shell
box-shadow: [horizontal offset] [vertical offset] [blur radius] [optional spread radius] [color];
```

- One-Side Only
  - Using a negative spread radius, you can get squeeze in a box shadow and only push it off one edge of a box
  ```css
    .one-edge-shadow {
      box-shadow: 0 8px 6px -6px black;
    }
  ```

### `currentColor`

- A CSS value that will apply the existing `color` value to other properties like `background-color`

```css
div {
  color: red;
  border: 5px solid currentColor;
  box-shadow: 0 0 5px currentColor;
  /** Everything will be black */
}
```

### `mask` [link](https://developer.mozilla.org/en-US/docs/Web/CSS/mask)

- hides an element (partially or fully) by masking or clipping the image at specific points
- **Constituent properties**
  - `mask-clip`
  - `mask-composite`
  - `mask-image`
  - `mask-mode`
  - `mask-origin`
  - `mask-repeat`
  - `mask-size`

## SVG Icons

- [IcoMoon](https://icomoon.io/)