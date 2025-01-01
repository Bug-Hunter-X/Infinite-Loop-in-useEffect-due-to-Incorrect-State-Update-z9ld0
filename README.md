# React useEffect Infinite Loop Bug

This repository demonstrates a common bug in React applications involving the `useEffect` hook. The bug arises from an incorrect way of updating state within the `useEffect`'s callback function, leading to an infinite loop.

## Bug Description

The `bug.js` file contains a React component that uses the `useState` hook to manage a count.  The `useEffect` hook attempts to increment the count on every render, which causes an infinite loop because the state change triggers a re-render, leading to another state change, and so on.

## Solution

The `bugSolution.js` file provides the corrected code.  The issue is resolved by correctly updating the state within the `useEffect` using functional updates to avoid the infinite loop.