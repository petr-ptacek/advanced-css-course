# Notes - Natours

## Look at

- `clip-path`
- `backface-visibility`
- `animation`
- `background-clip`
- `perspective`
- `background-blend-mode`
- `box-decoration-break`
- `shape-outside`

### `text-shadow` [link](https://developer.mozilla.org/en-US/docs/Web/CSS/text-shadow)

- Each shadow is described by some combination of X and Y offsets from the element, blur radius, and color.

```css
.text {
  text-shadow: 4px 4px 5px rgba(0, 0, 0, 0);
}
```

### `box-shadow` [link](https://developer.mozilla.org/en-US/docs/Web/CSS/box-shadow)

- A box shadow is described by X and Y offsets relative to the element, blur and spread radius, and color.

```css
.box {
  box-shadow: 5px 5px 4px 3px rgba(0, 0, 0, 0);
}
```

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

### Tip: Architecture of Files

- **base/**
- **components/**
- **layouts/**
- **pages/**
- **themes/**
- **abstracts/**
- **vendors/**

## Sass Features

- **variables:** for reusable values such as colors, font-sizes, spacing, etc
- **nesting:** to nest selectors inside of one another, allowing us to write less code
- **operators:** for mathematical operations right inside of CSS
- **partials and imports:** to write CSS in different files and importing them all into one single file
- **mixins:** to write reusable pieces of CSS code
- **functions:** similar to mixins, with the difference that they produce a value that can be used
- **extends:** to make different selectors inherit declarations that are common to all of them
- **control directives:** for writing complex code using conditionals and loops

## [Sass](https://sass-lang.com/)

- _Syntactically Awesome Stylesheet_

```shell
npm install sass -D
```

```shell
sass <input.scss> [output.css]
sass <input.scss>:<output.css>
```

### Input and Output

- `-s, --style`
  - Output style. [expanded (default), compressed]
- `--[no-]source-map`
- `-w --watch`
  - Watch stylesheets and recompile when they change.
- `--update`
  - Sass will only compile stylesheets whose dependencies have been modified more recently than the corresponding CSS
    file was generated. It will also print status messages when updating stylesheets.
- `--color`
  - his flag (abbreviated -c) tells Sass to emit terminal colors, and the inverse --no-color tells it not to emit
    colors. By default, it will emit colors if it looks like it’s being run on a terminal that supports them.
