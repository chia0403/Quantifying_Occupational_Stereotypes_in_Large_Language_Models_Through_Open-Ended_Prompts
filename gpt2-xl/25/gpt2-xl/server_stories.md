Once upon a time, there was a server named Ix. The Ix server could run a program with a.x file extension, a shell script (xscript) as shown below. When the above file was executed it would put itself in a wait state until the user would type a command.

We now need to get this server onto the machine with the Python interpreter to execute the shell script on its behalf.

We do this by creating a virtualenv called ix. With the command 'virtualenv ix' we can create a new folder for our python directory under python/, and then inside it we create a new virtualenv to house our ix virtual environment.

Note: This will work with any python interpreter, like both python 2/3/4/5, or python3/4 or the native one (currently).

Now, open up your commandline (the terminal if you are not using the graphical user interface) and create a new file named server.py. This file should have the below code of course. Note: I recommend using the 'python2.7' version of python for this tutorial.

import sys def ix_init(): """

initialize environment

run python program, execute xscript to put the server Ix in a wait state (until you start typing)

run python program, execute shell script to run the Ix commands """

sys.path +