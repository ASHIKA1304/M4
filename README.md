# EX-16-LEFT-SHIFT-OPERATION
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
int main() { 
int a = 44, b = 3; 
int result = a << b; 
printf("The result of left shifting %d by %d positions is: %d\n", a, b, result); 
return 0; 
}
```
## OUTPUT


![437953033-b2344627-f5fd-4d15-87a8-6baf063423c0](https://github.com/user-attachments/assets/21af7126-17b1-4c69-916b-3f85afef0454)


## RESULT
Thus the program to perform the basic left shift operation for 44 integer number with 3 shifts has been executed successfully.




 
 


# EX-17-TWO-NUMBERS-ARE-EQUAL-OR-NOT


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
int main()
{
    int a,b;
    scanf("%d%d",&a,&b);
    if (a==b)
    {
        printf("Number1 and Number2 are equal");
    }
    else
    {
        printf("Number1 and Number2 are not equal");
    }
}
```


## OUTPUT

![437953220-d355765d-4f68-47d9-ad4e-8e7535e3790f](https://github.com/user-attachments/assets/7ead1acf-a28a-4c50-b200-76864c9e522e)

           
## RESULT

Thus the program to check whether the two numbers are equal or not using simple if statement has been executed successfully
 
 


# EX-18-STRING-LOWERCASE-CONVERSION
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

int main() {
    char str[100];
    int i;
    scanf("%s", str);
    for (i = 0; str[i] != '\0'; i++) {
        str[i] = tolower(str[i]);
    }
    printf("Lower case String is:%s\n", str);

    return 0;
}
```

## OUTPUT

![437953353-e063db65-c254-43ad-905b-dfc7cb3c336c](https://github.com/user-attachments/assets/713efbf4-19e7-4f64-bd86-df60c873735a)


## RESULT
Thus the program to convert the given string into lowercase has been executed successfully
 
 


# EX-19-COUNT-OF-WORDS-IN-A-STRING
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
int i = 0, count = 1; 
fgets(str, sizeof(str), stdin); 
do { 
if (str[i] == ' ' || str[i] == '\t' || str[i] == '\n') { 
count++; 
} 
i++; 
} while (str[i] != '\0'); 
printf("Total number of words: %d\n", count); 
return 0;
}
```

## OUTPUT

![437953627-a3da5363-9527-482d-a91a-6166fd542b5a](https://github.com/user-attachments/assets/22e2b6f7-0914-4e46-a43c-d47bf072cea2)


## RESULT
Thus the program to count the total number of words in a given string using do While loop has been executed successfully
 
 


# EX  -20 -COMPARING TWO STRINGS
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
int main(){ 
    char c1[100], c2[100]; 
    int i = 0, flag = 0; 
    scanf("%[^\n]", c1); 
    scanf("%s", c2); 
    while (c1[i] != '\0' && c2[i] != '\0') 
    { 
        if (c1[i] != c2[i]) 
        { 
        flag = 1; 
        break; 
        } 
        i++; 
    } 
    if (c1[i] != '\0' || c2[i] != '\0') 
    { 
    flag = 1; 
    } 
    if (flag == 0) 
    { 
    printf("Strings are same.\n"); 
    }
    else {
    printf("Strings are not same.\n"); 
    } 
    return 0; 
}
```


## OUTPUT

 ![437953922-9029fb9b-e64f-4b1d-ba8b-8cca89fa7040](https://github.com/user-attachments/assets/e2944da5-74f0-44db-98f6-375294195f4f)


## RESULT
Thus the C Program to compare two strings without using strcmp() has been executed successfully.

