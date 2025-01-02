# Expo Android Build Failure: Gradle/AGP Version Mismatch

This repository demonstrates a common error encountered when building Android apps with Expo CLI. The issue stems from a conflict between the Android Gradle Plugin (AGP) version and the Gradle version used in the project.  This can result in cryptic error messages during the build process.

The `buildError.js` file shows a sample project setup that triggers the error. The `buildSolution.js` file provides the solution to resolve this incompatibility.

**Steps to Reproduce (buildError.js):**

1.  Follow the instructions in `buildError.js` to set up a minimal Expo project with a Gradle configuration likely to cause this issue.
2.  Attempt to build the Android APK using `expo build:android`.
3.  Observe the error messages indicating version conflicts.

**Solution (buildSolution.js):**

The solution involves ensuring compatibility between your AGP and Gradle versions. Refer to the official Android Gradle Plugin release notes for compatibility information.
The `buildSolution.js` file demonstrates how to configure your `android/gradle/wrapper` and `android/build.gradle` files to align the versions and resolve the conflict.