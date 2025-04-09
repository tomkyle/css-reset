# tomkyle-styles

Opionated CSS reset based on Josh W Comeau's [CSS Reset](https://www.joshwcomeau.com/css/custom-css-reset/), 
some of Andy Bell's [CSS rules](https://piccalil.li/blog/a-more-modern-css-reset/),
and Jen Simmons' [CSS Remedy](https://github.com/jensimmons/cssremedy/).

## Installation

```bash
npm install @tomkylenet/css-reset
```

## Opinionated Typography

- Default font is `system-ui` with fallback to whatever your browser considers `sans-serif`.
- Font size will grow from `1em` to `1.25em`, depending on screensize.
- Line height depends on font size *plus* a fixed `0.5rem` lead: The larger the font, the tighter its line height.

With these defaults, your page will appear pleasantly familiar. They are written as CSS short-hand rule on `html` element, so you can override them easily using `font-size`, `line-height`, and `font-family`.

## Adaptive list spacing

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





