# React Native Context Error: Context Not Available

This repository demonstrates a common error encountered in React Native applications when utilizing the Context API: the `Context not available` error.  This occurs when a component attempts to access a context value without being properly nested within the context provider.

The `bug.js` file showcases the problematic code that generates the error.  The solution, shown in `bugSolution.js`, illustrates how to correctly structure your components to avoid this issue by wrapping the components that use the context within the context provider.

## How to Reproduce

1. Clone the repository.
2. Run `npm install` to install dependencies.
3. Run the application (using a React Native environment). You will see the error in `bug.js` and the corrected version in `bugSolution.js`.

## Solution

The solution involves ensuring that all components that rely on the context value are rendered *within* the context provider.  This is demonstrated in `bugSolution.js`.