# Foodies

**Discover recipes, explore meal categories and keep your favorite dishes close.**

<img src="Foodies/carrot.png" width="120" alt="Foodies icon" />

## Features

- Browse meals by category and search by name.
- Open recipe details and preparation information.
- Save favorites in a local Room database.
- Navigate between home, categories, search and favorites.

![Foodies app screens](Foodies/screenshots.png)

## Quick start

Use Android Studio with Android SDK 32 and a JDK compatible with Android Gradle Plugin 7.2.0. The app targets Android 5.0 / API 21 or newer. Internet access is required to load meals and images.

```bash
git clone https://github.com/Muqimovdavronbek/Foodies-App.git
cd Foodies-App

```

Open the repository root in Android Studio, complete Gradle sync, select an emulator or connected device, then run the `app` configuration.

Build a debug APK on Linux/macOS:

```bash
chmod +x gradlew
./gradlew assembleDebug
```

On Windows, run `gradlew.bat assembleDebug`. Output: `app/build/outputs/apk/debug/app-debug.apk`.

## Usage

Choose a category or search for a meal, open its recipe and add it to favorites. Saved entries appear in the Favorites screen.

## Architecture

| Directory | Purpose |
| --- | --- |
| `app/src/main/java/com/example/foodies/ui/` | Activities and fragments |
| `app/src/main/java/com/example/foodies/viewmodel/` | Screen state |
| `app/src/main/java/com/example/foodies/data/` | Remote API and local database |
| `app/src/main/res/` | Layouts, icons and themes |

Built with Kotlin, MVVM/LiveData, Retrofit, Room, Hilt, Coroutines and Coil. The original Foodies-App project is credited to MathRoda; meal data is provided by TheMealDB.

## Troubleshooting and contributions

For Gradle errors, check the JDK and SDK configuration before changing dependency versions. For an empty meal list, check device connectivity. Bug reports should include Android version, reproduction steps and the error message.
