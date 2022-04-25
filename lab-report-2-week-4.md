# __Lab Report 2__
---
## Josue Martinez 

A16943817
#### CSE 15L
####  4/24/2022
## First Code Change
![FirstChange](/R2Images/FirstChange.png)

[Link to test file](https://github.com/josueemartinezz/markdown-parser/blame/main/test-file.md)

![FirstSymptom](/R2Images/FirstSymptom.png)

The bug is that the program reads all lines and looks for when to begin the search via the "[" character, but has no outline to follow when there's no occurence of the character. So when there's an extra, blank line as expressed in the failure-inducing input file, "test-file.md", the program runs forever; or atleast until it ouputs an "OutOfMemory" error and shows the symptom of an infinite loop. However, my attempt was unsuccesful as I used the wrong approach to check if there's nothing ahead of current index.

## Second Code Change
![SecondChange](/R2Images/SecondChange.png)

[Link to test file](https://github.com/josueemartinezz/markdown-parser/blame/main/newFile.md)

![SecondSymptom](/R2Images/SecondSymptom.png)

My next change attempted to account address the same bug of an empty line by trying to break the while loop to check if there's no more possible links to be found. This way, I could fix the symptom of the infinite loop. I did so by using String's `is.Empty()` method to assert there's no next link. Next, the failure inducing input was still the "test-file", but I rationalized a new file that tested the bug with an expected input with no extra line would not induce a failure (newFile.md).

## Third Code Change
![ThirdChange](/R2Images/ThirdChange.png)

[Link to test file](https://github.com/josueemartinezz/markdown-parser/blame/main/newFile2.md)

![ThirdSymptom](/R2Images/ThirdSymptom.png)

When a completely empty file (newFile2.md) is used as an input in the current program, it falls victim to a bug that isn't caught by the testing changes covered. Thus, it gives the usual symptom of a OutOfMemory error that equates to the infinite loop. Thereby, my fix is to change the print statement in the main method to check if the getLinks() method returns list contains nothing using `is.Empty()` to return an empty line.

##  <center>THANK YOU FOR VISITING</center>