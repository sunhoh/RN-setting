# 리액트네이티브 시작하기

## React Native Cli Setting

#### install list

```shell
Homebrew 설치 -> 공홈 참조
Node 설치 -> $ brew install node
JDK 설치 -> $ brew install --cask adoptopenjdk/openjdk/adoptopenjdk11
Watchman 설치 -> $ brew install watchman
Cocoapods 설치 -> $ sudo gem install cocoapods
```

Node package 관리를 위해 [Yarn](https://yarnpkg.com/en/docs/install)도 설치

```shell
brew install yarn
```

이제 ReactNative CLI를 설치해줍니다.

```shell
npm install global react-native-cli
  or
yarn global add react-native-cli
```

#### version check

```shell
$ node --version  -> 16.14.0
$ npm --version   -> 6.14.14
$ npx react-native --version  -> 2.0.1
$ java --version  -> 11.0.11
$ javac --version -> 11.0.11
$ watchman --version ->
$ pod --version  -> 1.11.2
```




## ReactNative project 만들기

```shell
react-native init Project
```

## 빌드 도구 설치(XCode, AndroidStudio)

iOS 앱 제작에 사용할 XCode를 설치합니다.

앱 스토어 -> XCode 검색 -> 설치

Android 앱 제작에 사용할 [AndroidStudio](https://developer.android.com/studio/index.html)를 설치합니다.


### 시뮬레이터에서 구동

#### iOS

iOS 앱을 빌드하고 시뮬레이터에서 구동

```shell
react-native run-ios
```

시뮬레이터 기기를 선택하고자 하는 경우 아래와 같이 특정 지어줄 수 있다.

```shell
react-native run-ios --simulator 'iPhone 6s Plus'
```

#### Android

Android 시뮬레이터를 시작합니다([참조](https://developer.android.com/studio/run/managing-avds.html))

> Tools -> Android -> AVD Manager

Android 앱을 빌드하고 시뮬레이터에서 구동

```shell
react-native run-android
```

#### version check

```shell
gradle-7.2-all.zip
buildToolsVersion = "30.0.2"
targetSdkVersion = 30
dependencies {
  classpath("com.android.tools.build:gradle:4.2.2")
}
```

