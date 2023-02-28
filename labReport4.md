# Lab Report 4
## Step 4: Log into ieng6    
![Image](labReport4step4.png)  
Keys pressed: `ssh cs15lwi23anw@ieng6.ucsd.edu` then `<enter>`                     
Explaination: I typed ssh then my username cs15lwi23anw@ieng6 followed by .ucsd.edu to sign in to my ieng6 account.           
                          
## Step 5: Clone your fork of the repository from your Github account    
![Image](labReport4step5.png)  
Keys pressed: `git clone<space>` then copy and pasted the link from the forked directory then `<enter>`    
Explaination: git clone is the command used to clone a path from gitHub. I typed git clone then entered the link from the forked directory to clone the directory to mine ieng6 account.                 
                        
## Step 6: Run the tests, demonstrating that they fail    
![Image](labReport4step6.png)  
Copy and paste the javac comand from the instruction. Then press `<enter>`          
Copy and paste the java comand from the instruction. Then add `<space>ListExamplesTests<enter>`         
Explaination: I copied and pasted the command used to compile and run JUnits provided to us in the instructions. The complie command don't need anny adjustment, but the run command does. I added the test file I wanted to run at the end of the command. At the moment, ListExamples.java has a bug so the test did not pass.         
                           
## Step 7: Edit the code file to fix the failing test    
![Image](labReport4step7.png)  
Keys pressed: `nano ListExamples.java` then hold `<down>` till you at the end then `<up>`x7 then `<right>`x12 then `<backspace>` then `2`         
then `Ctrl+O` then`enter` then `Ctrl+X`          
Explaination: I ran the command nano on the file ListExamples.java to open and edit its content. I moved the curser to one time the varible "index1" was called and change it to "index2" then I pressed <Ctrl+O> and <enter> to save the change and <Ctrl+X> to exit the nano window.             
                        
## Step 8: Run the tests, demonstrating that they now succeed    
![Image](labReport4step8.png)  
Keys pressed: `<up>`x3 `<enter>`          
Keys pressed: `<up>`x2 `<enter>`          
Explaination: I pressed <up> three times to acces the complie command I used previously. After running the compile comand, I pressed <up> two times to acces ListExamplesTests.java's run command previously used by me and pressed <enter> to run it. This time, the tests passed since I used the command nano to fix the bug.     
                             
## Step 9: Commit and push the resulting change to your Github account    
![Image](labReport4step9.png)  
Keys pressed: `git add ListExamples.java` then `<enter>` then `git commit -m "fix"` then `<enter>` then `git push origin main` then `<enter>`              
Explaination: I used the command git add to add ListExamples.java to the list of things I want to save to GitHub. I then used the commit command to finalize the list of changes I want to save to GitHub. I then used the push command to push all the changes I finalized to the forked file on GitHub.
