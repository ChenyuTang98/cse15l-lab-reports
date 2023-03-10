#  Displaying the count of number of matches
Using `grep -c` to find the number of lines that matches the given string/pattern.
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
Here I used `grep -c "Amsterdam" Amsterdam-WhatToDo.txt` to find the number of lines that matches "Amsterdam" in the given file "Amsterdam-WhatToDo.txt". This is good for me to know how often the certain words have been used and also helps me to catch the main point if I'm reading some articles.  
## Example 2:
### command:
```
grep -c "China" Beijing-History.txt
```
### output:
```
14
```

Here I used `grep -c "China" Beijing-History.txt` to find the number of lines that matches "China" in the given file "Beijing-History.txt". This is good for me to know how often the certain words have been used and also helps me to catch the main point if I'm reading some articles. 

# Display the file names that matches the pattern 
Here I used `grep -l` to display the files that contains the given string/pattern.
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
Here I used `grep -l "Beijing" *` to sdisplay the files that contains the given string "Beijing". Here it means as long as the files'contents contain the string "Beijing", then the file names would be displayed here. It is good for me to find the related articles containing the same keyword if I'm tring to do some researches.
## Example 2:
### command:
```
grep -l "Athens" *
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

Here I used `grep -l "Athens" *` to sdisplay the files that contains the given string "Athens". Here it means as long as the files'contents contain the string "Athens", then the file names would be displayed here. It is good for me to find the related articles containing the same keyword if I'm tring to do some researches.

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
The Netherlands are football (soccer) crazy and Ajax is the Amsterdam team, one of the most successful in Europe over the last 30 years. They play at the Amsterdam Arena, a fine modern stadium, which is also used for other sporting events ??? but unfortunately it is almost impossible to obtain tickets for matches.
```
Here I used `grep -i "football" Amsterdam-WhatToDo.txt` command to find all the matching string case-insensitive contains "football" no matter if they're upper or lower cases under berlitz2 folder in the given file "Amsterdam-WhatToDo.txt". So I got bunch of "Football" and "football" that are case-insensitive searches.

# Displaying only the matched pattern
Here I used `grep -o` to make the grep to display only the matched string by using the -o option.
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
Here I used `grep -o "Amsterdam" Amsterdam-WhatToDo.txt` to make the output only display the matches string "Amsterdam" by using the -o option in the given file "Amsterdam-WhatToDo.txt", instead of by default that grep displays the entire line which has the matched string. It is good when I only want to see the exactly matched word instead of dispalying the whole lines containing the word I'm looking for.
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
Here I used `grep -o "China" Beijing-History.txt` to make the output only display the matches string "China" by using the -o optionin the given file "Beijing-History.txt", instead of by default that grep displays the entire line which has the matched string. It is good when I only want to see the exactly matched word instead of dispalying the whole lines containing the word I'm looking for.
