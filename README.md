# Vite + React + TypeScript + Tailwind CSS + DaisyUI

## Project Setup

- Create Project using Vite + React + TypeScript: `npm create vite@latest`
- Install Tailwind CSS and plugins: follow the [instruction](https://tailwindcss.com/docs/installation) to install it.
- Install `prettier` and the Tailwind CSS formatter plugin: `npm install -D prettier prettier-plugin-tailwindcss`.
  Example of the configuration of `prettier`:

```json
{
  "semi": false,
  "singleQuote": true,
  "jsxSingleQuote": true,
  "trailingComma": "all",
  "tabWidth": 2,
  "printWidth": 80,
  "plugins": ["prettier-plugin-tailwindcss"]
}
```

- Add DaisyUI: `npm i -D daisyui@latest` and set it up in the `tailwind.config.js` file.

```javascript
import daisyui from 'daisyui'

/** @type {import('tailwindcss').Config} */
export default {
  content: ['./index.html', './src/**/*.{js,ts,jsx,tsx}'],
  theme: {
    extend: {},
  },
  plugins: [daisyui],
}
```
