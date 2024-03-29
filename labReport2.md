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
                         
                         
## Part 2       
The bug I chose is the reverse method. Instead of returning the given array in reverse order, the reverse method returns an array of zero's in the size of the given array.             
* A failure-inducing input for the buggy program, as a JUnit test and any associated code (write it as a code block in Markdown)          
```
@Test
  public void testReversed2() {
    int[] input1 = {1, 2};
    ArrayExamples.reversed(input1);
    assertArrayEquals(new int[]{2, 1}, ArrayExamples.reversed(input1));
  }
```
                
* An input that doesn’t induce a failure, as a JUnit test and any associated code (write it as a code block in Markdown)          
```
@Test
  public void testReversed() {
    int[] input1 = { };
    assertArrayEquals(new int[]{ }, ArrayExamples.reversed(input1));
  }
```
                   
* The symptom, as the output of running the tests (provide it as a screenshot of running JUnit with at least the two inputs above)          
![Image](cse15L_labReport2_part2example1.png)           
          
* The bug, as the before-and-after code change required to fix it (as two code blocks in Markdown)           

Before:          
```
static int[] reversed(int[] arr) {
    int[] newArray = new int[arr.length];
    for(int i = 0; i < arr.length; i += 1) {
      arr[i] = newArray[arr.length - i - 1];
    }
    return arr;
  }
```
After:                 
```
static int[] reversed(int[] arr) {
    int[] newArray = new int[arr.length];
    for(int i = 0; i < arr.length; i += 1) {
      newArray[i] = arr[arr.length - i - 1];
    }
    return newArray;
  }
```
                     
* Briefly describe why the fix addresses the issue.           
In the original code, the reverse method created an empty array with the size of the input array. It then copy the empty array in reverse order on to the array it plans to return, then return the array which has become empty. In the new code, I saved the input array in reverse order on to the newly created array and return an array with the data being reversed.                   
                      
                                 
## Part 3  
In a couple of sentences, describe something you learned from lab in week 2 or 3 that you didn’t know before.                            
                    
Before the lab, I did not know how to host my own website and make updates to it. It was very fun and rewarding to learn a new and usefull skill such as this. It feels like I'm making a small part of my own version of Twitter.                    
