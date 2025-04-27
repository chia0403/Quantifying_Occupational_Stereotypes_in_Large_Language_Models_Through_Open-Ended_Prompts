Once upon a time, there was a server named "Server".

"Server" was a wonderful server. It had great features and it was easy to setup and managed. Unfortunately, it had one serious bug: Server was just too powerful, and it managed too many concurrent users. As a result, it frequently crashed.

As of version 0.2.0, these issues have been fixed!

And now that these issues have been fixed, the following has been added to "Server" (it's almost as good as its new name):

The core server is an Apache server running on port 8080.

"Server" accepts anonymous connections and uses the following environment variables:

HOSTNAME - the hostname, without the port number

- the hostname, without the port number PORT - the port

- the port HTTP_PORT - the port used to access HTTP (default is 80)

- the port used to access HTTP (default is 80) HTTP_CONNECTION - the HTTP server to use

- the HTTP server to use HTTP_LOG - the logfile for http requests (default is 127.0.0.1:9990)

- the logfile for http requests (default is 127.0.0.1:9990) AUTH_USER - the username of the user running the server

- the username of the user running the server AUTH_PASS