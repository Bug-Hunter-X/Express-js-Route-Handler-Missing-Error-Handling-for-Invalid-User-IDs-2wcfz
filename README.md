# Express.js Route Handler Missing Error Handling for Invalid User IDs

This repository demonstrates a common error in Express.js route handlers: missing error handling for invalid input.

Specifically, the `/users/:id` route attempts to parse the `id` parameter as an integer.  If the `id` is not a valid integer (e.g., it's a string or contains non-numeric characters), the `parseInt` function will return `NaN`, leading to unexpected behavior and potentially crashes.

The `bug.js` file contains the buggy code. The `bugSolution.js` file provides a corrected version with proper error handling.