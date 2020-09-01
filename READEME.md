# Jest
# Typescript
# Typescript


## Setup Jest

### Install
```shell script
npm install --save-dev jest
```

### initialize
// ts-jestを利用する場合はスキップ

```shell script
jest --init
```

### Jest typescript
Compiling typescript jest doesn't support type check.
So you would better use ts-jest

### Install

#### Prerequisite

```shell script
npm i -D jest typescript
```

#### Install ts-jest
[ts-jest documentation](https://github.com/kulshekhar/ts-jest)

```shell script
npm i -D ts-jest @types/jest
```

#### Init ts-jest

````shell script
npx ts-jest config:init
````

- preset: ts-jest => node_modules/ts-jest/jest-preset.js
- testEnvironment: jsdom

### Typescript
```shell script
tsc --init
```

### tsconfig.json
target amd

```json
{
  "compilerOptions": {
    "target": "es5",
    "module": "amd",
    "sourceMap": true,
    "outDir": "./dist",
    "rootDir": "./src"
  }
}
```


## Compiler setting
```shell script
touch tsconfig.build.json
```

#### package.build.json
```json
{
  "extends": "./package.json",
  "includes": ["src"],
  "excludes": ["test"]
}
```

#### package.test.json
```json
{
  "extends": "./package.json",
  "includes": ["**/*.spec.ts"],
}
```

## Jest config setting

### Jest test

### Jest config file
[doc](https://jestjs.io/docs/en/configuration)
- package.json - jest
- jest.config.js
- jest.config.json

### Project setting
https://jestjs.io/docs/en/configuration#projects-arraystring--projectconfig

testRegex [string | array<string>]
Default: (/__tests__/.*|(\\.|/)(test|spec))\\.[jt]sx?$

The pattern or patterns Jest uses to detect test files. By default it looks for .js, .jsx, .ts and .tsx files inside of __tests__ folders, as well as any files with a suffix of .test or .spec (e.g.


## require.js/typescript

## Why change module resolution to node
[module resolution](https://www.typescriptlang.org/docs/handbook/module-resolution.html)
classic - backword compatibility. when target is set to not commonjs (amd, etc)
node-> mimic of node.js. default when target is set to commonjs

## tsconfig
