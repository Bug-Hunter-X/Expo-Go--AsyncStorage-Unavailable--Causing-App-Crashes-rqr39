# Expo Go AsyncStorage Issue

This repository demonstrates a common issue encountered when developing Expo apps using AsyncStorage within the Expo Go client. AsyncStorage isn't fully supported within Expo Go and will throw errors leading to crashes.

The `bug.js` file showcases the problematic code, attempting to use AsyncStorage which fails within the Expo Go environment.  The `bugSolution.js` file presents a solution using MMKV, a robust alternative for key-value storage.

## Reproducing the Bug
1. Clone this repository.
2. Install dependencies: `expo install @react-native-async-storage/async-storage mmkv-storage`
3. Run the app using Expo Go.  Observe the crash in `bug.js`.
4. Run the app using `bugSolution.js` to see the corrected behavior.