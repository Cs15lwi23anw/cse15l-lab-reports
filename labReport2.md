# Lab Report 2     

## Part 1         
This is my code for **StringServer**:             
![Image](cse15L_labReport2_part1code.png)             
        
This is an example of when I used /add-message:               
![Image](cse15L_labReport2_part1example1.png)               
Initially, **StringServer** runs its **main** method, which ask for the port number (4000) and pass it on to **Server's start** method along with a newly created **Handeler** object.   
**Server's start** method calls **Handler's handle** method to display and update the page.      
The **handle** method gets the URL's path and do different things based on the result.       
In the example, the path contains "/add-message" and its query has "s=hello" so it update the String **message** by adding "hello" on the next line.      
The String **message** is then displayed by **Server's start** method.      

             
This is another example of when I used /add-message:               
![Image](cse15L_labReport2_part1example2.png)                 
Initially, **StringServer** runs its **main** method, which ask for the port number (4000) and pass it on to **Server's start** method along with a newly created **Handeler** object.   
**Server's start** method calls **Handler's handle** method to display and update the page.      
The **handle** method gets the URL's path and do different things based on the result.       
In the example, the path contains "/add-message" and its query has "s=hi" so it update the String **message** by adding "hi" on the next line.      
The String **message** is then displayed by **Server's start** method.       
                         
                         
