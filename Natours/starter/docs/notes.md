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

### Tip: Architecture

- base/
- components/
- layouts/
- pages/
- themes/
- abstracts/
- vendors/

## Sass Features

- **variables:** for reusable values such as colors, font-sizes, spacing, etc
- **nesting:** to nest selectors inside of one another, allowing us to write less code
- **operators:** for mathematical operations right inside of CSS
- **partials and imports:** to write CSS in different files and importing them all into one single file
- **mixins:** to write reusable pieces of CSS code
- **functions:** similar to mixins, with the difference that they produce a value that can be used
- **extends:** to make different selectors inherit declarations that are common to all of them
- **control directives:** for writing complex code using conditionals and loops

## Npm Sass
```shell
npm install sass -D
```

```shell
sass <input.scss> [output.css]
sass <input.scss>:<output.css>
```

### Input and Output
- -s, --style
  - Output style. [expanded (default), compressed]
- --[no-]source-map
- -w --watch
  - Watch stylesheets and recompile when they change.

