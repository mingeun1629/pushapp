# 기본 세팅

# 참고 링크

https://github.com/zo0r/react-native-push-notification
https://rnfirebase.io/messaging/usage
https://firebase.google.com/docs/cloud-messaging/android/client?hl=ko

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

# /android/build.gradle 파일 의존성 추가

buildscript {
dependencies {
// ... other dependencies
classpath 'com.google.gms:google-services:4.3.3'
}
}

# /android/app/build.gradle 플러그인 추가

apply plugin: 'com.android.application'
apply plugin: 'com.google.gms.google-services' // <- 이 줄만 추가

# npm install

npm install --save @react-native-firebase/messaging
npm install --save react-native-push-notification
