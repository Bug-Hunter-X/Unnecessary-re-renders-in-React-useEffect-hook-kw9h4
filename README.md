# Unnecessary Re-renders in React useEffect Hook

This repository demonstrates a common React bug involving the `useEffect` hook. The provided code causes unnecessary re-renders because the dependency array is missing, leading to performance issues.

## Bug Description

The `useEffect` hook in `MyComponent` runs after every render instead of only when the `count` state variable changes.  This is inefficient and could lead to unexpected behavior.

## Solution

The solution includes a dependency array (`[count]`) in the `useEffect` hook. This ensures the effect only runs when the `count` value changes, thus optimizing performance.

## How to reproduce

1. Clone this repository
2. Run `npm install`
3. Run `npm start`