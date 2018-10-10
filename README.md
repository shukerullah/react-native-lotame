
# react-native-lotame

## Getting started

`$ npm install react-native-lotame --save`

### Important
If being added to an Objective c project. After installation. Add a dummy swift file and bridging header file (Xcode should suggest adding it). This is just to let Xcode link swift libraries while building the framework.

### Mostly automatic installation

`$ react-native link react-native-lotame`

### Manual installation


#### iOS

1. In XCode, in the project navigator, right click `Libraries` ➜ `Add Files to [your project's name]`
2. Go to `node_modules` ➜ `react-native-lotame` and add `RNLotame.xcodeproj`
3. In XCode, in the project navigator, select your project. Add `libRNLotame.a` to your project's `Build Phases` ➜ `Link Binary With Libraries`
4. Run your project (`Cmd+R`)<

#### Android

1. Open up `android/app/src/main/java/[...]/MainActivity.java`
  - Add `import com.reactlibrary.RNLotamePackage;` to the imports at the top of the file
  - Add `new RNLotamePackage()` to the list returned by the `getPackages()` method
2. Append the following lines to `android/settings.gradle`:
  	```
  	include ':react-native-lotame'
  	project(':react-native-lotame').projectDir = new File(rootProject.projectDir, 	'../node_modules/react-native-lotame/android')
  	```
3. Insert the following lines inside the dependencies block in `android/app/build.gradle`:
  	```
      compile project(':react-native-lotame')
  	```

#### Windows
[Read it! :D](https://github.com/ReactWindows/react-native)

1. In Visual Studio add the `RNLotame.sln` in `node_modules/react-native-lotame/windows/RNLotame.sln` folder to their solution, reference from their app.
2. Open up your `MainPage.cs` app
  - Add `using Lotame.RNLotame;` to the usings at the top of the file
  - Add `new RNLotamePackage()` to the `List<IReactPackage>` returned by the `Packages` method


## Usage
```javascript
import RNLotame from 'react-native-lotame';

// TODO: What to do with the module?
RNLotame;
```
  