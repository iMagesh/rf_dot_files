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