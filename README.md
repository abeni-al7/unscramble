# Unscramble

A word game: unscramble the shown word, submit your guess or skip, and score points over a 10-word round.

Built while following Google's [Android Basics with Compose](https://developer.android.com/courses/android-basics-compose/course) course (the "Unscramble" ViewModel codelab).

## Features

- Shows a scrambled word, the current word count (x/10) and your score
- Submit a guess (from the button or the keyboard's Done action) or skip the word
- Wrong guesses are flagged in the text field; correct ones add 20 points
- End-of-game dialog with your final score and **Play Again** / **Exit**

## Built with

- Kotlin, Jetpack Compose, Material 3
- `ViewModel` with `StateFlow<GameUiState>` (`lifecycle-viewmodel-compose`)
- JUnit tests for `GameViewModel` (correct/incorrect guesses, skipping, game over)
- Min SDK 24, target/compile SDK 35

## Run it

1. Open the project folder in Android Studio and let Gradle sync.
2. Run the `app` configuration on an emulator or device (Android 7.0 / API 24 or newer).

Or, with a device or emulator connected:

```sh
./gradlew installDebug
```

Unit tests: `./gradlew test`
