# Infinite useEffect loop in React

This repository demonstrates a common error in React applications: an infinite loop caused by a missing dependency in the `useEffect` hook.

## Bug Description
The `useEffect` hook is designed to perform side effects after a component renders.  However, if a dependency is missing from the dependency array, the effect will run on every render, leading to an infinite loop of re-renders and potentially crashing the application. 

## How to reproduce
1. Clone the repository.
2. Run `npm install` to install the dependencies.
3. Run `npm start` to start the development server.
4. Observe the console output and the infinite loop.

## Solution
The solution involves correctly specifying the dependency array in the `useEffect` hook, in this case, `count` variable.