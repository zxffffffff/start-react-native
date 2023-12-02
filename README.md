# start-react-native
 一个 RN 脚手架

# 开发环境

- 需要安装 Node.js 用于本地开发，不同平台还需额外安装步骤
- 参考：https://reactnative.dev/docs/environment-setup

## macOS

```bash
brew install node
brew install watchman # 监视文件变化
```

## iOS

手动安装 Xcode
```bash
brew install ios-deploy
```

## Android

以下安装 OpenJDK 发行版，也可以手动安装 Java，建议使用 JDK 11 (兼容问题)
```bash
brew tap homebrew/cask-versions
brew install --cask zulu11
brew info --cask zulu11         # 获取 cask 安装路径，双击安装
```

手动安装 Android Studio
```bash
- Android SDK
- Android SDK Platform
- Android Virtual Device
- Android 13 (Tiramisu)
- Android SDK Platform 33
# 添加 ~/.zshrc
export ANDROID_HOME=$HOME/Library/Android/sdk
export PATH=$PATH:$ANDROID_HOME/emulator
export PATH=$PATH:$ANDROID_HOME/platform-tools
```

# 创建 React Native 工程

参考：https://reactnative.dev/
```bash
# 检查开发环境
npx react-native doctor

# verbose 更多信息
npx react-native@latest init StartReactNative --verbose

# 运行
npm start   # Metro (将模块转换/转译为目标平台)
npm run ios # or android
```

# 【可选】安装 Antd for RN

参考：https://rn.mobile.ant.design/index-cn
```bash
npm install @ant-design/react-native --save
# 可选：字体和图标
npm install @ant-design/icons-react-native --save
```



This is a new [**React Native**](https://reactnative.dev) project, bootstrapped using [`@react-native-community/cli`](https://github.com/react-native-community/cli).

# Getting Started

>**Note**: Make sure you have completed the [React Native - Environment Setup](https://reactnative.dev/docs/environment-setup) instructions till "Creating a new application" step, before proceeding.

## Step 1: Start the Metro Server

First, you will need to start **Metro**, the JavaScript _bundler_ that ships _with_ React Native.

To start Metro, run the following command from the _root_ of your React Native project:

```bash
# using npm
npm start

# OR using Yarn
yarn start
```

## Step 2: Start your Application

Let Metro Bundler run in its _own_ terminal. Open a _new_ terminal from the _root_ of your React Native project. Run the following command to start your _Android_ or _iOS_ app:

### For Android

```bash
# using npm
npm run android

# OR using Yarn
yarn android
```

### For iOS

```bash
# using npm
npm run ios

# OR using Yarn
yarn ios
```

If everything is set up _correctly_, you should see your new app running in your _Android Emulator_ or _iOS Simulator_ shortly provided you have set up your emulator/simulator correctly.

This is one way to run your app — you can also run it directly from within Android Studio and Xcode respectively.

## Step 3: Modifying your App

Now that you have successfully run the app, let's modify it.

1. Open `App.tsx` in your text editor of choice and edit some lines.
2. For **Android**: Press the <kbd>R</kbd> key twice or select **"Reload"** from the **Developer Menu** (<kbd>Ctrl</kbd> + <kbd>M</kbd> (on Window and Linux) or <kbd>Cmd ⌘</kbd> + <kbd>M</kbd> (on macOS)) to see your changes!

   For **iOS**: Hit <kbd>Cmd ⌘</kbd> + <kbd>R</kbd> in your iOS Simulator to reload the app and see your changes!

## Congratulations! :tada:

You've successfully run and modified your React Native App. :partying_face:

### Now what?

- If you want to add this new React Native code to an existing application, check out the [Integration guide](https://reactnative.dev/docs/integration-with-existing-apps).
- If you're curious to learn more about React Native, check out the [Introduction to React Native](https://reactnative.dev/docs/getting-started).

# Troubleshooting

If you can't get this to work, see the [Troubleshooting](https://reactnative.dev/docs/troubleshooting) page.

# Learn More

To learn more about React Native, take a look at the following resources:

- [React Native Website](https://reactnative.dev) - learn more about React Native.
- [Getting Started](https://reactnative.dev/docs/environment-setup) - an **overview** of React Native and how setup your environment.
- [Learn the Basics](https://reactnative.dev/docs/getting-started) - a **guided tour** of the React Native **basics**.
- [Blog](https://reactnative.dev/blog) - read the latest official React Native **Blog** posts.
- [`@facebook/react-native`](https://github.com/facebook/react-native) - the Open Source; GitHub **repository** for React Native.
