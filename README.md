# Node.js Server Error: Unhandled Requests

This repository demonstrates a common error in Node.js servers where requests are not handled correctly.  The original `bug.js` file contains a basic server that lacks proper error handling and might lead to unexpected behavior or crashes under load. The solution, `bugSolution.js`, addresses these issues.

## Bug

The bug lies in the lack of robust error handling. The server might fail to handle exceptions during request processing, causing it to terminate unexpectedly or silently drop requests. 

## Solution

The solution includes comprehensive error handling using `try...catch` blocks and proper event listeners to gracefully manage potential errors and unexpected events.  The solution also demonstrates better resource management, which might be crucial to prevent resource leaks in production environments.

## How to Reproduce

1. Clone this repository.
2. Navigate to the directory.
3. Run `node bug.js` (to see the erroneous behavior).
4. Run `node bugSolution.js` (to see the improved error handling).