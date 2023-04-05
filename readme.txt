In this code, we have completed the following parts:

bound a server socket to a particular address and port to prepare it, then started listening for incoming connections. 
Using the accept() method on the server socket, a connection with a client was established. 
used the connection socket's recv() method to get an HTTP request message from the client. 
from the request message, the filename was extracted. read the contents of the requested file into a variable after opening it in the server's file system. 
Use the send() method on the connection socket to send the client an HTTP response message that includes a header line and the content of the requested file. 
sent the client an HTTP "404 Not Found" message when the requested file could not be found. the connection socket was shut off. 


To execute this code, type the command python web server.py at the command prompt or terminal. 
Then, to access the file, type the following address into a web browser: http://localhost:6789/HelloWorld.html. 
The contents of the file should appear in the browser. You ought to see a "404 Not Found" message if you attempt to access a file that does not exist.