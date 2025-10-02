# React + TypeScript + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react) uses [Babel](https://babeljs.io/) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh

## React Compiler

The React Compiler is not enabled on this template because of its impact on dev & build performances. To add it, see [this documentation](https://react.dev/learn/react-compiler/installation).

## Expanding the ESLint configuration

If you are developing a production application, we recommend updating the configuration to enable type-aware lint rules:

```js
export default defineConfig([
  globalIgnores(['dist']),
  {
    files: ['**/*.{ts,tsx}'],
    extends: [
      // Other configs...

      // Remove tseslint.configs.recommended and replace with this
      tseslint.configs.recommendedTypeChecked,
      // Alternatively, use this for stricter rules
      tseslint.configs.strictTypeChecked,
      // Optionally, add this for stylistic rules
      tseslint.configs.stylisticTypeChecked,

      // Other configs...
    ],
    languageOptions: {
      parserOptions: {
        project: ['./tsconfig.node.json', './tsconfig.app.json'],
        tsconfigRootDir: import.meta.dirname,
      },
      // other options...
    },
  },
# Snake Game

Welcome to the Snake Game, bro! This is a modern React + TypeScript implementation of the classic Snake game, built for fun and learning.

## Features
- Classic snake gameplay
- Responsive controls
- Clean UI with React
- Fast build with Vite

## Getting Started

### Prerequisites
- Node.js (v16+ recommended)
- npm or yarn

### Install
```bash
npm install
```

### Run the Game
```bash
npm run dev
```
Then open your browser to the local server URL (usually http://localhost:5173).

### Build for Production
```bash
npm run build
```

## Project Structure
- `src/` - Main source code (React components, styles)
- `public/` - Static assets
- `index.html` - App entry point
- `vite.config.ts` - Vite config

## Playwright Features
Check out `playwright-features.md` for end-to-end test ideas and automation tips.

## Contributing
Pull requests are welcome, bro! For major changes, open an issue first to discuss what you want to change.

## License
MIT
