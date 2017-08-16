### Is this a bug report?
Yes

### Have you read the [Contributing Guidelines](https://facebook.github.io/react-native/docs/contributing.html)?
Yes

### Environment
1. `react-native -v`:
react-native-cli: 2.0.0
react-native: n/a - not inside a React Native project directory
(I was inside the folder, version is: 0.47.1)
2. `node -v`: v7.10.0
3. `npm -v`: 4.2.0
4. `yarn --version`: 0.17.10

Then, specify:
- Target Platform: Android, iOS
- Development Operating System: macOS Sierra 10.12.6
- Build tools: Using Xcode 8.3.3 and Android Studio 2.3

### Steps to Reproduce
1. `react-native init rn_reproduce_transform_error`
2. `cd rn_reproduce_transform_error`
3. `react-native run-ios` or `react-native run-android`

### Expected Behavior
Should show the default "Welcome to React Native!" screen.

### Actual Behavior
![bundling failed: "TransformError: /Users/eduardo/Desktop/rn_reproduce_transform_error/index.ios.js: Unexpected token ) (While processing preset: \"/Users/eduardo/Desktop/rn_reproduce_transform_error/node_modules/babel-preset-react-native/index.js\")"](https://github.com/esganzerla/rn_reproduce_transform_error/blob/master/screenshots/app-error.png)

Same error occurs when I tried to update RN version to 0.48.0-rc.1
![SyntaxError: Unexpected token )](https://github.com/esganzerla/rn_reproduce_transform_error/blob/master/screenshots/upgrade-error.png)

### Reproducible Demo
https://github.com/esganzerla/rn_reproduce_transform_error

### Notes
- This happens both on android and iOS.
- I saw some people having the same problem on issue #15496.
