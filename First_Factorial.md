
### First_Factorial 

Tags: recursion, math fundamentals | Difficulty: Easy
Challenge
Have the function FirstFactorial(num) take the num parameter being passed and return the factorial of it. 
For example: if num = 4, then your program should return (4 * 3 * 2 * 1) = 24. 
For the test cases, the range will be between 1 and 18 and the input will always be an integer. 

Sample Test Cases
Input:4
Output:24

Input:8
Output:40320

View Hint

```
import java.util.*; 
import java.io.*;

class Main {  
  public static int FirstFactorial(int num) { 
    if (num == 0)    
        return 1;    
    else    
        return(num * FirstFactorial(num-1));
  }
  
  public static void main (String[] args) {  
    // keep this function call here     
    Scanner s = new Scanner(System.in);
    System.out.print(FirstFactorial(s.nextLine())); 
  }   
  
}
```
<center>OR</center>

```
import java.util.*; 
import java.io.*;

class Main {  
  public static int FirstFactorial(int num) { 
    int fact=1;
	for(int i=num;i>0;i--){
		fact=fact*i;
	}
	return fact;
  }
  
  public static void main (String[] args) {  
    // keep this function call here     
    Scanner s = new Scanner(System.in);
    System.out.print(FirstFactorial(s.nextLine())); 
  }   
  
}
```
