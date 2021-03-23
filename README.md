# eslint-config-mi-react

This package provides MI's .eslintrc as an extensible shared config.

## Installation

1. Install library via command

```
yarn add eslint-config-mi-react -D
```

2. Install peer dependencies

```
npx install-peerdeps eslint-config-mi-react --dev -Y
```

## Usage

### Configure ESLint

To enable this configuration to your project, create a `.eslintrc` file in the root of your project.

Add `"extends": "eslint-config-mi-react"` to your `.eslintrc`, e.g.:

```
{
  "extends": "eslint-config-mi-react"
}
```

### Configure Prettier

Create a `.prettierrc.js` file in the root of your project. Import prettier rules and export from file.

```
const defaultConfigs = require('eslint-config-mi-react/prettierrc');

module.exports = {
  ...defaultConfigs,
};
```

### Configure Babel

Create a `.babelrc.js` file in the root of your project. Import babel configs and export from file.

```
const { presets } = require('eslint-config-mi-react/babelrc');

module.exports = {
  presets: [...presets],
};

```
