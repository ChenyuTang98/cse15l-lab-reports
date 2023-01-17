# Installing VScode
* To install VScode, go to the Visual Studio Code website [Link](https://code.visualstudio.com/), and follow the instructions to download and install it on your computer. I did the version of operating systems with macOS (for Macs).
* After installed, go to VScode to open a window that looks like below. The system color and theme might be different, which would be fine. Mines is already installed before, so it would be slightly different.
![Image](file:///Users/Lenovo1/Desktop/Screenshot%202023-01-11%20at%203.19.45%20PM.png)

# Remotely Connecting
Here we would use VScode to connect to a remote computer over the Internet to do work there.
* For Windows user, you first need to install git.
* Then, to use ssh, you need to open a terminal in VScode. Use the command `$ ssh cs15lwi23zz@ieng6.ucsd.edu`. Everyone is having a unique course-specific account, please use that one.
* If it's the first time you’ve connected to this server, you will probably get a message saying authenticity can't be established. Just type `yes` and press Enter, and then type in your password for this account. Now if you're logged in, you would see things as below:
![Image](file:///Users/Lenovo1/Desktop/Screenshot%202023-01-11%20at%203.37.41%20PM.png)
 
# Trying Some Commands
Now try running some commands both on your computer, and on the remote computer (following after ssh by using the terminal in VScode).
* You can use commands such as `cd` `ls` `pwd` `mkdir` `cp`, a few times in different ways.
* Here I used `ls -lat` `ssh ls -lat` `ls -a`, and below would be my results of what I typed in.
* Finally, to log out of the remote server in your terminal, you could use either Ctrl-D or run the command `exit`.
![Image](Screenshot 2023-01-11 at 3.43.39 PM.png)
