# <center>Lab Report 5</center>
---
## Josue Martinez 

A16943817
#### CSE 15L
####  6/10/2022

## <center>Finding Tests With Different Results</center>
I used 'vimdiff' to go through several tests in the `/testfiles` directory manually.
![vimDiff](/R5images/vimdiff.png)
## <center>Test File Link</center>
[Link Address](https://github.com/josueemartinezz/markdown-parser/blob/main/test-file.md)

## <center>Test One (108.html.test)</center>

### Implementation Results 
I'd argue the given implementation from the lab is the correct one for this test file. Our implementation rolls over the '\<code>' portion of the file, whilst the provided implementation seemed to result in the expected links.
### Actual vs Expected Outputs
![testOne](/R5images/testTwo.png)
## <center>Test Two (118.html.test)</center>
### Implementation Results
Considering the given implementation from our lab 9 contains several more checks for the tests that our group's implementation didn't, the better one is this provided program. Our implementation fails to even find a the correct assignment of files to assert that any link can be found, extracted and ran through our implementation.
### Actual vs Expected Outputs
![testTwo](/R5images/testOne.png)
# <center>Thank you for visiting!</center>