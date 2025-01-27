# React useEffect Hook Logging Issue

This repository demonstrates a common issue with the React `useEffect` hook where the logged value doesn't update after a state change.  The problem lies in the dependency array of the `useEffect` hook.  The provided solution shows the correct usage.

## Bug Description
The provided code snippet attempts to log the current value of the count state variable using `console.log`. However, only the initial value is displayed, even though the button increments the count.  This is due to missing the `count` variable in the dependency array of the `useEffect` hook. 

## Solution
The solution includes the `count` variable in the dependency array, allowing the log to update whenever the state changes.

## How to Reproduce
1. Clone the repository.
2. Run `npm install`.
3. Run `npm start`.
4. Observe the console log and button behavior.