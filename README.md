# Unhandled Exception Crash in Node.js Server

This repository demonstrates an example of an unhandled exception in a Node.js server that causes a crash without detailed error information, and provides a solution to handle such exceptions effectively.

## Bug

The server might encounter unexpected errors, such as trying to access a non-existent file, that could crash the server without providing adequate context about the cause of failure.  The `bug.js` file demonstrates this scenario. The lack of proper error handling makes debugging difficult.

## Solution

The solution involves using `try...catch` blocks to wrap potentially problematic code and utilizing logging frameworks to provide more details in case of exceptions. The `bugSolution.js` file shows this improved error handling mechanism.

## How to reproduce

1. Clone the repository.
2. Navigate to the repository directory.
3. Run `node bug.js` to see the unhandled exception and server crash. 
4. Run `node bugSolution.js` to observe the improved error handling and logging.