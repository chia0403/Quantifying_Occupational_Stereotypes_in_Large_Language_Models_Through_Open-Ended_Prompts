Once upon a time, there was a server named "Raspberry" in the "public" network (router) which was accessible on the outside world. In reality, it was on a hidden, private network within the company. The owner of "Raspberry" saw this and installed a self-signed certificate for this server, and now everyone can authenticate.


This is an example of a certificate request generated on the machine.

This server is a machine used for administrative tasks, e.g., configuring the router, managing software updates and so on. A machine used for "administrative" tasks is known as "trusted".

An example of a certificate request sent by the server is shown in the next screenshot:


This is an email requesting a local client to upgrade to "version 3.50" and a self-signed certificate. This is an example of the request sent by the server and can be accepted by the client if it is on the trusted network.


This is email received from the client


This is an example of the certificate given by the server (which was self-signed) given to the client. The certificate is signed by the owner of "Raspberry" and provides authentication.

You may not have a client, but you can still get authentication by asking the "trusted" host. For example, if you visit Raspberry on a "trusted" network, the certificate from the server shows up