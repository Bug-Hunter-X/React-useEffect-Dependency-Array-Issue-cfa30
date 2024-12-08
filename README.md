# React useEffect Dependency Array Issue

This repository demonstrates a common error in React's `useEffect` hook: forgetting to include state variables in the dependency array.  This leads to the effect only running once (if no dependencies are provided), or to unexpected behavior with stale closures if dependencies are incorrect.

The `bug.js` file shows the problematic code, where the `count` variable is not added in the dependency array of the `useEffect` hook.  The `bugSolution.js` file presents the corrected code, with `count` added to the dependency array, ensuring correct updates.

## How to reproduce

1. Clone this repository.
2. Navigate to the directory.
3. Run `npm install` to install dependencies.
4. Run `npm start` to start the development server.
5. Observe the console logs to see the incorrect behavior in `bug.js` and the corrected behavior in `bugSolution.js`.

## Learn More

For more information on `useEffect` and dependency arrays, refer to the official React documentation:
[https://reactjs.org/docs/hooks-reference.html#useeffect](https://reactjs.org/docs/hooks-reference.html#useeffect)