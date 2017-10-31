# dev-env

## Atom

Install packages:
- `apm install atom-beautify prettier-atom linter linter-ui-default intentions busy-signal language-babel linter-eslint highlight-selected sort-lines`

Integrate `prettier-atom` with ESLint
- `Settings -> Packages -> prettier-atom -> Settings -> ESLint Integration`

Install `babel-eslint`
- `yarn add --dev babel-eslint`

Create `eslintrc.json` that extends `airbnb` and adds some custom rules

```
{
    "extends": "airbnb",
    "parser": "babel-eslint",
    "env": {
      "browser": true,
      "es6": true
    },
    "rules": {
      "semi": ["off"]
    }
}
```
