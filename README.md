# Silent Crash on Unhandled Promise Rejection in React Native Fetch

This repository demonstrates a common yet frustrating issue in React Native: silent crashes due to unhandled promise rejections during data fetching.  The app appears to freeze or simply stop responding without providing any clear error messages to the user.

The `bug.js` file contains the buggy code. The `bugSolution.js` demonstrates how to fix this issue using appropriate error handling and the `console.error` function.  Understanding and implementing proper error handling is crucial for building robust and user-friendly React Native applications. 

## Reproducing the Bug

1. Clone the repository.
2. Run `npm install` to install dependencies.
3. Run the app on your emulator or device.
4. Observe that the app crashes without a clear indication of what went wrong, potentially due to the api failing or returning an error.

## Solution

The solution involves enhancing the `try...catch` block to handle potential errors during the fetch process more effectively. The corrected code in `bugSolution.js` includes a `console.error` statement and improved error messaging to the user, preventing silent failures. It also incorporates a better way to handle the loading state.