# tomkyle-styles

**Opionated CSS reset based on Josh W Comeau's [Modern CSS Reset](https://www.joshwcomeau.com/css/custom-css-reset/), some of Andy Bell's [(More) Modern CSS Reset](https://piccalil.li/blog/a-more-modern-css-reset/), and Jen Simmons' [CSS Remedy](https://github.com/jensimmons/cssremedy/).**

## Installation

The asiest way is to just copy the contents of [dist/reset.css](./dist/reset.css). If you like to install it as dependency, install using NPM:

```bash
npm install @tomkylenet/css-reset
```

## Opinionated Features

### Dark mode support

My CSS reset introduces `dark` and `light` mode, unless configured in using `<meta name="color-scheme" content="light dark">`

### Typography

- Default font is `system-ui` with fallback to whatever your browser considers `sans-serif`.
- Font size will grow from `1em` to `1.25em`, depending on screensize.
- Line height depends on font size *plus* a fixed `0.5rem` lead: The larger the font, the tighter its line height.

With these defaults, your page will appear pleasantly familiar. They are written as CSS short-hand rule on `html` element, so you can override them easily using `font-size`, `line-height`, and `font-family`.

### List spacing

Compact list indentation on smaller screens grows with screen size from `1.4em` up to `2.5rem`, near the tradtionally hard-coded `40px` value.

## Development

This project uses [PostCSS](https://postcss.org/) with [Autoprefixer](https://github.com/postcss/autoprefixer) to process CSS files. The Development workflow:

1. Make changes to files in the `css/` directory
2. Run the watch script to automatically process changes.

```bash
npm run watch
````

Built files will go into `dist/` directory. To trigger a build:

```bash
npm run build
````





