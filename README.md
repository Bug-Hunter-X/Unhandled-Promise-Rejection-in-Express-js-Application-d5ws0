# Unhandled Promise Rejection in Express.js
This repository demonstrates a common error in Express.js applications: unhandled promise rejections in asynchronous operations.  The `bug.js` file shows an Express server with an asynchronous function that might fail.  However, it lacks proper error handling, resulting in silent failures or potential crashes.  The solution, in `bugSolution.js`, demonstrates how to correctly handle these rejections using a `catch` block and a centralized error handler.

## How to Reproduce
1. Clone the repository.
2. Run `node bug.js`.  Observe that the server may or may not report errors depending on the random success/failure of the asynchronous operation.
3. Run `node bugSolution.js`. Observe robust error handling.