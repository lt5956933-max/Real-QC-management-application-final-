# Relax QC Control Center - Android project

## Fixed build configuration
- Android Gradle Plugin: 9.4.0
- Gradle: 9.7.1
- compileSdk/targetSdk: 36
- Java: 17
- Built-in QC server: http://192.168.1.110:3000

## IMPORTANT
This package intentionally uses the Gradle version configured by Android Studio/Gradle distribution because the previous package was missing the Gradle wrapper JAR. Do not use an old project copy.

### Android Studio
1. Extract this ZIP.
2. Open ONLY the `android` folder in Android Studio.
3. Go to File > Settings > Build, Execution, Deployment > Build Tools > Gradle.
4. Set Gradle distribution to the Gradle 9.7.1 distribution (or the project's compatible Gradle 9.7.1 wrapper if Android Studio offers it).
5. Set Gradle JDK to JDK 17.
6. Sync Project with Gradle Files.
7. Build > Generate App Bundles or APKs > Generate APKs.

If Android Studio asks to download Gradle 9.7.1 or Android SDK 36, allow it.

## Server
The app opens: http://192.168.1.110:3000
The PC running Node.js must stay on and the phone must be on the same network.

If the PC IP changes, tap the gear in the app and change the server address.

## Node.js backend
From the project root, run `npm install` once, then `npm start`. If port 3000 is already in use and the QC site already opens, do not start a second server.
