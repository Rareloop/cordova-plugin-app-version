# Cordova App Version Plugin

Cordova/PhoneGap plugin for accessing the native app's version and build number within JavaScript. The values are bootstrapped at app load and can be used synchronously.

## Supported Platforms

- iOS
- Android
- Windows

## Installation

The plugin can be installed with the Cordova CLI:

```shell
cordova plugin add cordova-plugin-appversion
```

The plugin is hosted on NPM so requires Cordova CLI `5.0.0` as a minimum. If you have any issues installing, make sure you have the most upto date version of Cordova from NPM:

```shell
npm install -g cordova
```

## Usage

After `deviceReady` has fired you'll be able to access a new object in the global scope that contains three version-related properties:

- *version*: string value of the released version number
- *build*: number value of the build (more useful for Android)
- *buildString*: string value of the build (more useful for iOS, although also passes the Android build back as a string)

```javascript
console.log(AppVersion.version); // e.g. "1.2.3"
console.log(AppVersion.build); // e.g. 1234
console.log(AppVersion.buildString); // e.g. "1.2.3b4"
```
