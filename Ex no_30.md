# EX 30 C program to add two integer elements in an array using realloc() and that array already has three elements.
## DATE:17/03/26
## AIM:
To write a C program to add two integer elements in an array using realloc() and that array already has three elements.

## Algorithm
Start.
Declare array size
Initialize array elements using malloc()
Update array size using realloc()
Print the result.
End.   

## Program:
```
/*
C program to add two integer elements in an array using realloc() and that array already has three elements.

Developed by: ARIGALA LAVANYA
RegisterNumber:  212222060019
#include <stdio.h>
#include <stdlib.h>
int main() {
 int *arr, size, i;
 size = 3;
 arr = (int *)malloc(size * sizeof(int)); 
 for (i = 0; i < size; i++) {
 arr[i] = i * 10; }
 printf("Original array:\n");
 for (i = 0; i < size; i++) {
 printf("%d ", arr[i]);
 }
 printf("\n");
 size *= 2;
 arr = (int *)realloc(arr, size * sizeof(int)); 
 for (i = size / 2; i < size; i++) {
 arr[i] = i * 10;
printf("Updated array:\n");
 for (i = 0; i < size; i++) {
 printf("%d ", arr[i]);
 }}
*/
```

## Output:

<img width="458" height="233" alt="image" src="https://github.com/user-attachments/assets/0e45a9b8-e57d-41a7-839d-4328d7efd955" />


## Result:
Thus the program was executed and the output was verified successfully.
