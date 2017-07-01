# chatRoom_Nodejs

At the beginning every user can select their name and the server will assign them some random color and will post some system message to the console that a new user just connected. Then the user can post messages. When a user closes the browser window, server will post another system massage to the console that a user has disconnected.

Great advantage of WebSocket is two way communication. In this tutorial it means situation when some user sends a 
message (client -> server) and then server sends that message to all conected users (server -> client) — broadcast.

For client -> server communication I choosed simple text because it’s not necessary to wrap it in more complicated structure.

But for server -> client it’s a bit more complex. We have to distinguish between 3 different types of message:

    server assigns a color to user
    server sends entire message history
    server broadcasts a message to all users

Therefore every message is a simple JavaScript object encoded into JSON.

#Things Used
1.Basic HTML and CSS
2.Node module

