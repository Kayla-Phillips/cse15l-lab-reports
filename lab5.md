# Debugging Scenario
## Original Post
Title: Grading Script Issues

Hi everyone,
I'm having some issues when I run my grading script. The correct method is failing one of my tests. When I run the grading script with the corrected methods, I get an error saying that the recursion level has been exceeded. I'm not sure where I am using recursion. The error occurs on line 56 I think because one of the variable is a word instead of a number. I followed the same lines of code as we did in class that worked. If anyone can help me, it would be greatly appreciated!

![Description](file)

## TA Response
Can you try using cat to see the junit output? You may also want to try using echo on the relevant variables to see where the issue is happening.

## Student Response
!(Image.png)[]
The junit output looks as expected, but the variables are all wrong. I think the first variable that has the wrong value is `linecount` which should be 5 based on the junit output but is 20. This means that the `wc` command is not properly getting the correct number of lines. After doing research on the `wc` commands, I realized that I was using `-L` instead of `-l`.



# Reflection
