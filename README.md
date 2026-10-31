# TapeDeck MP3 for Android

A small Android music player with a retro cassette animation, local audio-file picker, saved playlist, seek bar, and previous / play-pause / next controls.

## Features

- Select one or multiple audio files using Android's built-in document picker.
- No broad storage permission is required; the user chooses which files the app can access.
- Play, pause, seek, skip forward/backward, and automatically continue to the next track.
- The chosen playlist is remembered between launches when the document provider grants persistent access.
- Cassette reels animate while music is playing.

## Build the APK using GitHub (website workflow)

1. Create a new GitHub repository named `TapeDeckPlayer`.
2. Upload the **contents** of this project folder to the repository root. Make sure `.github/workflows/android.yml` is included; on GitHub, enable viewing hidden files if needed.
3. Open the repository's **Actions** tab.
4. Select **Build TapeDeck MP3 APK** from the workflow list.
5. Press **Run workflow** and confirm.
6. When the run finishes with a green check, open that run and find **Artifacts** at the bottom.
7. Download `tapedeck-debug-apk`, unzip it, and install `app-debug.apk` on your Android phone. Allow installation from that source when Android asks.

The workflow also runs automatically when you push commits to the `main` branch.

## Build locally with Android Studio

- Open this folder in Android Studio.
- Use JDK 17 and install Android SDK Platform 35.
- Let Gradle sync, then choose **Build > Build Bundle(s) / APK(s) > Build APK(s)**.

## App details

- Application ID: `com.example.tapedeck`
- Minimum Android version: Android 6.0 (API 23)
- Target SDK: 35
- Version: 1.0

## Current limitations

This is a foreground player: playback is intended while the app is open. It does not yet include a background media service, lock-screen controls, Bluetooth headset media buttons, equalizer, lyrics, or automatic scanning of the whole phone. Those can be added in a later version.
