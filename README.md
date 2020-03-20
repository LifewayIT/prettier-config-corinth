# Prettier Config

Prettier config for the LifewayIT Corinth team.

## Setup

1. Install the following as dev dependencies via npm or similar:

- [prettier](https://github.com/prettier/prettier)
- [eslint-config-prettier](https://github.com/prettier/eslint-config-prettier)
- You can download this dependency via GitHub with `npm install github:LifewayIT/prettier-config-corinth -D`.

2. Add a `prettier.config.js` file to the root of the repo. It will need to include the following:

```
const prettierConfig = require('prettier-corinth');

module.exports = prettierConfig;
```

3. If applicable, extend the existing eslintrc file to include `prettier`. For example:

```
module.exports = {
  env: {
    node: true,
    es6: true
  },
  extends: ["corinth", "prettier"]
};
```

4. Enjoy

## Modify Rules

If you would like to modify the prettier configuration, simply modify the `index.json` file. The docs for possible options are [here](https://prettier.io/docs/en/options.html).
