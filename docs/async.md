# Async Fetch 

## Basics

* Dart code runs in a single “thread” of execution.
* Code that blocks the thread of execution can make your program freeze.
* Future objects (futures) represent the results of asynchronous operations — processing or I/O to be completed later.
* To suspend execution until a future completes, use await in an async function (or use then()).
* To catch errors, use try-catch expressions in async functions (or use catchError()).
* To run code concurrently, create an isolate (or for a web app, a worker).

## WebSockets

* WebSocketChannel that allows you to both listen for messages from the server and push messages to the server.
* StreamBuilder Widget listens for messages 
* In order to send data to the server, add messages to the sink provided by the WebSocketChannel
`channel.sink.add('Hello!');`