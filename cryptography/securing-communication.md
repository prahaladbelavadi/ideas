# Securing messaging using public cryptography and socket.io

> Needs thought or could already be implemented

__Securing key sessions two with socket.io__

2 Parties can connect to an independent entity Chat room via socket ensuring privacy using keys.

Architecture:

Users connect to a chatroom like branches on a tree.

Chatroom stays open as long as the initiator has the socket connection open.

Each person communicates via the chat room, information is sent to each other and for each message, the audience is described.
Similar to channels on slack, Each person has the liberty to chat with another person only via the same group, but without other people being able to read the message.
