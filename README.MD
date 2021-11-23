# 참고 링크

https://coding-hyeok.tistory.com/34

# 1 create project

npx react-native init pushapp

# 2 create local.properties routing Android SDK installed route

android/local.properties
sdk.dir=/Users/hyukyun/Library/Android/sdk

# Using npm

npm install --save @react-native-firebase/app

# Using Yarn

yarn add @react-native-firebase/app

# Default Module

npm install --save native-base @react-navigation/native react-native-reanimated react-native-gesture-handler react-native-screens react-native-safe-area-context @react-native-community/masked-view @react-navigation/stack @react-navigation/drawer react-native-webview

# SHA-1 키 명령어 (비밀번호 없이 엔터)

Window

keytool -list -v -alias androiddebugkey -keystore %USERPROFILE%\.android\debug.keystore

Mac/Linux

keytool -list -v -alias androiddebugkey -keystore ~/.android/debug.keystore
