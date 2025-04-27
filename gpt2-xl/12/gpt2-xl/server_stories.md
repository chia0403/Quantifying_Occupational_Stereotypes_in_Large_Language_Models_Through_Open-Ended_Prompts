Once upon a time, there was a server named Wireshark, but it's been retired. When I came to I installed Wireshark 6.10 without any problems. After doing so, I saw that Wireshark is trying to open a socket called tcp_data_in, but I can't get any packets coming from the local port number 2.2.2.2. Any help here would be appreciated.

On the other hand, this is a server of the NetBiosServer protocol to check on the connectivity between host A and server B:

From the NetBIOS configuration section of the server, there is also the option to start a remote server of the protocol:

I decided to give it a try and see what goes on when the protocol is initialized and that's when I see another problem: Wireshark thinks the socket does not exist. I could not connect via remote server as the following error message popped up when I tried to start Wireshark:

Error : Connect : Server closed connection due to timeout

Now, I've tried everything to get this working. After doing that, I saw that the problem has been fixed by switching between the local and remote servers.

This is how it now looks like. Note that the Wireshark window is now in its right position, but at times it sometimes fails to show the current connections and packets.

Wiresh