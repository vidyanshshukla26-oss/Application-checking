#Application Checking

A cross-platform mobile application built with Expo (v54) and React Native, featuring bottom-tab navigation for iOS, Android, and Web.
Tech Stack
PackageVersionExpo~54.0.33React19.1.0React Native0.81.5React Navigation (Bottom Tabs)^7.16.1React Navigation (Native)^7.2.4expo-status-bar~3.0.9react-native-safe-area-context~5.6.0react-native-screens~4.16.0
Prerequisites

Node.js (LTS recommended)
npm or yarn
Expo CLI — install globally via npm install -g expo-cli
For iOS: macOS with Xcode installed
For Android: Android Studio with an emulator or a physical device

Getting Started

Clone the repository

bash   git clone https://github.com/your-username/my_app.git
   cd my_app

Install dependencies

bash   npm install

Start the development server

bash   npm start
This launches Expo Dev Tools in your browser. From there you can open the app on a simulator, emulator, or physical device.
Running on a Specific Platform
bash# iOS simulator (macOS only)
npm run ios

# Android emulator / device
npm run android

# Web browser
npm run web
Project Structure
my_app/
├── assets/             # App icons, splash screen, and other static assets
├── src/
│   └── App.js          # Root application component
├── index.js            # Entry point — registers the root component with Expo
├── app.json            # Expo configuration
├── package.json        # Dependencies and scripts
└── .gitignore
Configuration
App metadata (name, version, orientation, icons, splash screen) is managed in app.json. Refer to the Expo app.json / app.config.js docs for all available options.
Building for Production
Use EAS Build for creating production-ready binaries:
bash# Install EAS CLI
npm install -g eas-cli

# Log in to your Expo account
eas login

# Configure the project (first time only)
eas build:configure

# Build for Android
eas build --platform android

# Build for iOS
eas build --platform ios
Contributing

Fork the repository
Create a feature branch: git checkout -b feature/your-feature
Commit your changes: git commit -m "feat: add your feature"
Push to the branch: git push origin feature/your-feature
Open a Pull Request

License
This project is private. All rights reserved.
