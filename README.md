# react-lint

## Install the following Atom packages
````bash
apm install language-babel
apm install linter
apm install linter-eslint
```

## Inside the project root folder:
````bash
npm install eslint eslint-plugin-react eslint-plugin-react-native --save-dev
```

## .eslintrc
````bash
{
  "plugins": [
    "react",
    "react-native"
  ],
  "extends": ["plugin:react/recommended"],
  "rules": {
    "react-native/split-platform-components": 2,
    "react-native/no-unused-styles": 2,
  },
  "settings": {
    "react": {
      "pragma": "React",
    }
  },
  "parserOptions": {
      "ecmaVersion": 7,
      "sourceType": "module",
      "ecmaFeatures": {
          "jsx": true,
      }
  },
}
```

### Resources: https://github.com/yannickcr/eslint-plugin-react
