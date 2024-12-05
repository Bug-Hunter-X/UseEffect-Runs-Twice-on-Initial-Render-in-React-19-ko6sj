# React 19 useEffect Bug: Double Run on Initial Render

This repository demonstrates a bug encountered in React 19 where the `useEffect` hook runs twice during the initial render of a component.  This can lead to unexpected behavior and performance issues. The solution provides a fix to mitigate the issue.

## Bug Description

The `useEffect` hook, designed to perform side effects after component rendering, is unexpectedly running twice on the initial mount of the component in React 19.  This behavior is inconsistent with the expected single execution. 

## Reproduction Steps

1. Clone this repository.
2. Run `npm install` to install dependencies.
3. Run `npm start` to start the development server.
4. Observe the console logs, noting that the effect runs twice before any interaction with the button. 

## Solution

The solution involves carefully examining and potentially restructuring the component's logic and dependencies within the `useEffect` hook to ensure that the effect runs only when intended and avoiding unnecessary re-renders.