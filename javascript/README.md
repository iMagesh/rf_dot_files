# Eslint 

### Installation

```
npm install eslint —-save-dev
```

### Installing the style guide

```
npm install eslint-config-airbnb —-save-dev
```

This will install airbnb style guide.

### Eslint React Plugin

```
npm install eslint eslint-plugin-react --save-dev
```

### Eslint React with TypeScript

We can refer to the instructions here
https://andrebnassis.medium.com/setting-eslint-on-a-react-typescript-project-2021-1190a43ffba

### Eslint React Native

```
npm install --save-dev eslint
npm install --save-dev eslint-plugin-react
npm install --save-dev eslint-plugin-react-native

Add plugins section and specify ESLint-plugin-React (optional) and ESLint-plugin-react-native as a plugin.

{
  "plugins": [
    "react",
    "react-native"
  ]
}
```

### Configuring Eslint

We need to create a configuration file called eslintrc. This file can be in either json or yml format.

JSON

```
{
  "extends": "airbnb",
  ...
  ...
  additional rules
}
```

YML

```
extends:
   - "airbnb"
additional_riles:
   ...   
```

### Adding a lint script

package.json

```
"scripts": {
   "lint" : "./node_modules/.bin/eslint"
}
```

### IDE Support

Eslint plugins are available for all popular IDEs and text editors such JetBrains WebStorm, VS Code etc.

### Eslint Plugins/Extensions

Eslint rules can be extended with the help of plugins/extensions depending on the project.
Before using a plugin, we have to install it using npm or yarn

Example

We can use this plugin to add additional rules applicable for TypeScript

@typescript-eslint/eslint-plugin

```
npm install @typescript-eslint/eslint-plugin —-save-dev
```

Similarly eslint-plugin-vue plugin can be used to add additional rules for Vue.js

```
npm install eslint-plugin-vue —-save-dev
```
