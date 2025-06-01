# Ex11 Tree Representation and Traversal
## DATE:
## AIM:
To write a C function to perform post order traversal of a binary tree.

## Algorithm
1. Start and define display_postorder(root_node).
2. If root_node is not null, recursively call left and right children.
3. After both calls, print the current node’s value.
4. End algorithm.  

## Program:
```
Program to perform post order traversal of a binary tree.
Developed by: S.VENGADA KRISHNAN
RegisterNumber:  212223110061

/*struct node
{
int value;
struct node*left_child, *right_child;
};
*/
void display_postorder(struct node*root_node)
{
    if(root_node)
    {
        display_postorder(root_node->left_child);
        display_postorder(root_node->right_child);
        printf("%d\n",root_node->value);
    }
}
```

## Output:
![Screenshot 2025-04-29 212313](https://github.com/user-attachments/assets/6bfabcd0-f056-47f5-8763-e1eda17a4682)




## Result:
Thus, the function to perform post order traversal of a binary tree is implemented successfully
