# Unresponsive Node.js Server

This repository demonstrates a common Node.js issue: an unresponsive server caused by a long-running synchronous operation blocking the event loop. The `bug.js` file contains the problematic code.  The solution, demonstrated in `bugSolution.js`, involves using asynchronous operations or offloading long-running tasks to worker threads or a message queue.

## How to Reproduce

1. Clone this repository.
2. Run `node bug.js`.
3. Try to access `http://localhost:3000` in your browser.  You'll likely see a timeout or very slow response.

## Solution

The solution utilizes asynchronous operations to prevent blocking the event loop.  The `bugSolution.js` file demonstrates an improved implementation.  Refer to the comments within the code for a detailed explanation.