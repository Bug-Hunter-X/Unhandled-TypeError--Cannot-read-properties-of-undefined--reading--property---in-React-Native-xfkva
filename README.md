# Unhandled TypeError: Cannot read properties of undefined (reading 'property') in React Native

This repository demonstrates a common error in React Native: attempting to access a property of an object that is null or undefined.  This typically occurs when dealing with asynchronous data fetching. The `bug.js` file shows the problematic code, while `bugSolution.js` provides a solution using optional chaining and nullish coalescing.

## Problem

The issue arises when a component attempts to render before the asynchronous data it relies on is fully loaded. This results in a `TypeError` because the component tries to read a property from an object that hasn't been populated yet.