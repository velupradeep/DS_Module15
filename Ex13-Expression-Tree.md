# Ex13 Expression Tree
## DATE: 01/05/2025
## AIM:
To write a C function to construct an Expression Tree for the given Postfix Expression and display the output in the format of In-order ,Pre-order and Post-order traversal.

## Algorithm
1.Start

2.Print node data in preorder then traverse left then

3.Traverse left in inorder then print node data then traverse right

4.Traverse left in postorder then traverse right then print node data

5.Recursive approach is used for all three traversal methods

6.Functions handle each tree node using tree->d, tree->l, tree->r

7.End

## Program:
```
/*
Program to construct an Expression Tree for the given Postfix Expression and display the output in the format of In-order ,Pre-order and Post-order traversal.
Developed by: PRADEEP V
RegisterNumber: 212223240119
*/
struct n { 
char d; 
struct n *l; 
struct n *r; 
};*/ 
void preOrder(struct n *tree) 
{ 
if(tree) 
{ 
printf("%c",tree->d); 
preOrder(tree->l); 
preOrder(tree->r); 
} 
} 
void inOrder(struct n *tree) 
{ 
if(tree) 
{ 
inOrder(tree->l); 
printf("%c",tree->d); 
inOrder(tree->r); 
} 
} 
void postOrder(struct n *tree) 
  
  
{ 
if(tree) 
{ 
postOrder(tree->l); 
postOrder(tree->r); 
printf("%c",tree->d); 
} 
} 
```

## Output:

![437461342-bb84060f-0ca9-4de4-b37f-92152fb3d8e7](https://github.com/user-attachments/assets/f305b7c0-6a7e-46bd-a309-9e9a11450279)


## Result:
Thus, the C program to display the Expression Tree in the format of In-order ,Pre-order and Post-order traversal.
