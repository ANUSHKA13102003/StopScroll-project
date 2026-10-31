# StopScroll – Scroll Less. Live More. 📱

**StopScroll** is an Android application designed to help users reduce digital distractions by blocking short-form video content such as Instagram Reels and YouTube Shorts while allowing access to other useful features of social media applications.

## 🚀 Problem Statement

Short-form video platforms encourage endless scrolling, resulting in wasted time, reduced productivity, and difficulty maintaining focus.

Traditional screen-time applications restrict entire apps rather than targeting specific distracting features.

StopScroll aims to solve this problem by targeting short-form video sections without blocking complete applications.

## 💡 Our Solution

StopScroll uses Android Accessibility Services to identify selected short-video interactions and help users avoid unnecessary scrolling.

The goal is to encourage mindful smartphone usage while maintaining access to essential app features.

## ✨ Key Features

- **Smart Detection:** Identifies selected Reels and Shorts accessibility labels.
- **Selective Blocking:** Aims to restrict short-form video sections rather than entire applications.
- **Accessibility Service:** Uses Android accessibility events for content detection.
- **Persistent Service:** Includes background service components.
- **Boot Receiver:** Includes a component to handle device reboot events.
- **User Interface:** Provides dedicated screens for app interaction and settings.

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| Java | Android application development |
| XML | User interface design |
| Android Studio | Development environment |
| Gradle | Build automation |
| Android Accessibility API | UI event detection |

## 🏗️ Project Architecture

The project includes the following major components:

- `MainActivity.java` – Main application screen.
- `SplashActivity.java` – Splash screen.
- `ChoiceActivity.java` – User choice screen.
- `BlockShortsService.java` – Accessibility-based detection logic.
- `PersistentService.java` – Background service component.
- `BootReceiver.java` – Device reboot receiver.
- `AndroidManifest.xml` – Application components and permissions.

## 📂 Project Structure

```text
StopScroll/
│
├── app/
│   ├── src/
│   │   └── main/
│   │       ├── java/
│   │       │   └── com/mythsphere/stopscroll/
│   │       │       ├── MainActivity.java
│   │       │       ├── SplashActivity.java
│   │       │       ├── ChoiceActivity.java
│   │       │       ├── BlockShortsService.java
│   │       │       ├── PersistentService.java
│   │       │       └── BootReceiver.java
│   │       │
│   │       ├── res/
│   │       └── AndroidManifest.xml
│   │
│   └── build.gradle
│
├── gradle/
├── build.gradle
├── settings.gradle
├── gradle.properties
├── gradlew
├── gradlew.bat
└── README.md
```

## ⚙️ Installation and Setup

1. Clone this repository:

```bash
git clone https://github.com/ANUSHKA13102003/StopScroll-project.git
```

2. Open Android Studio.
3. Select **Open** and choose the project folder.
4. Allow Gradle synchronization to complete.
5. Connect an Android device or start an emulator.
6. Run the application.

## 🔐 Accessibility Permission

StopScroll requires Android Accessibility Service permission for its detection functionality.

Users must manually enable the service through Android Settings → Accessibility → StopScroll.

Accessibility permissions should only be enabled after understanding the access they provide.

## 🧪 Current Implementation Status

This project is currently an academic prototype.

The existing detection logic checks selected accessibility-node labels associated with Instagram Reels and YouTube Shorts.

Detection across all app versions, entry points, and Facebook Reels has not yet been fully implemented or verified.

## 🔮 Future Enhancements

- Improved short-video detection across platforms.
- Facebook Reels support.
- Daily screen-time reminders.
- Weekly and monthly activity reports.
- Personalized blocking settings.
- Digital wellbeing recommendations.
- Improved user experience and interface.

## 🎯 Project Objective

To encourage healthier digital habits by helping users take control of their screen time without completely disconnecting from social media.

**StopScroll – Scroll Less. Live More.**

---

## 👩‍💻 Author

**Anushka**

GitHub: [ANUSHKA13102003](https://github.com/ANUSHKA13102003)

---

*Developed as an academic Android application project.*
