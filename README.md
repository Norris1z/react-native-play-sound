## react-native-play-sound
React Native module for playing sound and melody on iOS, Android

## Installation via npm
First install the npm package from your app directory:
```
    npm install react-native-play-sound --save
```
## Installation via yarn
First install the yarn package from your app directory:
```
    yarn
```
After save package name in package.json:
```
    yarn add react-native-play-sound
```
After install package saved:
```
    yarn
```
Then link it automatically using:
```
    react-native link react-native-play-sound
```

## Basic usage
ANDROID: Save your sound clip files under the directory android/app/src/main/res/raw. Note that files in this directory must be lowercase and underscored (e.g. my_file_name.mp3) and that subdirectories are not supported by Android.
IOS: Open Xcode and add your sound files to the project.

In React-native project:

```
import PlaySound from 'react-native-play-sound';

// And on press or anywhere you need it :
// PlaySound('sound_name')

// Note that sound name must be identical on Android and iOS

// Example:
        <TouchableOpacity
          onPress={() => PlaySound('jingle_bells_keyboard')}
          style={styles.touchable}
        >
          <Text>Play Jingle Bell</Text>
        </TouchableOpacity>

```