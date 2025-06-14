# App

This repository contains a minimal Android project skeleton.

## Prerequisites

- [Android Studio](https://developer.android.com/studio) (latest stable release)
- Android SDK with **compileSdkVersion** 33
- **minSdkVersion** 21
- JDK 11 or later

## Setting up Android Studio

1. Install Android Studio from the official website.
2. Open Android Studio and choose **Open an existing project**, then select this directory.
3. When prompted, install any missing SDK components.
4. Wait for Gradle to sync the project. The first sync may take a few minutes.

## Building from the command line

If you prefer not to use the IDE, you can build the debug APK directly:

```bash
./gradlew assembleDebug
```

The APK will be located in `app/build/outputs/apk/debug/` when the build completes.

## Troubleshooting Gradle sync issues

- **Check your internet connection.** Gradle must download dependencies on the first build.
- **Refresh dependencies.** Run `./gradlew --refresh-dependencies` to force an update.
- **Clear the Gradle cache.** Removing the `.gradle` directory in your home folder can resolve corrupted downloads.
- **Update the Gradle wrapper.** Use `./gradlew wrapper --gradle-version <version>` if you encounter version conflicts.

If sync problems persist, inspect the "Build" tool window in Android Studio for detailed error messages.
