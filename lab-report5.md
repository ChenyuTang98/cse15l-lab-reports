#  Search files with specified type ".txt"
Using `find -name` to search for files with a specified name.
source: [Link](https://www.geeksforgeeks.org/grep-command-in-unixlinux/)
## Example 1:
### command:
```
grep -c "Amsterdam" Amsterdam-WhatToDo.txt
```
### output:
```
23
```
Here I used find -name *.txt to find files with the certain pattern of ".txt" files under folder of Castro. And it shows all the files ended with `.txt`. This command is good to find the certain pattern, especially when sometimes we only need .txt files, or .md files, etc.

## Example 2:
### command:
```
grep -c "China" Beijing-History.tx
```
### output:
```
14
```

Here I used find -name *.txt to find files with the certain pattern of ".txt" files under folder of Rybczynski. And it shows all the files ended with `.txt`. This command is good to find the certain pattern, especially when sometimes we only need .txt files, or .md files, etc.

# Search files and folders by size 
Here I used `find -size` to search for files with a specified size.
Source: [Link](https://www.geeksforgeeks.org/grep-command-in-unixlinux/)
## Example 1:
### command:
```
grep -l "Beijing" *
```
### output:
```
Beijing-History.txt
Beijing-WhatToDo.txt
Beijing-WhereToGo.txt
China-History.txt
China-WhatToDo.txt
China-WhereToGo.txt
Cuba-WhereToGo.txt
```
Here I used find `find ./berlitz2 -size +100` to search for files under berlitz2 folder with the size greater than 100 bytes. The purpose of this is to find the certain file size with limits so sometimes when my storage is not enough so I can find really large files to choose to delete them.
## Example 2:
### command:
```
grep -l "Athen" *
```
### output:
```
Athens-History.txt
Athens-Intro.txt
Athens-WhatToDo.txt
Athens-WhereToGo.txt
Barcelona-History.txt
Berlin-History.txt
Berlin-WhereToGo.txt
Boston-WhereToGo.txt
Canada-WhereToGo.txt
Crete-History.txt
Crete-WhereToGo.txt
```

Here, I used `find ./travel_guides -size -10` to search for files under travel_guides folder with the size smaller than 10 bytes. The purpose of this is to find the certain file size with limits so sometimes when my storage is not enough so I can find really large files to choose to delete them.

# List directories under specified path
Here I used `find -type d` to list all the directories under the certain folder.
Source: [Link](https://www.geeksforgeeks.org/grep-command-in-unixlinux/)
## Example 1:
### command:
```
grep -o "Amsterdam" Amsterdam-WhatToDo.txt
```
### output:
```
Amsterdam
Amsterdam
Amsterdam
Amsterdam
Amsterdam
Amsterdam
Amsterdam
Amsterdam
Amsterdam
Amsterdam
Amsterdam
Amsterdam
Amsterdam
Amsterdam
Amsterdam
Amsterdam
Amsterdam
Amsterdam
Amsterdam
Amsterdam
Amsterdam
Amsterdam
Amsterdam
Amsterdam
Amsterdam
Amsterdam
Amsterdam
Amsterdam
Amsterdam
Amsterdam
Amsterdam
```
Here I used `find ./travel_guides -type d` to search for the directory under travel_guides folder. And I got 2 directories under it. The purpose for this is to look every directory under certain folders so that I could know which directory I'm going into if I only remember certain keywords.
## Example 2:
### command:
```
grep -o "China" Beijing-History.txt
```
### output:
```
China
China
China
China
China
China
China
China
China
China
China
China
China
China
China
China
China
China
China
China
China
China
China
```
Here I used  find the directory under non-fiction directory. The purpose for this is to look every directory under certain folders so that I could know which directory I'm going into if I only remember certain keywords.

# Search files with case insensitive
Here I used `grep -i` to do the case-insensitive search. The key for this is the use of the -i option, which is only one character different from the -name option. The -i option is what makes the search case-insensitive.
Source: [Link](https://www.geeksforgeeks.org/grep-command-in-unixlinux/)
## Example 1:
### command:
```
grep -i "hotels" HandRHongKong.txt
```
### output:
```
Recommended Hotels
Hong Kong has some of the most luxurious hotels in the
Hotels listed below have full air-conditioning, offer 24-hour or
limited room service, and a wide range of facilities. Hong Kong hotels
occupancy, with bath or shower. Unless otherwise noted, hotels take all
```
Here I used `grep -i "hotels" HandRHongKong.txt` command to find all the matching string case-insensitive contains "hotels" no matter if they're upper or lower cases under berlitz1 folder in the given file "HandRHongKong.txt". So I got bunch of "Hotels" and "hotels" that are case-insensitive searches.
## Example 2:
### command:
```
grep -i "football" Amsterdam-WhatToDo.txt
```
### output:
```
Football (Soccer)
The Netherlands are football (soccer) crazy and Ajax is the Amsterdam team, one of the most successful in Europe over the last 30 years. They play at the Amsterdam Arena, a fine modern stadium, which is also used for other sporting events — but unfortunately it is almost impossible to obtain tickets for matches.
```
Here I used `grep -i "football" Amsterdam-WhatToDo.txt` command to find all the matching string case-insensitive contains "football" no matter if they're upper or lower cases under berlitz2 folder in the given file "Amsterdam-WhatToDo.txt". So I got bunch of "Football" and "football" that are case-insensitive searches.
