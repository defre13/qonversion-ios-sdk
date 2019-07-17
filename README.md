![Qonversion](https://qonversion.io/img/brand.png)

Feed your Facebook Ad account with the data on high-value users and see how your Ad account will be enriched with offline purchase events data.

[![Version](https://img.shields.io/cocoapods/v/Qonversion.svg?style=flat)](https://cocoapods.org/pods/Qonversion)
[![Platform](https://img.shields.io/cocoapods/p/Qonversion.svg?style=flat)](https://cocoapods.org/pods/Qonversion)

## Simple Installation:

1. Install Facebook's SDK `FBSDKCoreKit` with their [guide](https://developers.facebook.com/docs/ios/getting-started). 

2. Request the key from [qonversion.io](https://qonversion.io). It's in a beta right now, so no charges on a launch 🐬

3. Provide Facebook's token in your [qonversion.io](https://qonversion.io) account.

4. Run `pod install` with `pod 'Qonversion'` in your pod file (Carthage will be supported later).

5. In your `AppDelegate` in the `application:didFinishLaunchingWithOptions:` method, setup the SDK like so:
```
Qonversion.launch(withKey: "projectKey", autoTrackPurchases: true)
```

SDK will automatically track any purchase events (subscriptions, trials, basic purchases). But If you want to track purchases manually, you can pass `false` in `autoTrackPurchases` and call `trackPurchase:transaction:` on every purchase event in your application.

## Authors

Developed by Team of [Qonversion](https://qonversion.io), and written by [Bogdan Novikov](https://github.com/Axcic) & [Sam Mejlumyan](https://github.com/smejl)

## License

Qonversion SDK is available under the MIT license.
