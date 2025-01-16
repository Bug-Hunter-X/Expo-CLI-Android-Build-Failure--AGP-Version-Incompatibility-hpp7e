# Expo CLI Android Build Failure: AGP Version Incompatibility

This repository demonstrates a bug encountered when building an Android app using the Expo CLI. The issue stems from an incompatibility between the required Android Gradle Plugin (AGP) version and the version available or configured within the Expo project.

## Bug Description

The Expo CLI build process for Android fails due to an AGP version mismatch.  The error message typically highlights that a newer AGP version is required than what's currently installed or compatible with the Expo CLI's configuration.  This results in a build failure and prevents the successful generation of the Android APK.

## Bug Reproduction Steps

1. Clone this repository.
2. Navigate to the project directory.
3. Attempt to build the Android app using the Expo CLI: `expo build:android`
4. Observe the build failure and the error message related to the AGP version incompatibility.

## Solution

The solution involves ensuring compatibility between the required AGP version (as specified in the project's `android/gradle/wrapper/gradle-wrapper.properties` file and the Android Gradle Plugin version installed in your environment. In many cases updating the gradle wrapper to the latest version solves the issue.

## Contributing

Contributions are welcome! If you encounter this issue or a similar one, feel free to open an issue or submit a pull request.