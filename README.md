# Create a new React Native project
### 1. Open CMD
### 2. ```npx react-native init <nameproject>```

# Using a physical device

### 1. Open PowerShell
### 2. Run ```adb devices```
### 3. Run ```adb -s <device name> reverse tcp:8081 tcp:8081```
### 4. Rung ```npx react-native run-android```

# React Developer Tools Setup
### 1. Open CMD (run as Administrator)
### 2. Add the react-devtools package to your project using ```npm install --save-dev react-devtools```
### 3. Add ```"react-devtools": "react-devtools"``` to the scripts section in your ```package.json```
### 4. Run ```npm run react-devtools``` from your project folder to open the DevTools.

# VSCode - ESLint, Prettier & Airbnb Setup

### 1. Install ESLint & Prettier extensions for VSCode

Optional - Set format on save and any global prettier options

### 2. Install Packages
```
npm i -D eslint prettier eslint-plugin-prettier eslint-config-prettier
```

```
npx install-peerdeps --dev eslint-config-airbnb
```

### 3. Create .prettierrc for any prettier rules (semicolons, quotes, etc)

### 4. Create .eslintrc.json file (You can generate with eslint --init if you install eslint globally)

```
{
  "extends": ["airbnb", "prettier"],
  "plugins": ["prettier"],
  "rules": {
    "prettier/prettier": "error",
    "no-unused-vars": "warn",
    "no-console": "off",
    "func-names": "off",
    "no-process-exit": "off",
    "object-shorthand": "off",
    "class-methods-use-this": "off"
  }
}
```

### Reference
* ESLint Rules - https://eslint.org/docs/rules/
* Prettier Options - https://prettier.io/docs/en/options.html
* Airbnb Style Guide - https://github.com/airbnb/javascript
