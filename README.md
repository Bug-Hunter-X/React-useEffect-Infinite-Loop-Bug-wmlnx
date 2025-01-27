# React useEffect Infinite Loop Bug

This repository demonstrates a common error in React's `useEffect` hook: creating an infinite loop by updating state based on the state's current value within the effect's callback function.

The `bug.js` file contains the buggy component. The `bugSolution.js` file provides a corrected version.

## Bug Description
The `useEffect` hook in the buggy component attempts to increment the `count` state variable on every render without a dependency array that correctly manages when it updates, resulting in a continuous re-render and an infinite loop.