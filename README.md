# AndroidApps

A collection of small **Android applications** (mostly games and graphics demos), each maintained as an independent Gradle project within this repository. The apps are built with the Android Gradle Plugin and can be opened individually in Android Studio.

## Apps

| App | Folder | Description |
|-----|--------|-------------|
| Catch The Ball | `CatchTheBall/` | An arcade-style game where the player catches a falling ball. |
| Fractal Drawing | `FractalDrawing/` | A graphics app that renders fractal patterns. |
| Guess The Gibberish | `GuessTheGibberish/` | A word/phrase guessing game based on "gibberish" prompts. |
| Maze Musti | `MazeMusti/` | A maze navigation game. |
| My Application | `MyApplication/` | A starter / sample Android project. |

## Tech Stack

- **Platform:** Android
- **Build system:** Gradle with the Android Gradle Plugin (`com.android.tools.build:gradle:3.6.2`)
- **Repositories:** Google + JCenter
- **IDE:** Android Studio (each app includes `.idea`, `gradlew`, and `settings.gradle`)

## Project Structure

Each app is a self-contained Gradle project:

```
<AppName>/
├── app/                 # Application module (source, resources, manifest)
├── build.gradle         # Top-level build configuration
├── settings.gradle      # Module includes (e.g. ':app')
├── gradle.properties
├── gradlew / gradlew.bat
└── gradle/              # Gradle wrapper
```

## Build & Run

Open and run each app individually:

1. In **Android Studio**, choose *Open* and select one of the app folders (e.g. `CatchTheBall`).
2. Let Gradle sync and download dependencies.
3. Build and run on an emulator or a connected Android device.

Alternatively, from a terminal inside an app folder you can build a debug APK with the Gradle wrapper:

```bash
cd CatchTheBall
./gradlew assembleDebug
```

> Note: These projects use the legacy Android Gradle Plugin 3.6.2 and JCenter, so building with a current Android Studio / Gradle version may require updating the plugin version, the Gradle wrapper, and the repository configuration.
