# Abstracts

The `abstracts` folder contains all Sass tools and helpers that are used throughout the project. These files do not generate any CSS directly but provide utilities for other styles.

## Contents

- **_variables.scss**: Define project-wide variables such as colors, font-sizes, etc.
- **_mixins.scss**: Include mixins for reusable pieces of code.
- **_functions.scss**: Define custom functions for use within your stylesheets.
- **_placeholders.scss**: Include placeholders for extending selectors without generating additional CSS.
- **_index.scss**: Use `@forward` to forward all files in this folder.

Ensure that all files in this folder are forward only and do not output any CSS on their own.
