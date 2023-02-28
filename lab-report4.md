# Step 4:
![Image](4-1.png)
I used the keyboard shortcuts to type `Ctrl-R` and then start typing part of a command, here I used "aop" since this is my distinct account and then I get the whole line I needed to log on to ieng6, `ssh cs15lwi23aop@ieng6.ucsd.edu` showed up, and successfully logged in. Here I don't have to type my password since I have generated SSH Keys for ieng6.
# Step 5:
![Image](4-2.png)
Here, to clone my fork of the repository from my Github account. First I clicked the button `Open with Github Desktop` and then I copied the address under ssh down so that I could run the command `git clone git@github.com:ChenyuTang98/lab7.git` with the copied address 
# Step 6:
![Image](4-3.png)
First I have to change my path to inside the lab7 directory by `cd lab7/`, here I used `<tab> l` and directly get the rest of the command line and pressed `<Enter>`. Then I used `<up><up><up><enter>` to get `javac -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar *.java`because this ommand was 3 up in the search history, so I used up arrow to access it. And then type `java -cp .:lib/hamcrest-core-1.3.jar:lib/junit-4.13.2.jar org.junit.runner.JUnitCore` to run the java files. Here I used the same `<up><up><up><enter>` to get the command since it's in history.
# Step 7:
![Image](4-4.png)
To edit the code file to fix the failing test, first I used `nano ListExamples.java` to directly access the java file I want to make changes to. And then by directly replace the `index1 += 1` in the last while loop with `index2 += 1`. In this way, the incremented index is correct when it's all about loop index2 in list2, and thus could end the infinite loop. In order to save the change, I used `<ctrl-o>` to write-out and used `<ctrl-x>` to exit the editing file.
