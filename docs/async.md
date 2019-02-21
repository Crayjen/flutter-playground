# Async Fetch 

## Basics

**Flutter is declarative. Flutter builds its user interface to reflect the current state of your app**

The declarative style of UI programming has many benefits. Remarkably, there is only one code path for any state of the UI. You describe what the UI should look like for any given state, once — and that is it.

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