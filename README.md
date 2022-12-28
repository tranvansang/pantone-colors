# Pantone color palette

## Usage

- NPM package name: `pantone-colors`.
- Default export: `{[colorId]: colorInRGB}`.
- Named export: `export const isDark {[colorId]: boolean}`.

## Sample usage with Tailwind

In `tailwind.config.js`:

```js
const pantoneColors = require('pantone-colors').default
// or import pantoneColors from 'pantone-colors'

module.exports = {
	theme: {
		extend: {
			colors: {
				pantone: pantoneColors
			},
		}
	},
}
```

In code: `bg-pantone-290`, `text-pantone-500`, etc.
