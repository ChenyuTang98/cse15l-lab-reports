# Part1
My code StringServer:
```
import java.io.IOException;
import java.net.URI;

class Handler implements URLHandler {
    // The one bit of state on the server: a number that will be manipulated by
    // various requests.
    private String concatenatedString = "";

    public String handleRequest(URI url) {
            System.out.println("Path: " + url.getPath());
            if (url.getPath().contains("/add-message")) {
                String[] parameters = url.getQuery().split("=");
                if (parameters[0].equals("s")) {
                        concatenatedString += parameters[1] + "\n";
                        return concatenatedString;
                }
            }
            return "Invalid input!";

        }
}

class StringServer {
    public static void main(String[] args) throws IOException {
        if(args.length == 0){
            System.out.println("Missing port number! Try any number between 1024 to 49151");
            return;
        }

        int port = Integer.parseInt(args[0]);

        Server.start(port, new Handler());
    }
}
```
![Image](lab2-1.png)
* Which methods in your code are called?
* What are the relevant arguments to those methods, and the values of any relevant fields of the class?
* How do the values of any relevant fields of the class change from this specific request? If no values got changed, explain why.
![Image](lab2-2.png)
* Which methods in your code are called?
* What are the relevant arguments to those methods, and the values of any relevant fields of the class?
* How do the values of any relevant fields of the class change from this specific request? If no values got changed, explain why.

# Part2
* For Windows user, you first need to install git.
 1. Open Visual Studio Code and use the Terminal -> New Terminal menu to open the terminal.
 2. Open the command using ctrl + shift + P.
 3. Select Default Profile and select Git Bash from the options and then click on the + icon in the terminal window.
 4. The new terminal now will be a Git Bash terminal.
* Then, to use ssh, open a terminal in VScode. Use the command `$ ssh cs15lwi23zz@ieng6.ucsd.edu`. "zz" should be replaced with the letter that everyone have a unique course-specific account. To connect remotely, you will need to find your own course-specific account, which can be found by this website [Link](https://sdacs.ucsd.edu/~icc/index.php) and reset your password. 
* If it's the first time you’ve connected to this server, you will probably get a message saying authenticity can't be established. Just type `yes` and press Enter, and then type in your password for this account. Now if you're logged in, you would see things as below:
![Image](cse15lab1-2.png)
 
# Part3
Now try running some commands both on your computer, and on the remote computer (following after ssh by using the terminal in VScode).
* You can use commands such as `cd` `ls` `pwd` `mkdir` `cp`, a few times in different ways.
 1. cd - switch the current working directory to the given path
 2. ls - lists the files and folders for the given path
 3. pwd - prints the current working directory
 4. mkdir - makes a new directory
 5. cp - create a copy of the contents of the file
* Here I used `ls -lat` `ssh ls -lat` `ls -a`, and below would be my results of what I typed in.
* Finally, to log out of the remote server in your terminal, you could use either Ctrl-D or run the command `exit`.
![Image](cse15lab1-3.png)
