# Using -name to search for files with a specified name
```
find ./Castro  -name "*.txt"
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

```
find ./Rybczynski -name "*.txt"
./Rybczynski/ch2.txt
./Rybczynski/ch3.txt
./Rybczynski/ch1.txt
```
[Link](https://www.geeksforgeeks.org/find-command-in-linux-with-examples/)
Here I used find -name *.txt to find files with the certain pattern of ".txt" files. I looked into folders of Castro and Rybczynski. This command is good to find the certain pattern, especially when sometimes we only need .txt files, or .md files, etc.

# Using -size to search for files with a specified size
```
find ./berlitz2 -size +100                              
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

```
find ./travel_guides -size -10 
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
[Link](https://www.redhat.com/sysadmin/linux-find-command)
Here I used find -size +100 to search for files under berlitz2 folder with the size greater than 100 bytes, and find -size -10 to search for files under travel_guides folder with the size smaller than 10 bytes. The purpose of this is to find the certain file size with limits so sometimes when my storage is not enough so I can find really large files to choose to delete them.

# Using -type d to search for files of a specified type(here is directory)
```
find ./travel_guides -type d
./travel_guides
./travel_guides/berlitz1
./travel_guides/berlitz2
```

```
find ./non-fiction -type d
./non-fiction
./non-fiction/OUP
./non-fiction/OUP/Berk
./non-fiction/OUP/Abernathy
./non-fiction/OUP/Rybczynski
./non-fiction/OUP/Kauffman
./non-fiction/OUP/Fletcher
./non-fiction/OUP/Castro
```
[Link](https://www.redhat.com/sysadmin/linux-find-command)
Here I used find -type d to search for the directory under travel_guides folder and find the directory under non-fiction directory. The purpose for this is to look every directory under certain folders so that I could know which directory I'm goinging into if I only remember certain keywords.

# Using -name ".txt" to search a file with specific name.
```
find ./berlitz2 -name "Beijing-History.txt"
./berlitz2/Beijing-History.txt
```

```
find ./Kauffman -name "ch4.txt"              
./Kauffman/ch4.txt
```
[Link](https://www.geeksforgeeks.org/find-command-in-linux-with-examples/)
Here I used find -name "Beijing-History.txt" to find the this file I want under berlitz2 folder and fine -name "ch4.txt" to find this file from Kauffman folder. The purpose for this is that when sometimes I forgot where exactly is the specific file I'm looking for when I can only remember the file name.
