# JavaScript Closure and setTimeout Unexpected Behavior

This repository demonstrates a common pitfall in JavaScript involving closures and the `setTimeout` function.  The code in `bug.js` appears to intend to print numbers 0 through 9 with a one-second delay between each. However, due to how closures work in JavaScript, it unexpectedly prints '10' ten times.

The `bugSolution.js` file shows how to correctly capture the value of 'i' using an immediately invoked function expression (IIFE) to create a new scope for each iteration, thus demonstrating the correct implementation and resolving the issue.

## How to Reproduce
1. Clone the repository.
2. Open `bug.js` and `bugSolution.js`.
3. Run `bug.js` to observe the unexpected behavior.
4. Run `bugSolution.js` to observe the corrected behavior.