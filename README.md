# Socket Chat

This is a very, <i>very</i> simple CLI socket based chat written in Python. It was meant as an early exercise in socket programming and to a lesser extent, familiarizing myself better with Python.

# Dependencies

- Python 3.x
- GNU/Linux
- some open ports

# Execution

You can clone this repository to your computer with the below:

` $ git clone https://github.com/stratzilla/socket-chat`

Execute the `sock_server.py` script first:

` $ ./sock_server.py <IP> <Port>`

Where `<IP>` is the IP address to connect to and `<Port>` likewise is the port to connect to. This script will start a server which will listen for incoming connections by chat clients. In another terminal (or another PC depending on your networking settings), you can open client(s):

` $ ./sock_client.py <IP> <Port>`

Where the arguments again are the IP address and port you'd wish to connect to. Ensure they're identical to where the server is listening.

# Usage

After starting a client, it will prompt for a username. Send messages as you would in any other messenger program and type `/me` to perform an action or `/quit` to quit the server.

Every client can see every message provided they are currently connected. The server will also output all communication it sees between clients.