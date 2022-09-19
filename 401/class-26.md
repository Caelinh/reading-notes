# Android fundamentals

## Introduction to android
- Android apps can be written in Kotlin, Java and C++.
- THe android SDK bundles and compjiles code to be runnable on the platform.
- Android system runs on a multi user linux OS where each app is a user.
- Android uses the principle of least privelege where each app only uses what permissions it needs. Anything else has to be approved by the user.
- 4 types of app components 
    - Activities
    - Services
    - Broadcast receivers
    - Content providers

## Activities

An activity is the entry point for interacting with the user. It represents a single screen with a user interface.
An activity facilitates the following key interactions between system and app.
 - Keeping track of what the user currently cares about (what is on screen) to ensure that the system keeps running the process that is hosting the activity.
 - Knowing that previously used processes contain things the user may return to (stopped activities), and thus more highly prioritize keeping those processes around.
 - Helping the app handle having its process killed so the user can return to activities with their previous state restored.
 - Providing a way for apps to implement user flows between each other, and for the system to coordinate these flows. (The most classic example here being share.)

## Services

Used to keep an app running in the background. For long running operations or for remote processes. Two types of services.
 - **Started Services**
    - Keep running until their work is completed. Some take more priority over others. Such as a more active process like playing music where the user would be upset if interupted. the system will prioritize this service.
 - **Bound services**
  -  Run because some other app (or the system) has said that it wants to make use of the service. This is basically the service providing an API to another process.

## Broadcast Recievers
 - A broadcast receiver is a component that enables the system to deliver events to the app outside of a regular user flow, allowing the app to respond to system-wide broadcast announcements.   
 
## Content provider

 - A content provider manages a shared set of app data that you can store in the file system, in a SQLite database, on the web, or on any other persistent storage location that your app can access. Through the content provider, other apps can query or modify the data if the content provider allows it.   

## Resources
[Android Docs](https://developer.android.com/guide/components/fundamentals)

