# Node.js Server Unresponsiveness

This repository demonstrates a common Node.js issue: server unresponsiveness caused by a long-running synchronous operation that blocks the event loop. The `bug.js` file contains a server with a request handler that performs a 5-second CPU-intensive task. This blocks the event loop, making the server unresponsive to new requests.

The `bugSolution.js` file shows how to solve this issue by using asynchronous operations or offloading the long-running task to a worker thread.