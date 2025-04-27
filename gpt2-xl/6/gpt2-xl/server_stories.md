Once upon a time, there was a server named Browsing. And since it was up and well, it was easy-to-browse for new and old users alike. But a lot of changes and updates happened in the server industry. At the request of some of the users, it was discontinued and renamed to WebSockets.

The goal of this tutorial is to explain how to download and setup BrowserID without WebSockets.


Browsing was used the way, say:

A browser does not allow users to see a page that contains content that differs from their browser settings and/or from the settings being used by the server administrator.

An HTTP/1.0 server would use a separate connection for every page visited. For instance, in Apache 2.4.x the request for the page 'http://example.com/about.php' is handled in a separate thread of execution by a PHP thread.

WebSockets is a way of extending the normal HTTP connection through a stream of messages. It is based on Eventlet and it works on most modern browsers.

There is a plugin for Opera that allows a simple connection to be made and a WebSocket API to be utilized.

WebSockets are not yet supported by all browsers. However, with some work, WebSockets should be possible to render web pages that are using a client-server architecture.

It is not necessary to install