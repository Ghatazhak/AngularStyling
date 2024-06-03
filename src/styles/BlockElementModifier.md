# BEM Quick Start Guide

This guide provides a quick introduction to using the BEM (Block Element Modifier) methodology for naming CSS classes. BEM helps in creating reusable components and code sharing in front-end development.

## BEM Methodology

1. **Block**: The outermost parent component. Standalone entity that is meaningful on its own.
2. **Element**: A part of the block that performs a certain function. Elements are semantically tied to their block.
3. **Modifier**: A flag on a block or element that changes its look or behavior. Modifiers are independent of the block or element and can be used in different contexts.

## BEM Naming Convention

- Block: `.block-name`
- Element: `.block-name__element-name`
- Modifier: `.block-name--modifier-name` or `.block-name__element-name--modifier-name`

## Example: Card Component

### HTML Structure

```html
<div class="card card--featured">
  <div class="card__header">
    <h2 class="card__title">Card Title</h2>
  </div>
  <div class="card__body">
    <p class="card__text">This is some card text. It provides additional information about the card.</p>
  </div>
  <div class="card__footer">
    <button class="card__button card__button--primary">Read More</button>
  </div>
</div>
```
### CSS Styles

```scss
/* Block component */
.card {
  border: 1px solid #ccc;
  border-radius: 4px;
  padding: 16px;
  background-color: #fff;

  /* Modifier for the block */
  &--featured {
    border-color: #f39c12;
  }

  /* Element inside the block */
  &__header {
    border-bottom: 1px solid #ccc;
    padding-bottom: 8px;
    margin-bottom: 16px;
  }

  &__title {
    font-size: 1.5em;
    margin: 0;
  }

  &__body {
    padding: 16px 0;
  }

  &__text {
    margin: 0;
    font-size: 1em;
    color: #333;
  }

  &__footer {
    border-top: 1px solid #ccc;
    padding-top: 8px;
    margin-top: 16px;
    text-align: right;
  }

  /* Element inside the block with modifier */
  &__button {
    padding: 8px 16px;
    font-size: 1em;
    border: none;
    border-radius: 4px;
    cursor: pointer;

    &--primary {
      background-color: #3498db;
      color: #fff;
    }
  }
}
```
