# Lab Report 3
                 
**find /path -name filename**                   
I found all the information from this blog [Link](https://www.stackscale.com/blog/find-command-linux/)                   
This command is usefull to find things in your data structure.               
```
[cs15lwi23anw@ieng6-201]:~:147$ find /home/linux/ieng6/cs15lwi23/cs15lwi23anw/skill-demo1-data/written_2 -name ch1.txt
/home/linux/ieng6/cs15lwi23/cs15lwi23anw/skill-demo1-data/written_2/non-fiction/OUP/Abernathy/ch1.txt
/home/linux/ieng6/cs15lwi23/cs15lwi23anw/skill-demo1-data/written_2/non-fiction/OUP/Berk/ch1.txt
/home/linux/ieng6/cs15lwi23/cs15lwi23anw/skill-demo1-data/written_2/non-fiction/OUP/Fletcher/ch1.txt
/home/linux/ieng6/cs15lwi23/cs15lwi23anw/skill-demo1-data/written_2/non-fiction/OUP/Kauffman/ch1.txt
/home/linux/ieng6/cs15lwi23/cs15lwi23anw/skill-demo1-data/written_2/non-fiction/OUP/Rybczynski/ch1.txt
```
In the code block, I found every file with the name "ch1.txt" in the directory **written_2**.                 
```
[cs15lwi23anw@ieng6-201]:~:148$ find /home/linux/ieng6/cs15lwi23/cs15lwi23anw/skill-demo1-data/written_2 -name ch2.txt
/home/linux/ieng6/cs15lwi23/cs15lwi23anw/skill-demo1-data/written_2/non-fiction/OUP/Abernathy/ch2.txt
/home/linux/ieng6/cs15lwi23/cs15lwi23anw/skill-demo1-data/written_2/non-fiction/OUP/Berk/ch2.txt
/home/linux/ieng6/cs15lwi23/cs15lwi23anw/skill-demo1-data/written_2/non-fiction/OUP/Fletcher/ch2.txt
/home/linux/ieng6/cs15lwi23/cs15lwi23anw/skill-demo1-data/written_2/non-fiction/OUP/Rybczynski/ch2.txt
```
In the code block, I found every file with the name "ch2.txt" in the directory **written_2**.                 
                              
**find /path -mtime 1**                            
I found all the information from this blog [Link](https://www.stackscale.com/blog/find-command-linux/)                  
This command is useful since it can help you find your progress. It helps you find what you modified in the data structure and when.
```
[cs15lwi23anw@ieng6-201]:~:168$ find -mtime -1
./.cache/abrt
./.cache/abrt/lastnotification
./.modulesbegenv
./.motd
```
In the code block, I found every file that was modified in the past day in the current working directory.                 
```
[cs15lwi23anw@ieng6-201]:~:173$ find -mtime -2
.
./.cache/abrt
./.cache/abrt/lastnotification
./.modulesbegenv
./.motd
./some-files.txt
```
In the code block, I found every file that was modified in the past 2 day in the current working directory. You can see the file "some-files.txt" listed since I made it 2 days ago.               
                       
**find -maxdepth 3 /path**                                     
I found all the information from this blog [Link](https://www.stackscale.com/blog/find-command-linux/)                  
This command is useful since it can help you identify the data structure near the path you want. It can be adjusted to show more or less information based on how many levels you want to see.      
```
[cs15lwi23anw@ieng6-201]:~:185$ find -maxdepth 1
.
./.bash_profile
./.bashrc
./.cshrc
./.kshrc
./.locallogin
./.login
./.procmailrc
./.profile
./.zprofile
./.zshenv
./.zshrc
./.cache
./.config
./.modulesbegenv
./.local
./perl5
./.motd
./.bash_history
./skill-demo1-server
./.pki
./skill-demo1-data
./some-files.txt
```
In the code block, I found every file that is in the current directory or 1 level deeper from the current directory.                 
```
[cs15lwi23anw@ieng6-201]:~:186$ find -maxdepth 2
.
./.bash_profile
./.bashrc
./.cshrc
./.kshrc
./.locallogin
./.login
./.procmailrc
./.profile
./.zprofile
./.zshenv
./.zshrc
./.cache
./.cache/abrt
./.config
./.config/abrt
./.modulesbegenv
./.local
./.local/share
./perl5
./.motd
./.bash_history
./skill-demo1-server
./skill-demo1-server/.git
./skill-demo1-server/.gitignore
./skill-demo1-server/FileServer.java
./skill-demo1-server/FileServerTests.java
./skill-demo1-server/Server.java
./skill-demo1-server/lib
./skill-demo1-server/test-data
./skill-demo1-server/FileHelpers.class
./skill-demo1-server/Handler.class
./skill-demo1-server/URLHandler.class
./skill-demo1-server/FileServer.class
./skill-demo1-server/FileServerTests.class
./skill-demo1-server/ServerHttpHandler.class
./skill-demo1-server/Server.class
./.pki
./.pki/nssdb
./skill-demo1-data
./skill-demo1-data/.git
./skill-demo1-data/written_2
./skill-demo1-data/find-results.txt
./skill-demo1-data/grep-results.txt
./some-files.txt
```
In the code block, I found every file that is in the current directory or 1 to 2 levels deeper from the current directory.          
                                                         
**find /path -size +100k**                                    
I found all the information from this blog [Link](https://www.stackscale.com/blog/find-command-linux/)                  
This command is useful since it can help you identify files based on the size you're looking for.                   
```
[cs15lwi23anw@ieng6-201]:~:198$ find -size +300k
./skill-demo1-server/.git/objects/pack/pack-cd15105c095bef3eabe7ab46217abba163043e6c.pack
./skill-demo1-server/lib/junit-4.13.2.jar
./skill-demo1-data/.git/objects/pack/pack-b98cb6a4ca64cc7b2944f0fa07d3e03927d66064.pack
```
In the code block, I found every file that is bigger thank 300 kilobyte in the current directory or deeper.          
```
[cs15lwi23anw@ieng6-201]:~:199$ find -size +400k
./skill-demo1-data/.git/objects/pack/pack-b98cb6a4ca64cc7b2944f0fa07d3e03927d66064.pack
```
In the code block, I found every file that is bigger thank 400 kilobyte in the current directory or deeper.  

