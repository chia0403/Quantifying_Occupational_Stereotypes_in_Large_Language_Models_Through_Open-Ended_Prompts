Once upon a time, there was a server named "Bubbble" who was used to handle our most popular topics. He was popular because he served every single one of our users. However, as the years rolled by, we started to make new clients that we liked better. And as time passed, we only found them running on other web sites. This means a different server was needed to keep those users online. It meant we had 3 servers to maintain and they all had different specs. So all the issues bubbled up to the top and it just wasn't viable anymore.


While we were discussing this, we were doing something to try and keep all the problems at bay. We decided to make our own service and name it "Reddit".


A Few More Bits about the Server


When you create a new application, our application server takes care of the basics of running your application. When you run an application, it first starts up a database, and then starts a process to fetch new users from the network. Then it starts the application to handle requests and responds to them within a set amount of time.


All of the work is done in the backend using PostgreSQL, and all of our web servers (front and back ends) use PHP to run the database layer of the application. When we are working on a new client or patching up a certain part of our application, it is the Postgres database I start and not the PHP code