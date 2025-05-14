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
#include<math.h>
void emi(float p,float r,float n)
{
    r=r/(100*12);
    n=n*12;
    float emi=p*r*pow(1+r,n)/(pow(1+r,n)-1);
    printf("Monthly EMI is= %.3f",emi);
}
int main()
{
    float p,n,r;
    scanf("%f %f %f",&p,&r,&n);
    emi(p,r,n);
}


```


## OUTPUT

![Screenshot 2025-04-27 150352](https://github.com/user-attachments/assets/d15b6f9d-3da0-41ff-a814-e3ad3063745f)



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
#include<stdio.h>
void fibonacci(int n)
{
    int temp=-1,a=1,b=0;
    for (int i=1;i<=n;i++)
    {
        temp=a+b;
        a=b;
        b=temp;
        printf("%d ",a);
       
    }
}
int main()
{
    int num;
    scanf("%d",&num);
    fibonacci(num);
}

```

## OUTPUT

![Screenshot 2025-04-27 150452](https://github.com/user-attachments/assets/cdc27f77-0a25-4bf3-8a0e-7ef322435607)




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
#include<stdio.h>
int main()
{
    int n,i;
    scanf("%d",&n);
    int arr[n];
    for (i=0;i<n;i++)
    {
        scanf("%d",&arr[i]);
    }
    if (n>0) printf("%d\n",arr[n-1]);
    else printf(" ");   
}
```

## OUTPUT

![Screenshot 2025-04-27 150543](https://github.com/user-attachments/assets/34851039-ad90-4502-b85c-dc0c5777a8a6)



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
#include<stdio.h>
int main()
{
    int n,i;
    scanf("%d",&n);
    int arr[n],count_pos=0,count_neg=0;
    for (i=0;i<n;i++)
    {
        scanf("%d",&arr[i]);
        if (arr[i]>0) count_pos++;
        else count_neg++;
    }
    printf("count  of positive numbers  in array: %d\n",count_pos);
    printf("count  of negative numbers  in array: %d",count_neg);
}

```

## OUTPUT
![Screenshot 2025-04-27 150632](https://github.com/user-attachments/assets/cfca22c6-72b5-45c1-bfa6-52d15c754121)

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
    int n;
    scanf("%d", &n);

    int arr[n];
    for (int i = 0; i < n; i++) {
        scanf("%d", &arr[i]);
    }

    for (int i = 0; i < n; i++) {
        if (arr[i] % 2 == 0) {
            arr[i] = 'E';  // Replacing even numbers with 'E'
        }
    }

    for (int i = 0; i < n; i++) {
        if (arr[i] == 'E') {
            printf("E ");
        } else {
            printf("%d ", arr[i]);
        }
    }

    return 0;
}
```
## Output:
![WhatsApp Image 2025-04-27 at 15 09 19_29145594](https://github.com/user-attachments/assets/8069572d-0579-4e34-acf8-50030e3aea5f)

## Result:

Thus, the program to replace all even elements with 'E' in one dimensional array was verified successfully.



