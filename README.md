Python-Secure-Socket-Chat - AUTHOR: ALMODAD MUTINDA - MOI UNIVERSITY
=====================================================================

Python Secure Socket Chat With Diffie Hellman is a secure, cross-platform socket based chat application utilizing Diffie-Hellman key exchange to send secure chat messages across the internet. This application uses the client-server architecture.

USER MANUAL

SYSTEM REQUIREMENTS

Hardware Requirements:
The minimum requirements are as follows:
.	512 MB RAM
.	Processor with speed of 1GHz.
.	Internet or LAN connection (not mandatory).
.	MOUSE: 2 or 3 button mouse
.	KEYBOARD: 101 key Keyboard
.	A 14’’ (or bigger) display screen/monitor

Software requirements
.	Python interpreter (version 2.7 or higher)
.	Pygame python library (for playing audio chat notifications)
.	Operating system that supports python. (A Linux based system is preferred, eg. UBUNTU) 

ENVIRONMENT SETUP

This application has been tested in UBUNTU 14.04.
In Linux based systems, python 2.7 is installed by default. However python 3 is not. This is needed for some components of this application to run.

In order to install the simple chat application, a few dependencies should be installed first. Follow these steps to install python3 and pygame:
1.
    Change to your home directory.
    cd ~
    Get Pygame source code.

    sudo apt-get install mercurial
    hg clone https://bitbucket.org/pygame/pygame
    cd pygame

    Install dependencies.
    sudo apt-get install python3-dev python3-numpy libsdl-dev libsdl-image1.2-dev \
      libsdl-mixer1.2-dev libsdl-ttf2.0-dev libsmpeg-dev libportmidi-dev \
      libavformat-dev libswscale-dev libjpeg-dev libfreetype6-dev

    Build and install Pygame.
    python3 setup.py build
    sudo python3 setup.py install 
Done. You can now use the simple chat application. 

To run the application:
2. Copy the folder called SwiftChat to a location on your computer, say /home/yourname/.
a)  Open the terminal
b) change directory to where to where you copied the SwiftChat folder, e.g.
     /home/yourname/SwiftChat

Note: The application contains user defined modules. For python to interpret these modules, the PYTHONPATH environment variable needs to point to the application root. Therefore, run the following command to export PYTHONPATH:

export PYTHONPATH=${PYTHONPATH}:/home/yourname/SwiftChat

Now you are ready to run the application. First, run the server by typing:
python3 startserver.py

Once the server is running, open a new tab in the terminal and run the client by typing:
python3 startclient.py

Once the client is running, login/create a username by typing the preferred name in the textbox and press <Enter>.  A default password will be generated for you. The password is in the form, username-0-1-. You can use it to login later in the console mode.

Repeat the above step until you get two or more clients, as desired.

To start a chat with a logged in client, select the client from the Who is online list and click the Chat Now button.

The other client needs to accept the chat by selecting the requesting client and clicking the Chat Now button.

The secret key and the encrypted message are printed on the terminal as clients exchange messages.

To run the application in console mode, change directory to console/ and type:
python server.py to run the server
Then 
python client.py to run the client

The console mode supports both group chat and private chat.

APPLICATION CONFIGURATION:

The application configuration can be edited in the file SwiftChat/common/config/config.py

