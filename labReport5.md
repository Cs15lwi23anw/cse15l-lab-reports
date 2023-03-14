# Lab Report 5
                 
## grep -c PATTERN filename                   
I found all the information from this blog [Link](https://www.geeksforgeeks.org/grep-command-in-unixlinux/)                   
This command takes in a pattern and a file name and output the number of lines that contains the pattern that was input.             
This command is usefull for keeping track of how often a word pops up in your file. For example, you saved a list of students in your class in a text file. On every line is a different student. If you want to find out how many students in your class has the name "Steve", you can find that out with this command. You can input the word "Steve" and the file's name. The command you output the number of lines that has the word "Steve", which is also the number of students with the name Steve in your class.                 
```
[cs15lwi23anw@ieng6-201]:Abernathy:284$ grep -c "the" ch1.txt 
68

```
In the code block, I found the number of lines that has the word "the" in the file ch1.txt.                 
```
[cs15lwi23anw@ieng6-201]:Abernathy:285$ grep -c "in" ch1.txt
71

```
In the code block, I found the number of lines that has the word "in" in the file ch1.txt. 

## grep -i PATTERN filename                   
I found all the information from this blog [Link](https://www.geeksforgeeks.org/grep-command-in-unixlinux/)                   
This command takes in a pattern and a file name and output all lines that contains the pattern that was input while ignoring what case the word is in.             
This command is usefull for keeping track of how often a word pops up in your file while not take in accout the case. For example, you saved a list of students in your class in a text file. On every line is a different student. If you want to find out how many students in your class has the letter "s" in their name. You can find that out with this command. You can input the letter "s" and the file's name. The command you output all the lines that has the letter "s" while ignoring the case of the letter, which is also the number of students with the letter "s" in their name.                 
```
[cs15lwi23anw@ieng6-201]:Abernathy:308$ grep -i -c "new york" ch1.txt
3

```
In the code block, I found all the lines that has the word "new york" in the file ch1.txt while ignoring what case the word is in with the command -i. But instead of outputing all the lines, I only output the number of lines by using the command -c in conjunction.                 
```
[cs15lwi23anw@ieng6-201]:Abernathy:309$ grep -i -c "bond" ch1.txt
6

```
In the code block, I found all the lines that has the word "bond" in the file ch1.txt while ignoring what case the word is in with the command -i. But instead of outputing all the lines, I only output the number of lines by using the command -c in conjunction. 
