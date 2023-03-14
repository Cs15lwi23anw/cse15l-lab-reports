# Lab Report 3
                 
## find /path -name filename                   
I found all the information from this blog [Link](https://www.stackscale.com/blog/find-command-linux/)                   
This command take in a path and a file name then give out all files with the same name in the given directory and all its sub-directories.             
This command is usefull to find things in your data structure by name. As an example. if you forgot where you saved you file, you can find it with this command by entering the file's name and you home directory. This command would output the path from the home directory to your file.               
```
[cs15lwi23anw@ieng6-201]:~:147$ find ./skill-demo1-data/written_2 -name ch1.txt
./skill-demo1-data/written_2/non-fiction/OUP/Abernathy/ch1.txt
./skill-demo1-data/written_2/non-fiction/OUP/Berk/ch1.txt
./skill-demo1-data/written_2/non-fiction/OUP/Fletcher/ch1.txt
./skill-demo1-data/written_2/non-fiction/OUP/Kauffman/ch1.txt
./skill-demo1-data/written_2/non-fiction/OUP/Rybczynski/ch1.txt
```
In the code block, I found every file with the name "ch1.txt" in the directory **written_2**.                 
```
[cs15lwi23anw@ieng6-201]:~:148$ find ./skill-demo1-data/written_2 -name ch2.txt
./skill-demo1-data/written_2/non-fiction/OUP/Abernathy/ch2.txt
./skill-demo1-data/written_2/non-fiction/OUP/Berk/ch2.txt
./skill-demo1-data/written_2/non-fiction/OUP/Fletcher/ch2.txt
./skill-demo1-data/written_2/non-fiction/OUP/Rybczynski/ch2.txt
```
In the code block, I found every file with the name "ch2.txt" in the directory **written_2**. 
