# Publishing apps to the play store

## Questions related to reading

1. How are releases and versioning related?
A release is the first iteration of your final app. It's a production version of the app and it's ready for the outside world.
Versions of the app are updates that come out after that improve the release and add more features.

2. What are the 5 main tasks you need to complete to prepare your application for release to the Google Play Store?
    1. Configuring your application for release.
At a minimum you need to remove Log calls and remove the android:debuggable attribute from your manifest file. You should also set your app's version information.
    2. Building and signing a release version of your application.
You can use the Gradle build files with the release build type to build and sign a release version of your application.
    3. Testing the release version of your application.
Before you distribute your application, you should thoroughly test the release version on at least one target handset device and one target tablet device.
    4. Updating application resources for release.
You need to be sure that all application resources such as multimedia files and graphics are updated and included with your application or staged on the proper production servers.
    5. Preparing remote servers and services that your application depends on.
If your application depends on external servers or services, you need to be sure they are secure and production ready.

## Resources
[Play store publishing docs](https://developer.android.com/studio/publish)
