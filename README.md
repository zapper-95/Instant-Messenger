# Instant Messanger
## Overview
This code provides a simple instant messaging device using Python with TCP. It also allows users to upload files to the server. As a part of the networks module, my original coursework submission recieved 94/100.  



https://github.com/zapper-95/Instant-Messenger/assets/92369126/8f289204-6382-4e76-a07d-2e60a8662dee



### Running the Server
To run the server run:
```
python server.py [port]
``` 

The server will output during run time about clients connecting, disconnecting and certain exception messages. These will later be stored and saved to a server.log file.

A seperate thread is run to handle input. From there, you can type 'q', to close the server

Please note the server has been set to run on 127.0.0.1, so please use this hostname when connecting with the client.

### Running the Client
To join the server run:
```
python client.py [username] 127.0.0.1 [port]
``` 
To close it, simply type 'q' in the terminal

To send a message, type whatever message you want, and press enter

To upload a file to the server, type the following in the command line
```
upload file_name.extension
``` 
with the approriate file_name and extension.

Multiple clients with the same username are not allowed on the server at the same time.
If a client with username 'NAME' joins the server, and then leaves, he will be able to rejoin with the same username
This means, he will also upload to the same folder, on the server side, as before.

