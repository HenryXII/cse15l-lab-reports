# Week 4 Lab Report
### bug fix 1
![Fix 1](fix1.png)
The linke to the failure-inducing input:
[test file 2](https://github.com/HenryXII/markdown-parse/blob/main/test-file2.md)

The corresponding symptom
![Symp 1](symp1.png)

The symptom shows a out of memory error, which imply that the program goes into an infinite loop. When I check the code I can see that it can only end the loop if a close paren is at the end of the input file, which is not the case for test file 2.
### bug fix 2
![Fix 2](fix2.png)
The linke to the failure-inducing input:
[test file 3](https://github.com/HenryXII/markdown-parse/blob/main/test-file3.md)

The corresponding symptom
![Symp 2](symp2.png)

The symptom is that the link of an image also got printed. This happened because there is an image link in the input file and the code had a bug that it couldn't distinguish the difference between an image link or a normal link.
### bug fix 3
![Fix 3](fix3.png)
The linke to the failure-inducing input:
[test file 4](https://github.com/HenryXII/markdown-parse/blob/main/test-file4.md)

The corresponding symptom
![Symp 3](symp3.png)

The symptom is that the link at the beginning is not getting printed. The input has a link at the beginning. The bug is created by the fix to previous problem, apparently a link at the beginning got treated like an image.