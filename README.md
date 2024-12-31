# React useEffect setInterval Memory Leak

This example demonstrates a common mistake in React: using `setInterval` within the `useEffect` hook without properly cleaning up the interval. This leads to memory leaks and unexpected behavior.

The `bug.js` file contains the faulty code, while `bugSolution.js` provides the corrected version.  The issue arises because the interval continues to run even after the component unmounts.