# Android Gradle Build Fix

The failing project requested Android Gradle Plugin `8.7`, which is not a complete published plugin coordinate. Use `8.7.3` and Gradle `8.9`.

## Replace in the repository root

Copy these files/folders over the existing project:

- `build.gradle`
- `settings.gradle`
- `gradle.properties`
- `.github/workflows/build-apk.yml`
- `gradle/wrapper/gradle-wrapper.properties` if the project uses a wrapper

Do not place the Android project inside an extra nested directory. The repository root must contain `app`, `.github`, `build.gradle`, `settings.gradle`, and `gradle.properties`.
