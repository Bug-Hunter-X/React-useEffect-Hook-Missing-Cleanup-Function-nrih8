# React useEffect Hook Missing Cleanup Function

This repository demonstrates a common error in React applications involving the `useEffect` hook:  forgetting to include a cleanup function. This can lead to memory leaks and unexpected behavior.

The `bug.js` file shows the erroneous code. The `bugSolution.js` provides the corrected version.

## Problem

The `useEffect` hook in `bug.js` lacks a return statement for the cleanup function. This means that any side effects initiated within the effect will not be properly cleaned up when the component unmounts or updates.  This is particularly problematic with things like event listeners or subscriptions.

## Solution

The `bugSolution.js` demonstrates the corrected code.  The addition of a return statement with the cleanup function ensures resources are released properly.
