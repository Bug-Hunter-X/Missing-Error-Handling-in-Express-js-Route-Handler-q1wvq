# Express.js Route Handler Bug: Missing Error Handling

This repository demonstrates a common bug in Express.js route handlers: missing error handling for invalid input.  The provided code attempts to retrieve a user from an array based on a user ID from the request parameters. However, it lacks proper error handling if the provided ID is not a valid integer, leading to potential crashes or unexpected behavior.

The `bug.js` file contains the buggy code.  The `bugSolution.js` file shows the corrected code with proper error handling to address the issue.

## How to reproduce

1. Clone the repository
2. Run `npm install express`
3. Run `node bug.js`
4. Try accessing `/users/abc` or another invalid ID.