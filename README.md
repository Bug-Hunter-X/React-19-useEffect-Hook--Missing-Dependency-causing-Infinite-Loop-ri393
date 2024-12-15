# React 19 useEffect Hook: Missing Dependency causing Infinite Loop

This repository demonstrates a common error in React 19 applications involving the `useEffect` hook.  The issue arises from an incomplete dependency array, leading to infinite re-renders and unexpected behavior.  This example showcases the problem and its solution.

## Bug
The `bug.js` file contains a component that uses the `useEffect` hook to log the current count to the console after every render. However, the `count` variable is not included in the dependency array. This causes the effect to run on every render, leading to an infinite loop.

## Solution
The `bugSolution.js` file demonstrates the corrected code. By adding `count` to the dependency array, the effect now only runs when the `count` value changes, resolving the infinite loop problem.