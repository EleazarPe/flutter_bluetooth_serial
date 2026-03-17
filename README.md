# Flutter Bluetooth Serial (Updated Fork)

This repository is a fork of **flutter_bluetooth_serial** with the sole purpose of maintaining compatibility with modern Flutter and Android environments.

## Changes Made

- Updated versions of:
  - Flutter SDK
  - Gradle
  - Android Gradle Plugin
  - Kotlin
  - compileSdk / targetSdk (Android)

- Compatibility fixes:
  - Added `android:exported` in the `AndroidManifest`
  - Adjustments to Android 12+ requirements
  - Removal or adaptation of deprecated APIs

- Build adjustments:
  - Updated `gradle.properties` to prevent memory issues (Jetifier / desugaring)
  - AndroidX compatibility

## Objective

Restore the ability to build and run the plugin in modern environments without modifying its original logic or behavior.

No new features were added.

## Status

- Builds successfully on modern Flutter versions
- Compatible with recent Android SDKs (>= 35)
- May still include deprecated APIs that remain functional

## Limitations

- The original plugin is not fully updated to the latest Android standard
- Deprecation warnings may appear during build
- Future compatibility is not guaranteed without further maintenance

## Usage

Used the same way as the original repository:

```yaml
dependencies:
  flutter_bluetooth_serial:
    git:
      url: <URL_OF_THIS_REPOSITORY>
```

## Credits

All credit for the original development goes to the authors of **flutter_bluetooth_serial**.

This fork only introduces maintenance changes to keep it working in modern environments.
