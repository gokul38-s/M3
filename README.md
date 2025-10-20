# EX-11-EMI-CALCULATOR

## AIM

To write a program to prepare EMI calculator using function without return type and with arguments.

## ALGORITHM

1.	Start the program.
2.	Read principal amount, rate of interest and months.
3.	Pass these values as arguments to function.
4.	Calculate EMI using the formula, amt=(prpow(1+r,t))/(pow(1+r,t)-1)
5.	Display the result.
6.	Stop the program.

## PROGRAM
```c
#include <stdio.h>
#include <math.h>

double calculateEMI(double principal, double rate, int months) {
    double r = rate / (12 * 100);
    double t = months;
    double amt = (principal * r * pow(1 + r, t)) / (pow(1 + r, t) - 1);
    return amt;
}

int main() {
    double principal, rate, emi;
    int months;
    scanf("%lf %lf %d", &principal, &rate, &months);
    emi = calculateEMI(principal, rate, months);
    printf("%.2lf\n", emi);
    return 0;
}
```

## OUTPUT
<img width="1630" height="782" alt="c_11" src="https://github.com/user-attachments/assets/63b2548e-6c99-4468-a537-26bb415cf8db" />





## RESULT

Thus the program to prepare EMI calculator using function without return type with arguments has been executed successfully
 
 


# EX-12-FIBONACCI-SERIES
## AIM
To write a C program to generate the Fibonacci series for the value 6.

## ALGORITHM
1.	Start the program.
2.	Read number of terms to display.
3.	Add the previous two terms and store it in new term.
4.	Assign 2nd term to 1st term and 3rd term to 2nd term.
5.	Repeat steps 3 and 4 n number of times.
6.	Display the result.
7.	Stop the program.

## PROGRAM
```c
#include <stdio.h>

int main() {
    int n, i, t1 = 0, t2 = 1, nextTerm;
    scanf("%d", &n);
    for (i = 1; i <= n; i++) {
        printf("%d ", t1);
        nextTerm = t1 + t2;
        t1 = t2;
        t2 = nextTerm;
    }
    printf("\n");
    return 0;
}
```
## OUTPUT
<img width="1627" height="782" alt="C_12" src="https://github.com/user-attachments/assets/9b10b99b-5bc3-4dcb-88f1-785e03a627da" />








## RESULT
Thus the program to generate the Fibonacci series for the value 6 has been executed successfully.
 
 


# EX-13-ONE-DIMENSIONAL-ARRAY
## AIM
To write a C program to read n elements as input and print the last element of the array.

## ALGORITHM
1.	Start the program.
2.	Read a variable.
3.	Read the array values n number of times.
4.	Print the last element.
5.	Stop the program.

## PROGRAM
```c
#include <stdio.h>

int main() {
    int n, i;
    scanf("%d", &n);
    int arr[n];
    for (i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }
    printf("%d\n", arr[n-1]);
    return 0;
}

```
## OUTPUT
<img width="1626" height="778" alt="C_13" src="https://github.com/user-attachments/assets/94cd7388-f4ef-4da9-b0a6-5028e558f626" />









## RESULT
Thus the program to read n elements as input and print the last element of the array has been executed successfully.
 
 


# EX-14-POSITIVE-ARRAY-ELEMENTS
## AIM
To write a C Program to count total number of positive elements in an array.

## ALGORITHM
1.	Start the program.
2.	Read a variable.
3.	Read the array values n number of times.
4.	If the array value can be divided by 2 then increment count by 1.
5.	Display result.
6.	Stop the program.

## PROGRAM
```c
#include <stdio.h>

int main() {
    int n, i, count = 0;
    scanf("%d", &n);
    int arr[n];
    for (i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
        if (arr[i] % 2 == 0)
            count++;
    }
    printf("%d\n", count);
    return 0;
}
```
## OUTPUT
<img width="1627" height="781" alt="C_14" src="https://github.com/user-attachments/assets/1091c7c9-f5a0-483c-b643-f06c7dce41c4" />





## RESULT
Thus the program to count total number of positive elements in an array has been executed successfully.





 
 


# EX -15 - Replace All Even Elements With 'E' In One Dimensional Array

## Aim:
To write a C program to replace all even elements with 'E' in one dimensional array

## Algorithm:
1.	Input the array:
  Read the size of the array.
  Input the elements of the array.
2.	Iterate through the array:
 	For each element of the array, check if the element is even (i.e., if the element modulo 2 equals 0).
3.	Replace even elements with 'E':
     If an element is even, replace that element with the character 'E'.
4.	Output the updated array:
 Print the updated array after replacements.

## Program:
```c
#include <stdio.h>

int main() {
    int n, i;
    scanf("%d", &n);
    char arr[n];
    int temp;
    for (i = 0; i < n; i++) {
        scanf("%d", &temp);
        if (temp % 2 == 0)
            arr[i] = 'E';
        else
            arr[i] = temp + '0';
    }
    for (i = 0; i < n; i++) {
        printf("%c ", arr[i]);
    }
    printf("\n");
    return 0;
}
```
## Output:
<img width="1627" height="785" alt="C_15" src="https://github.com/user-attachments/assets/18a3d378-70eb-4047-9f5d-d0895fafefea" />
 


## Result:

Thus, the program to replace all even elements with 'E' in one dimensional array was verified successfully.



