# main.scss

The `main.scss` file serves as the central point for importing and forwarding all your individual style folders. This file should not contain any actual styles; instead, it should use the `@forward` rule to gather all the necessary styles from the different parts of your project.

## Usage

1. **@forward**: Use `@forward` to forward all the styles from each of the individual style folders. This ensures that the styles are properly namespaced and can be used throughout the project.

## Example

```scss
// Forwarding styles from individual folders
@forward 'abstracts';
@forward 'base';
@forward 'elements';
@forward 'layout';

// Optionally, if you have additional folders like components or themes
// @forward 'components';
// @forward 'themes';
