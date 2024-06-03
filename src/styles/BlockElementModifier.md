# BEM Quick Start Guide

This guide provides a quick introduction to using the BEM (Block Element Modifier) methodology for naming CSS classes. BEM helps in creating reusable components and code sharing in front-end development.

## BEM Methodology

1. **Block**: The outermost parent component.
2. **Element**: A part of the block that performs a certain function.
3. **Modifier**: A flag on a block or element that changes its look or behavior.

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
