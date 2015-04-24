# Cordova App Version Plugin

Cordova/PhoneGap plugin for accessing the native app's version and build number within JavaScript. The values are bootstrapped at app load and can be used synchronously.

## Supported Platforms

- iOS

## Installation

Using the Cordova CLI:

```shell
cordova plugin add https://github.com/Rareloop/cordova-plugin-app-version.git
```

## Usage

After `deviceReady` has fired you'll be able to access a new object in the global scope that contains both the app version and build number.

```javascript
console.log(AppVersion.version); // e.g. "1.2.3"
console.log(AppVersion.build); // e.g. 1234
```
