Tic-Tac-Toe over LAN
=====================

This is a Tic Tac Toe game that is ran through the command line written in Python 2. It allows you to play with a friend over the Local Area Network


Prerequisites
--------------
-Python 2.7 (Not python 3 compatible as of now)

-Port 21217 available (can be changed in .py file)



Usage
------

There are 2 python files included with this game, player1.py and player2.py

player1.py acts as a server listening for an incoming connection and should be ran first before player2.py
After starting player1.py it will ask you for your private IP. You can find this using the 'ipconfig' or 'ifconfig' command. After entering your IP, player1.py will bind it with the port and wait for a connection. At this time, player2.py can be started.

player2.py acts as a client and attempts to connect to the server(player1.py) and should be ran after player1.py has setup listening on a socket. Ask your friend for their private IP that they entered when running player1.py
This will be the IP that you will enter when prompted

After the players connect and choose their display name, they will see the game board:

[' 1 ', ' 2 ', ' 3 ']
[' 4 ', ' 5 ', ' 6 ']
[' 7 ', ' 8 ', ' 9 ']

From here, enter the number of the position you want to place your piece. Player 1 is always Xs and Player 2 is always Os


Example usage/video coming soon.





Planned Features
----------------

-'Chat feature' -> chat with your friend during the game

-'Game loop' -> at end of game it will ask if you want to continue 					  playing instead of closing socket

-'Python 3' -> Create python 3 version (Not high priority)




Why?
----

While taking an online Python course, one of the 'homework' assignments was to create a basic tic-tac-toe game. I originally decided to start learning Python for network and security purposes so I'd figure I would get some extra practice and combine my tic-tac-toe game with some networking concepts. 
