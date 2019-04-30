# New project

## Initial git

```
git init
```

- create .gitignore file using https://www.gitignore.io
- ex: https://www.gitignore.io/api/osx,node,windows

## Initial node project

```
yarn init
yarn add express
```

```js
{
  # package.json
  ...
  "scripts": {
    "dev": "node index.js"
  },
  ...
}
```

```
yarn dev
```

```
yarn add --dev eslint
yarn eslint --init
yarn add prettier
```

```js
# .prettierrc
{
  "trailingComma": "es5",
  "tabWidth": 2,
  "semi": false,
  "singleQuote": true
}
```

- command + ,
- workspace setting
- format on save: true

- https://babeljs.io/setup
- https://babeljs.io/docs/en/babel-core

```
# ลง babel-node -> จะได้พร้อมใช้ syntax ใหม่
yarn add @babel/core @babel/node --dev

# ลง preset-env -> ลง syntax พวก import,export และอื่นๆ
yarn add @babel/preset-env --dev
```

- https://babeljs.io/docs/en/babel-preset-env

```js
# .babelrc
{
  "presets": ["@babel/preset-env"]
}
```

```
# ลง plugin-proposal-optional-chaining -> ใช้ ?. ได้
yarn add @babel/plugin-proposal-optional-chaining --dev
```

```js
# .babelrc
{
  ...
  "plugins": ["@babel/plugin-proposal-optional-chaining"]
  ...
}
```

```
# ลงไม่ให้ eslint แดง
yarn add babel-eslint --dev
```

```yaml
# .eslintrc.yaml
parser: babel-eslint
```

- command + ,
- workspace setting
- Javascript › Validate: false
- Typescript › Validate: false
