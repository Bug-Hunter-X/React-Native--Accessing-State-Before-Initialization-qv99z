# React Native: Accessing State Before Initialization

This repository demonstrates a common error in React Native: accessing a state variable before it has been initialized.  The example uses the `useState` hook and highlights how to prevent this error using optional chaining. The error typically manifests as unexpected behavior or crashes.

## Problem

In functional components, the `useState` hook initializes state asynchronously. If you attempt to access the state immediately, it might still be `undefined`, resulting in errors.

## Solution

The recommended solution is to use optional chaining (`?.`) to safely access the state variable. This prevents errors when the state is still undefined.  Additional error handling (like default values or conditional rendering) can also be beneficial.