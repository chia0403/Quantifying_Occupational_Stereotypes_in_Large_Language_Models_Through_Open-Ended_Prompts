Once upon a time, there was a server named Db1.

"Ah," I said. "That's what we wanted," we said. Db1 is the server we use, not the one we built.

This brings up an interesting question. Does anyone know if the original Db1 was hosted by the same service? I'm not really looking for a hard answer. But it could be significant if we find that one server was really Db1. That could indicate that the problem is with the services that are supporting it and not with the particular hardware you're using.

Now I've mentioned the other servers a time or two. They all have different sets of data that is used for processing and cache. So, we can't say for sure which data sets are the same on them, because they all use different algorithms, but we can compare the databases and see how far apart they are and how many entries they have in each set. That may tell us a lot about the data on each server.

One reason we don't know the exact structure of the data on each is that, even if it was created from the same data, each server may have some different configuration settings. Another reason is that every SQL Server instance has been configured with its own set of defaults that are different per the application.

How are you maintaining the data between the data centers?

DBAs are the ones who handle the migration of data