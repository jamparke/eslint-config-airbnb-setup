 
# Guide for Eslint, Prettier, & AirBnB Rules for Create-react-app projects

## 1. Install the correct versions of each package, which are listed by the command:

We then install our eslint-airbnb and our prettier dependencies in the terminal like so: 
```
npm install --save-dev eslint eslint-plugin-import@2.7.0 eslint-plugin-jsx-a11y@6.0.2 eslint-plugin-react@7.4.0 eslint-config-airbnb prettier eslint-plugin-prettier eslint-plugin-flowtype babel-eslint eslint-config-prettier
```

## 2. Create a Eslint config call in your root directory and enable AirBnB. 

Make a new file in the project root named .eslintrc and add the following to it:
```
{
  "extends": [
    "airbnb",
    "prettier",
    "prettier/react"
  ],
  "plugins": [
    "prettier"
  ],
  "parserOptions": {
    "ecmaVersion": 2016,
    "sourceType": "module",
    "ecmaFeatures": {
      "jsx": true
    }
  },
  "env": {
    "es6": true,
    "browser": true,
    "node": true
  }
}
```

## 3. Install prettier extension for your editor of choice https://prettier.io/
 
VSCode: [Prettier-Extension](https://marketplace.visualstudio.com/items?itemName=esbenp.prettier-vscode)
Then add this to your VSCode settings so it auto formats on save:
 ```
 "editor.formatOnSave": true
 ```