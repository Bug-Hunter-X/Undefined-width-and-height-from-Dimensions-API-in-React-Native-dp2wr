## React Native Dimensions API returns undefined width and height

This repository demonstrates a common bug encountered when using the `Dimensions` API in React Native to access screen dimensions. The issue occurs when attempting to access the dimensions before the component has fully mounted, resulting in `undefined` values for `width` and `height`.

The `DimensionsBug.js` file showcases the problematic code.  The `DimensionsBugSolution.js` file provides a solution to address the issue by using the `useEffect` hook to ensure the dimensions are accessed after the component has mounted and potentially making use of state to handle this asynchronous behaviour.

This problem can lead to various issues including layout issues, unexpected behaviour and even crashes. The solution involves using the `useEffect` hook to handle the asynchronous nature of the `Dimensions` API in a clean manner.