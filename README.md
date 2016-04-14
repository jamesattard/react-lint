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
{
  "globals": {
      "require": false,
  },
  "parserOptions": {
      "ecmaVersion": 7,
      "sourceType": "module",
      "ecmaFeatures": {
          "jsx": true,
      }
  },
  "plugins": [
    "react",
    "react-native"
  ],
  "extends": ["eslint:recommended", "plugin:react/recommended"],
  "rules": {
    "comma-dangle" : 0,
    "react-native/no-unused-styles": 2,
    "react-native/split-platform-components": 2,
  },
  "settings": {
    "react": {
      "pragma": "React",
    }
  },
}
