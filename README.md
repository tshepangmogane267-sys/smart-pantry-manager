# Smart Pantry Manager

Smart Pantry Manager is a Java Android application that helps users reduce food waste by recording ingredients in their pantry and suggesting recipes that can be made strictly from those ingredients.

## Main features

- Add, view, edit and delete pantry ingredients.
- Store pantry data locally with SQLite.
- Seed 18 recipes on the first run.
- Show only recipes for which every required ingredient and quantity is available.
- Handle simple differences such as `tomato` and `tomatoes`.
- Open a recipe detail screen with ingredients and preparation steps.
- Store the expiry-alert preference in SQLite.

## Technology choice

The project uses Java, Android Studio, AndroidX, Material components, RecyclerView and SQLiteOpenHelper. SQLite was selected because the application is designed for a single user, works offline, and needs reliable local persistence without a separate server.

## How to run

1. Open the `SmartPantryManager` folder in Android Studio.
2. Allow Android Studio to sync the Gradle files.
3. Start an Android emulator or connect a USB-debugging-enabled Android phone.
4. Click **Run** and select the device.
5. Add pantry ingredients such as eggs, tomato and onion to test the strict recipe suggestions.

## Testing the strict rule

Add `eggs` quantity 2, `tomato` quantity 1 and `onion` quantity 0.5. `Tomato Omelette` should appear. Delete onion or reduce its quantity below 0.5. The recipe must disappear because one required ingredient is missing or insufficient.

## Submission evidence still required

The student must add their student number, public GitHub URL, genuine screenshots, and a narrated 5-7 minute demonstration video before submission. GitHub history must be created through meaningful incremental commits; it should not be fabricated in one final upload.
