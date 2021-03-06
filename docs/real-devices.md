Appium on real devices
======================
Appium has preliminary support for real device testing.

To get started on a real device, you will need the following:

1. An Apple Developer ID and a valid Developer Account with a configured distribution certificate and provisioning profile.
2. An iPad or iPhone.
3. The source code of your app.
4. A Mac with XCode and the XCode Command Line Developer Tools

Provisioning Profile
---

A valid iOS Development Distribution Certificate and Provisioning Profile are necessary to test on a real device. You can find information about configuring these in the [Apple documentation](http://developer.apple.com/library/ios/#documentation/ToolsLanguages/Conceptual/YourFirstAppStoreSubmission/TestYourApponManyDevicesandiOSVersions/TestYourApponManyDevicesandiOSVersions.html)

You will also need to [sign your app](http://developer.apple.com/library/ios/#documentation/ToolsLanguages/Conceptual/YourFirstAppStoreSubmission/ProvisionYourDevicesforDevelopment/ProvisionYourDevicesforDevelopment.html#//apple_ref/doc/uid/TP40011375-CH4-SW1).

Running your tests with Appium
---

Once your device and app are configured, you can run tests on that device by passing the -U flag to server.js:

```
node server.js -U <UDID> --app <PATH_TO_APP>
```

This will start Appium and have Appium use the device to test the app.
