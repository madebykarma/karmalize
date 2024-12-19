# @madebykarma/karmalize

`@madebykarma/karmalize` is a refined CSS baseline built on top of [`modern-normalize`](https://github.com/sindresorhus/modern-normalize).  It ensures consistent typography, smoother cross-browser rendering, and a reliable starting point for establishing a unified design system.

## Differences from `modern-normalize`

- Uses a base `font-size: 16px;` and `line-height: 1.5;` for improved readability.
- More broadly inherits `color`, `font-family`, and other typographic properties for cohesive branding.
- Extends resets for elements like `hr`, `abbr`, `fieldset`, and `legend`, offering a more comprehensive baseline.

## Installation

Use `npm`:

```sh
npm install @madebykarma/karmalize
```

or `yarn`:

```sh
yarn add @madebykarma/karmalize
```

## Usage

Import it in your main stylesheet:

```css
@import "@madebykarma/karmalize";
```

### Next.js (App Router) Example:

```jsx
// app/layout.js
import "@madebykarma/karmalize";

export default function RootLayout({ children }) {
  return (
    <html lang="en">
      <body>{children}</body>
    </html>
  );
}
```

### Astro Example:

```astro
---
import "@madebykarma/karmalize";
---

<html lang="en">
  <body>
    <h1>Hello, Astro!</h1>
  </body>
</html>
```
