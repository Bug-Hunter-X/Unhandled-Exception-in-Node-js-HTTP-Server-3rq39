# Unhandled Exception in Node.js HTTP Server

This repository demonstrates an example of an unhandled exception in a Node.js HTTP server and its solution.

## Bug

The `bug.js` file contains a simple HTTP server that throws an unhandled exception if the requested URL is `/error`. This causes the server to crash without any proper error handling.

## Solution

The `bugSolution.js` file demonstrates how to handle the exception gracefully using a `try...catch` block. This prevents the server from crashing and allows for more robust error management.

## How to reproduce the bug

1.  Clone this repository.
2.  Run `node bug.js`.
3.  Access `http://localhost:3000/error` in your browser. The server will crash.

## How to see the solution

1.  Run `node bugSolution.js`.
2.  Access `http://localhost:3000/error` in your browser. The server will respond with an error message without crashing.