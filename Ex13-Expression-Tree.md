# Ex13 Expression Tree
## DATE:
## AIM:
To write a C function to construct an Expression Tree for the given Postfix Expression and display the output in the format of In-order ,Pre-order and Post-order traversal.

## Algorithm

1.	Start
2.	Print node data in preorder then traverse left then right
3.	Traverse left in inorder then print node data then traverse right
4.	Traverse left in postorder then traverse right then print node data
5.	Recursive approach is used for all three traversal methods
6.	Functions handle each tree node using tree->d, tree->l, tree->r
7.	End

## Program:
```
/*
Program to construct an Expression Tree for the given Postfix Expression and display the output in the format of In-order ,Pre-order and Post-order traversal.
Developed by: S.VENGADA KRISHNAN
RegisterNumber:  212223110061
*/
```
```
/*
struct n {
   char d;
   struct n *l;
   struct n *r;
};*/
void preOrder(struct n *tree) {
 // Type your code here
 if(tree)
 {
     printf("%c",tree->d);
     preOrder(tree->l);
     preOrder(tree->r);
 }
   
}
void inOrder(struct n *tree) {
  //type your code here
  if(tree){
      inOrder(tree->l);
  printf("%c",tree->d);
     inOrder(tree->r);
  }  
}
void postOrder(struct n *tree) {
  //type your code here 
  if(tree){
  
     postOrder(tree->l);
     postOrder(tree->r);
     printf("%c",tree->d);
  }
}
```
## Output:
![Screenshot 2025-04-29 212903](https://github.com/user-attachments/assets/b425d948-0e32-4082-9e51-bb49fc029e6c)


## Result:
Thus, the C program to display the Expression Tree in the format of In-order ,Pre-order and Post-order traversal.
