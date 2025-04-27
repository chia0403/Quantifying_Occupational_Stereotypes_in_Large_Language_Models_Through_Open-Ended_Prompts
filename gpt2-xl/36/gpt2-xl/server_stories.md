Once upon a time, there was a server named tihmstar. So this server would need an authentication protocol. After reading a little bit more about it, here is my protocol proposal:

It could be called: http-server-idle-authentication.

In all the details, I will assume that I would have to call the http-server-idle-auth.service, and then the http-server-authenticator.service. If you don't have a server ready, go ahead and start it.

The idea is to put the following line in a new file to hold the connection data:

In my application, I can do something like:

Note that I used the string "hello world".

In a way, you could think of server-ip as the same thing: a server name. Then it's just a question of whether you use that or not. Here are my two examples:

(and of course some basic socket configuration would be needed)

So if I have a server called "example.org", which will host this blog:

What I need to do is just call the http-server-idle-auth.service, and specify the server name, listening port, and authentication method. The only thing missing in both of these examples is the actual authentication.

Ok, let's get to that.

For the authentication, I have written an