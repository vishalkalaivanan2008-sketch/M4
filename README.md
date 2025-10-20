# EX-16-LEFT-SHIFT-OPERATION

## Name : VISHAL K
## Register Number : 25016496

## AIM
To write a C Program to perform the basic left shift operation for 44 integer number with 3 shifts.

## ALGORITHM
1.	Start the program.
2.	Assign values of a and b as 44 and 3.
3.	Use left shift operator (<<) and shift the value of a three times.
4.	Display the result.
5.	Stop the program.

## PROGRAM
```
#include <stdio.h>

int main() 
{
    
    int a = 44; 
    int b = 3;   
    int result = a << b;
    printf("The result of left shifting %d by %d is: %d\n", a, b, result);
    return 0;
}
```

## OUTPUT
<img width="1919" height="386" alt="image" src="https://github.com/user-attachments/assets/211beafb-ecf5-4587-b7a9-8ace1d640bc7" />



## RESULT
Thus the program to perform the basic left shift operation for 44 integer number with 3 shifts has been executed successfully.




 
 


# EX-17-TWO-NUMBERS-ARE-EQUAL-OR-NOT
## Name : VISHAL K
## Register Number : 25016496


## AIM

Write a C Program to check whether the two numbers are equal or not using simple if statement.

## ALGORITHM

1.	Start the program.
2.	Read two numbers.
3.	If first number is equal to second number, display both are equal.
4.	Otherwise display both are not equal.
5.	Stop the program.

## PROGRAM
```
#include <stdio.h>

int main() {
    
    int num1, num2;
    scanf("%d%d", &num1,&num2);
    if (num1 == num2) 
    {
        printf("Both numbers are equal.\n");
    } 
    else
    {
        printf("Both numbers are not equal.\n");
    }
    return 0;
}
```


## OUTPUT
<img width="1914" height="538" alt="image" src="https://github.com/user-attachments/assets/3f17b20f-3efa-4b33-9407-bd3ffa9180c5" />


           
## RESULT

Thus the program to check whether the two numbers are equal or not using simple if statement has been executed successfully
 
 


# EX-18-STRING-LOWERCASE-CONVERSION
## Name :VISHAL K
## Register Number : 25016496

## AIM
Write a C Program to convert the given string into lowercase.

## ALGORITHM
1.	Start the program.
2.	Read a string variable.
3.	Using tolower( ) function convert the given string into its lowercase.
4.	Display the result.
5.	Stop the program.

## PROGRAM
```
#include <stdio.h>
#include <ctype.h>  
int main()
{
    char str[100];
    fgets(str, sizeof(str), stdin);  
    for (int i = 0; str[i] != '\0'; i++) 
    {
        str[i] = tolower(str[i]);
    }
    printf("The string in lowercase is: %s\n", str);
    return 0;
}
```

## OUTPUT
<img width="1919" height="458" alt="image" src="https://github.com/user-attachments/assets/5b5889a8-8dec-4e05-8dcf-fec03af39f19" />





## RESULT
Thus the program to convert the given string into lowercase has been executed successfully
 
 


# EX-19-COUNT-OF-WORDS-IN-A-STRING

## Name : VISHAL K
## Register Number : 25016496

## AIM
Write a C Program to count the total number of words in a given string using do While loop.

## ALGORITHM
1.	Start the program.
2.	Read a string variable.
3.	Using for loop, inspect the string character by character.
4.	Whenever a space is encountered increment count by 1.
5.	Display the result.
6.	Stop the program.

## PROGRAM
```
#include <stdio.h>

int main() 
{
    char str[100];
    int i = 0, count = 0;
    printf("Enter a string: ");
    fgets(str, sizeof(str), stdin);  
    if (str[0] != '\0') 
    {  
        do {
            if (str[i] == ' ') 
            {
                count++;
            }
            i++;
        } 
        while (str[i] != '\0');
    }
    if (i > 1 && str[i-2] != ' ') 
    {
        count++;
    }
    printf("Total number of words: %d\n", count);
    return 0;
}
```

## OUTPUT
<img width="1919" height="805" alt="image" src="https://github.com/user-attachments/assets/bbc0e235-aa5e-4349-95b8-dbc72e83e62c" />





## RESULT
Thus the program to count the total number of words in a given string using do While loop has been executed successfully
 
 


# EX  -20 -COMPARING TWO STRINGS

## Name : VISHAL K
## Register Number : 25016496

## AIM
write a Program to compare two strings without using strcmp().
## ALGORITHM
Step 1: Start the program.
Step 2: Declare two character arrays c1 and c2 of size 100 to store the strings. Also, declare an integer variable
             flag and initialize it to 0, and i for indexing.      
Step 3: Read the first string c1 using scanf("%[^\n]", c1); — this reads input until a newline is encountered 
            (i.e., can include spaces).
Step 4: Read the second string c2 using scanf("%s", c2); — this reads input until a space or newline (i.e., no 
            spaces in the second string).
Step 5: Start comparing characters of both strings from index i = 0.
Step 6: Repeat the following while neither c1[i] nor c2[i] is '\0' (i.e., end of string):
•	If c1[i] is not equal to c2[i], set flag = 1.
•	Increment i by 1.
Step 7: After the loop, check the value of flag:
•	If flag == 0, print "strings are same".
•	Otherwise, print "strings are not same".
Step 8: End the program.

## PROGRAM
```
#include <stdio.h>
int main() 
{
    char c1[100], c2[100];
    int i = 0, flag = 0;
    scanf("%[^\n]", c1);
    scanf("%s", c2);
    do 
    {
        if (c1[i] != c2[i]) 
        {
            flag = 1;
            break; 
        }
        i++;
    } 
    while (c1[i] != '\0' || c2[i] != '\0'); 
    if (flag == 0) 
    {
        printf("Strings are same.\n");
    } 
    else 
    {
        printf("Strings are not same.\n");
    }
    return 0;
}
```


## OUTPUT
<img width="1632" height="835" alt="image" src="https://github.com/user-attachments/assets/48fb7766-c4cf-41f3-9f80-4d8331294da9" />

 

## RESULT
Thus the C Program to compare two strings without using strcmp() has been executed successfully.
