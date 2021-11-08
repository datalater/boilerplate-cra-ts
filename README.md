# TypeScript 세팅하기

```bash
yarn create react-app ts-todo --template typescript
```

**craco 설치**

create-react-app-configuration-override(craco)

```bash
yarn add @craco/craco
```

`package.json`:

```json
"scripts": {
  "start": "craco start",
  "build": "craco build"
},
```

**emotion 설치**

```bash
yarn add @emotion/react
```

emotion을 쉽게 사용하기 위해 babel 플러그인 설치:

```bash
yarn add -D @emotion/babel-preset-css-prop
```

craco 설정하기:

`craco.config.js`:

```js
module.exports = {
  babel: {
    presets: ["@emotion/babel-preset-css-prop"],
  },
};
```

**storybook 설치**

```bash
npx -p @storybook/cli sb init
```
