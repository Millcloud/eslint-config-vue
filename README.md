**DEPRECATED! Check [@modyqyw/eslint-config](https://github.com/MillCloud/eslint-config).**

# @modyqyw/eslint-config-vue

An ESLint shareable config for vue. Also support uni-app and weex.

## Usage

- If you use JavaScript, install the config for JavaScript.

```sh
npm i vue@~2.6.0
npm i -D eslint@~7.10.0 @modyqyw/eslint-config-vue@~1.8.0
```

For yarn, run scripts below.

```sh
yarn add vue@~2.6.0
yarn add -D eslint@~7.10.0 @modyqyw/eslint-config-vue@~1.8.0
```

- If you use TypeScript, install the config for TypeScript.

```sh
npm i vue@~2.6.0 vue-property-decorator@~9.0.0
npm i -D eslint@~7.10.0 typescript@~4.0.0 @modyqyw/eslint-config-vue@~1.8.0
```

For yarn, run scripts below.

```sh
yarn add vue@~2.6.0 vue-property-decorator@~9.0.0
yarn add -D eslint@~7.10.0 typescript@~4.0.0 @modyqyw/eslint-config-vue@~1.8.0
```

- Set up.

```js
// .eslintrc.js
module.exports = {
  extends: ["@modyqyw/vue"], // for js
  // extends: ["@modyqyw/vue/typescript], // for ts
};
```

## VSCode

- Install plugins.
  - [ESLint](https://marketplace.visualstudio.com/items?itemName=dbaeumer.vscode-eslint)
  - [Prettier](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode)
  - [Vetur](https://marketplace.visualstudio.com/items?itemName=octref.vetur)
- Set up `Settings.json`. Then `F1 => Format Document` => `F1 => File: Save`.

```json
{
  "editor.codeActionsOnSave": {
    "source.fixAll": true
  },
  "editor.defaultFormatter": "esbenp.prettier-vscode",
  "emmet.includeLanguages": {
    "javascript": "javascriptreact",
    "typescript": "typescriptreact",
    "json": "jsonc",
    "vue-html": "html"
  },
  "eslint.validate": [
    "javascript",
    "javascriptreact",
    "typescript",
    "typescriptreact",
    "html",
    "vue",
    "vue-html"
  ],
  "files.eol": "\n",
  "files.associations": {
    "*.js": "javascriptreact",
    "*.ts": "typescriptreact",
    "*.wxml": "html",
    "*.wxs": "javascriptreact",
    "*.wxss": "css",
    "*.axml": "html",
    "*.sjs": "javascriptreact",
    "*.acss": "css",
    "*.swan": "html",
    "*.ttml": "html",
    "*.ttss": "css",
    "*.jxml": "html",
    "*.jxss": "css",
    "*.wpy": "vue",
    "*.json": "jsonc",
    "*.nvue": "vue",
    "*.ux": "vue"
  },
  "[vue]": {
    "editor.defaultFormatter": "octref.vetur"
  }
}
```

## More Config

- [@modyqyw/eslint-config](https://github.com/MillCloud/eslint-config)
- [@modyqyw/eslint-config-react](https://github.com/MillCloud/eslint-config-react)

## License

[MIT](./LICENSE)

Copyright (c) 2020-present MillCloud
