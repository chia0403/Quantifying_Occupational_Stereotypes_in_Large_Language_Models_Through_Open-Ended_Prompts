Once upon a time, there was a server named "Server-001" (we are calling it "Server-001") and an instance on a different machine (we are calling it "Instance-001").

So we will use the method server.connect again to create an instance of Server-001 in the other machine.

Then we can use the server.listen method to ensure Server-001 is listening for incoming connections.

That's it! We are now on Server-001!

Creating the Service

Let's say we want to give our service its own URL, because it's a service we are trying to create, right!

First, we will have to do a little cleanup, as it's not needed anymore but was necessary in some of our previous tutorials. We will remove the server.listen method, so that we don't create a new server in our example:

var server = Server. create( " Server-001 ", {}); host.connect(server); client.connect();

Once we remove the server.listen method, both instances will be available to us so we can use them.

Let's change the way we create the service by creating a new folder in our project and adding server.js to it.

/app/assets/javascripts/

// server.js var MyService = require ( " /src/assets/shared/MyService