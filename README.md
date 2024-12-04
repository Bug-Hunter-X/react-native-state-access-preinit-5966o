# React Native: Accessing State Before Initialization

This repository demonstrates a common error in React Native where a state variable is accessed before it has been initialized. This often occurs in functional components before the first render. Accessing an uninitialized state variable results in undefined values, causing unexpected behavior or crashes. The provided solution showcases how to mitigate this issue using optional chaining or default values to handle the uninitialized state.

## Bug Description:
The `Bug.js` file shows a functional component that attempts to use the state variable `count` before it's been initialized. This leads to an error because `count` is initially undefined.

## Solution:
The `BugSolution.js` file presents two approaches to solve this problem. The first uses optional chaining (`?.`), and the second utilizes default values during state access.

Both solutions ensure that even before the first render or in case of unexpected behavior, the application will not crash due to undefined state variables. This is crucial for robust application development.