# Node Typescript Module Template

## Overview

Typescript node module template with pre-configured build. The project was setup by creating a skeleton node module project and running the following commands to add typescript build and lint options.

```
npm install --save-dev typescript
npm install --save-dev @types/node

npx tsc --init --rootDir src --outDir lib \
  --esModuleInterop --resolveJsonModule --lib es6 \
  --module commonjs --allowJs true --noImplicitAny true

npm install --save-dev eslint @typescript-eslint/parser @typescript-eslint/eslint-plugin
npm install --save-dev prettier eslint-config-prettier eslint-plugin-prettier
```

## Building

Analyse code for potential errors:
```
npm run lint
```

Build project:
```
npm run build
```

## References

* https://docs.npmjs.com/creating-node-js-modules
* https://itnext.io/step-by-step-building-and-publishing-an-npm-typescript-package-44fe7164964c
* https://khalilstemmler.com/blogs/typescript/node-starter-project/
* https://khalilstemmler.com/blogs/typescript/eslint-for-typescript/
* https://www.robertcooper.me/using-eslint-and-prettier-in-a-typescript-project

