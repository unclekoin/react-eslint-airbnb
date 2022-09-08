# React Eslint airbnb setting

```shell
> npx create-react-app . --template typescript
```

1. Remove from `package.json`
```json
  "eslintConfig": {
    "extends": [
      "react-app",
      "react-app/jest"
    ]
  },
  ```

  2. [eslint-config-airbnb](https://www.npmjs.com/package/eslint-config-airbnb)
  ```shell
  npx install-peerdeps --dev eslint-config-airbnb
  ```

3. [eslint-config-airbnb-typescript](https://www.npmjs.com/package/eslint-config-airbnb-typescript)

```shell
npm install eslint-config-airbnb-typescript \
            @typescript-eslint/eslint-plugin@^5.13.0 \
            @typescript-eslint/parser@^5.0.0 \
            --save-dev
```

4.
```json
// package.json
  "scripts": {
    // ...
    "lint": "npx eslint -c .eslintrc --ext .js,.jsx,.ts,.tsx",
    "lint:fix": "npm run lint -- --fix"
  },
```
