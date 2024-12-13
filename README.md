# React Native useEffect Async State Update Warning/Error

This repository demonstrates a common issue in React Native applications where asynchronous operations within the `useEffect` hook lead to warnings or errors when the component unmounts before the asynchronous action completes.

## Problem

The provided `useEffectBug.js` file shows an example of this problem.  Asynchronous operations, like `setTimeout`, are initiated in the `useEffect` hook. If the component unmounts before the `setTimeout` completes, it will attempt to update state on an unmounted component.