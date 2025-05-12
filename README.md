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

void calculateEMI(float principal, float rate, int months) {
    float emi, amt;
    float r = rate / 100 / 12;  // Monthly interest rate
    float t = months;  // Number of months

    amt = (principal * pow(1 + r, t) * r) / (pow(1 + r, t) - 1);

    printf("EMI: %.2f\n", amt);
}

int main() {
    float principal, rate;
    int months;

    scanf("%f", &principal);
    scanf("%f", &rate);
    scanf("%d", &months);

    calculateEMI(principal, rate, months);

    return 0;
}
```

## OUTPUT
![image](https://github.com/user-attachments/assets/3d2060c1-89bf-4ebb-ba0d-5828aff392c8)





## RESULT

Thus the program to prepare EMI calculator using function without return type with arguments has been executed successfully
 
 <hr>


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
    int n = 6;
    int firstTerm = 0, secondTerm = 1, nextTerm;

    printf("Fibonacci Series: ");
    
    for (int i = 1; i <= n; i++) {
        if (i == 1) {
            printf("%d ", firstTerm);
            continue;
        }
        if (i == 2) {
            printf("%d ", secondTerm);
            continue;
        }
        
        nextTerm = firstTerm + secondTerm;
        printf("%d ", nextTerm);
        
        firstTerm = secondTerm;
        secondTerm = nextTerm;
    }

    printf("\n");

    return 0;
}
```
## OUTPUT


![image](https://github.com/user-attachments/assets/65b85234-839c-40ec-93d7-a1f87b944676)






## RESULT
Thus the program to generate the Fibonacci series for the value 6 has been executed successfully.
 
 <hr>


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
    int n;

    scanf("%d", &n);

    int arr[n];

    for (int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }

    printf("%d\n", arr[n-1]);

    return 0;
}
```
## OUTPUT
![image](https://github.com/user-attachments/assets/e71902d1-a6f5-4457-8dfc-9d40fa04cdc6)








## RESULT
Thus the program to read n elements as input and print the last element of the array has been executed successfully.
 
 <hr>


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
#include <stdio.h>
```c
int main() {
    int n, count = 0;

    scanf("%d", &n);

    int arr[n];

    for (int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }

    for (int i = 0; i < n; i++) {
        if (arr[i] > 0) {
            count++;
        }
    }

    printf("Total positive elements: %d\n", count);

    return 0;
}
```

## OUTPUT

![image](https://github.com/user-attachments/assets/8fff035e-d24c-4e8f-9c22-be2fb63ad96c)




## RESULT
Thus the program to count total number of positive elements in an array has been executed successfully.


<hr>


 
 


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
    int n;

    scanf("%d", &n);

    int arr[n];

    for (int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }

    for (int i = 0; i < n; i++) {
        if (arr[i] % 2 == 0) {
            arr[i] = 'E';
        }
    }

    for (int i = 0; i < n; i++) {
        if (arr[i] == 'E') {
            printf("'E' ");
        } else {
            printf("%d ", arr[i]);
        }
    }

    printf("\n");

    return 0;
}
```
## Output:
 
![image](https://github.com/user-attachments/assets/c504b4e0-834d-491b-81f5-fc2d0297db6b)


## Result:

Thus, the program to replace all even elements with 'E' in one dimensional array was verified successfully.


<hr>
