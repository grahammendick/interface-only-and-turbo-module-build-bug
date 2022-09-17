# interfaceOnly and TurboMoule build on Android
React Native published an [example repo that shows how to autolink libraries that contain interfaceOnly components](https://github.com/troZee/react-native-cpp-autolinking). But the approach doesn't work when the library also has a TurboModule. This repository contains an example app built from `npx react-native init`. The only thing I've added is a dependency to my `navigation-react-native` library. My library has `interfaceOnly` components and a TurboModue.

## Steps to recreate the problem
1. cd to the `example` app
2. Run `npm install`
3. Run `npx react-native run-android`
4. See the TurboModule error `error: cannot find symbol
public class Material3Module extends NativeMaterial3ModuleSpec {` 
