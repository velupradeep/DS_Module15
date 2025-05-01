# Ex14 Heap Tree
## DATE: 01/05/2025
## AIM:
To write a C function to delete an element in a Heap Tree.

## Algorithm
1.Start

2.Find the index of the element num in the array.

3.Swap the element to be deleted with the last element in the array.

4.Decrease the array size (size) by 1.

5.Start heapifying from the last non-leaf node (index size/2 - 1).

6.Call heapify() to restore the heap property for each node.

7.End

## Program:
```
/*
Program to delete an element in a Heap Tree
Developed by: PRADEEP V
RegisterNumber: 212223240119
*/
void deleteRoot(int array[], int num) 
{ 
int i; 
for(i=0;i<size;i++) 
{ 
if(num==array[i]) 
{ 
break; 
} 
} 
swap(&array[i],&array[size-1]); 
size-=1; 
for(i=size/2-1;i>=0;i--) 
{ 
heapify(array,size,i); 
} 
}
```

## Output:

![437462564-0862893a-8a09-4817-98fa-0cc89849be7b](https://github.com/user-attachments/assets/89e34a2c-b5ca-4be0-be09-94d7fbb9ea09)


## Result:
Thus, the function to delete an element in a Heap Tree is implemented successfully.
