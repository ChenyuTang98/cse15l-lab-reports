#  Search files with specified type ".txt"
Using `find -name` to search for files with a specified name.
source: [Link](https://www.geeksforgeeks.org/find-command-in-linux-with-examples/)
## Example 1:
### command:
```
find ./Castro  -name "*.txt"
```
### output:
```
./Castro/chR.txt
./Castro/chP.txt
./Castro/chQ.txt
./Castro/chB.txt
./Castro/chC.txt
./Castro/chA.txt
./Castro/chV.txt
./Castro/chW.txt
./Castro/chM.txt
./Castro/chZ.txt
./Castro/chL.txt
./Castro/chN.txt
./Castro/chY.txt
./Castro/chO.txt
```
Here I used find -name *.txt to find files with the certain pattern of ".txt" files under folder of Castro. And it shows all the files ended with `.txt`. This command is good to find the certain pattern, especially when sometimes we only need .txt files, or .md files, etc.

## Example 2:
### command:
```
find ./Rybczynski -name "*.txt"
```
### output:
```
./Rybczynski/ch2.txt
./Rybczynski/ch3.txt
./Rybczynski/ch1.txt
```

Here I used find -name *.txt to find files with the certain pattern of ".txt" files under folder of Rybczynski. And it shows all the files ended with `.txt`. This command is good to find the certain pattern, especially when sometimes we only need .txt files, or .md files, etc.

# Search files and folders by size 
Here I used `find -size` to search for files with a specified size.
Source: [Link](https://www.redhat.com/sysadmin/linux-find-command)
## Example 1:
### command:
```
find ./berlitz2 -size +100
```
### output:
```
./berlitz2/Berlin-WhereToGo.txt
./berlitz2/Amsterdam-WhereToGo.txt
./berlitz2/Costa-WhereToGo.txt
./berlitz2/Portugal-WhereToGo.txt
./berlitz2/Boston-WhereToGo.txt
./berlitz2/California-WhereToGo.txt
./berlitz2/Bahamas-WhereToGo.txt
./berlitz2/Crete-WhereToGo.txt
./berlitz2/Canada-WhereToGo.txt
./berlitz2/Bali-WhereToGo.txt
./berlitz2/Budapest-WhereoGo.txt
./berlitz2/Barcelona-WhereToGo.txt
./berlitz2/Athens-WhereToGo.txt
./berlitz2/Paris-WhereToGo.txt
./berlitz2/China-WhereToGo.txt
./berlitz2/PuertoRico-WhereToGo.txt
./berlitz2/Cuba-WhereToGo.txt
./berlitz2/Nepal-WhereToGo.txt
./berlitz2/CanaryIslands-WhereToGo.txt
./berlitz2/Algarve-WhereToGo.txt
./berlitz2/Beijing-WhereToGo.txt
./berlitz2/Bermuda-WhereToGo.txt
./berlitz2/Vallarta-WhereToGo.txt
./berlitz2/Cancun-WhereToGo.txt
```
Here I used find `find ./berlitz2 -size +100` to search for files under berlitz2 folder with the size greater than 100 bytes. The purpose of this is to find the certain file size with limits so sometimes when my storage is not enough so I can find really large files to choose to delete them.
## Example 2:
### command:
```
find ./travel_guides -size -10
```
### output:
```
./travel_guides
./travel_guides/berlitz1
./travel_guides/berlitz1/HandRLasVegas.txt
./travel_guides/berlitz1/HandRIstanbul.txt
./travel_guides/berlitz1/HandRHongKong.txt
./travel_guides/berlitz1/WhatToHawaii.txt
./travel_guides/berlitz1/HandRLisbon.txt
./travel_guides/berlitz1/HandRMallorca.txt
./travel_guides/berlitz1/WhatToFrance.txt
./travel_guides/berlitz1/HandRLosAngeles.txt
./travel_guides/berlitz1/HandRMadeira.txt
./travel_guides/berlitz1/HandRIbiza.txt
./travel_guides/berlitz1/HandRLakeDistrict.txt
./travel_guides/berlitz1/WhereToHawaii.txt
./travel_guides/berlitz1/HandRJerusalem.txt
./travel_guides/berlitz2
```

Here, I used `find ./travel_guides -size -10` to search for files under travel_guides folder with the size smaller than 10 bytes. The purpose of this is to find the certain file size with limits so sometimes when my storage is not enough so I can find really large files to choose to delete them.

# List directories under specified path
Here I used `find -type d` to list all the directories under the certain folder.
Source: [Link](https://www.redhat.com/sysadmin/linux-find-command)
## Example 1:
### command:
```
find ./travel_guides -type d
```
### output:
```
./travel_guides
./travel_guides/berlitz1
./travel_guides/berlitz2
```
Here I used `find ./travel_guides -type d` to search for the directory under travel_guides folder. And I got 2 directories under it. The purpose for this is to look every directory under certain folders so that I could know which directory I'm going into if I only remember certain keywords.
## Example 2:
### command:
```
find ./non-fiction -type d
```
### output:
```
./non-fiction
./non-fiction/OUP
./non-fiction/OUP/Berk
./non-fiction/OUP/Abernathy
./non-fiction/OUP/Rybczynski
./non-fiction/OUP/Kauffman
./non-fiction/OUP/Fletcher
./non-fiction/OUP/Castro
```
Here I used  find the directory under non-fiction directory. The purpose for this is to look every directory under certain folders so that I could know which directory I'm going into if I only remember certain keywords.

# Search files with case insensitive
Source: [Link](https://www.geeksforgeeks.org/find-command-in-linux-with-examples/)

