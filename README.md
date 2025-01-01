# React useEffect Infinite Loop Bug

This repository demonstrates a common error in React's `useEffect` hook: an infinite loop caused by omitting the dependency array.

## The Bug
The `bug.js` file contains a component that uses `useEffect` without specifying a dependency array. This causes the effect to run after every render, leading to an infinite render loop.

## The Solution
The `bugSolution.js` file shows the corrected code.  By adding an empty dependency array `[]`, we ensure the effect runs only once after the initial render.  Alternatively, the correct dependencies (`count`) should be listed if the effect needs to run whenever a specific value changes.

## How to reproduce
1. Clone this repository.
2. Run `npm install`
3. Run `npm start`
4. Observe the console output for the infinite loop in the original file and the corrected behavior in the solution file.
