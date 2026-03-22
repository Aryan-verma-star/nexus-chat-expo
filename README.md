# Nexus Chat Hub - iOS & Android App

A React-based chat application built with Expo for cross-platform mobile development.

## Features
- Real-time chat functionality
- User authentication
- Job management
- AI-powered features

## Automatic iOS Build

This repository uses **GitHub Actions** to automatically build the iOS app when code is pushed. No Mac required!

### How it works
1. Push code to this repository
2. GitHub Actions automatically builds the iOS app on macOS runners
3. Download the built .ipa file from the Actions artifacts

## Manual Build

### Prerequisites
- Node.js 18+
- Expo CLI
- For iOS: Apple Developer Account (for App Store deployment)
- For Android: Android Studio (optional)

### Setup
```bash
npm install
npx expo prebuild
```

### Build iOS (requires Mac)
```bash
cd ios
pod install
xcodebuild -workspace NexusChatHub.xcworkspace -scheme NexusChatHub -configuration Release build
```

### Build Android
```bash
npx expo run:android
```

## Download Pre-built Apps

### Android
Download the APK from: https://github.com/Aryan-verma-star/nexus-chat-android

### iOS
The iOS build is created automatically via GitHub Actions when you push to main branch.

## Tech Stack
- React Native (via Expo)
- TypeScript
- Supabase (Backend)
- Capacitor (Native wrapping)
