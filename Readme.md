# Vite + React + Tailwind Template Project

This is a template repository to make spinning up a new app using Vite/React/Tailwind faster. 

## Usage
1. Create project based on template.
2. `npm install` from project base directory.
3. Enjoy.

## Create the Project
```console
npm create vite@latest project-name-here -- --template react
```

## Install Tailwind
https://tailwindcss.com/docs/guides/vite

1. Install Tailwind and create the tailwind config files:
```console
npm install -D tailwindcss postcss autoprefixer
npx tailwindcss init -p 
```

2. Update the tailwind.config.js file:
```javascript
/** @type {import('tailwindcss').Config} */
export default {
  content: [
    "./index.html",
    "./src/**/*.{js,ts,jsx,tsx}",
  ],
  theme: {
    extend: {},
  },
  plugins: [],
}
```

3. Update `src/index.css`:
```css
@tailwind base;
@tailwind components;
@tailwind utilities;
```

4. Rebuild and run the project:
```console
npm run dev 
```