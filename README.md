# React + TypeScript + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react) uses [Babel](https://babeljs.io/) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh

## Tailwindcss

This project is already configure with tailwindcss

## Vitest

This project is configured to use vitest as the testing library. It was installed following this steps:

1. Install dependencies
```sh
npm i -D vitest jsdom @testing-library/react @testing-library/user-event @testing-library/jest-dom
```
2. Create a [./test/setup.ts](./test/setup.ts) file with the code that will run after each test
3. Create [./vitest.config.ts](./vitest.config.ts) to define vitest config
4. Add `test: vitest` command in the package.json
5. Add this option in the [tsConfig.json](./tsConfig.json)`:
```json
"compilerOptions": {
    "types": ["vitest/globals", "@testing-library/jest-dom"]
  }
```
6. Add the same option inside the compilerOptions in the [tsConfig.app.json](./tsConfig.app.json)`:
```json
"types": ["vitest/globals", "@testing-library/jest-dom"]
```


