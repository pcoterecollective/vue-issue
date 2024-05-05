# Vue 3 + TypeScript + Vite

## Steps to reproduce
- Clone repo and install dependencies using `yarn`;
- Run `yarn preview`;
- Open browser's devtools in the `console` tab - `./dist/index.html` was updated with `console.log(app.__vue_app__._instance)`;

## Actual behavior
- app.__vue_app__._instance is `undefined`

## Expected behavior
- app.__vue_app__._instance should have the same value then when in dev mode

## Comments:
- This is important because any difference between values in dev mode and production mode can lead to unexpected behavior and make debugging harder.