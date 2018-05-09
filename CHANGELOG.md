Batch Cordova Plugin

## 2.0.0

Rewrote the plugin:

* Native code is now included in the open-source repository, meaning that 3rd party developers can update the underlying native SDKs directly.
* Plugin is fully definied in a typescript definition, improving documentation readability and Ionic support
* Plugin is now testable
* Cordova-plugin's versioning system will now differ from the native SDK versioning

Cordova 8 compatibility. **Note: Users of earlier versions of cordova will have to downgrade to 1.7.4**

Updated native SDKs to 1.12.0

Android now uses FCM to register for notifications: setGCMSenderId has been removed, and you will need to generate a `google-services.json` file to keep push notifications.

## 1.7.4

Update native SDKs to the latest version
The plugin now depends on the appcompat-v7 library on Android
Added support for Mobile Landings
Added a "hasMobileLanding" property in the push event, so you can avoid doing some actions on a push that already displayed a mobile landing

## 1.7.2

Update native SDKs to 1.7  
Added the ability to turn on foreground push delivery on Android (rather than delivering them in the notification center) to match iOS' behaviour.  
The plugin now depends on the support-v4 library

## 1.5.3

Update native SDKs to 1.5.3

## 1.5

Update native SDKs to 1.5
Custom user data (attributes, tags and events)
Added an API to retrieve Batch's unique installation identifier
Deprecated BatchUserProfile
Added ability to start Batch in a service

## 1.4

Update native SDKs to 1.4
iOS 9 and bitcode support

## 1.3.3 Beta 3

Batch Push has a new method to allow you to get the last known push token

## 1.3.3 Beta 2

Updated native sdks to 1.3.3 (prerelease)

Batch Push is now fully available:

* It is now possible to read the notification payload in your JS code
* Setting the wanted notification types is supported

Added Batch Unlock

## 1.3.2 Beta 1

Initial release