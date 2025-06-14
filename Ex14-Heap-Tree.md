# Ex14 Heap Tree
## DATE:
## AIM:
To write a C function to delete an element in a Heap Tree.

## Algorithm

1.	Start
2.	Find the index of the element num in the array.
3.	Swap the element to be deleted with the last element in the array.
4.	Decrease the array size (size) by 1.
5.	Start heapifying from the last non-leaf node (index size/2 - 1).
6.	Call heapify() to restore the heap property for each node.
7.	End
 
## Program:
```
/*
Program to delete an element in a Heap Tree
Developed by: S.VENGADA KRISHNAN
RegisterNumber:  212223110061
*/
```
```
void deleteRoot(int array[], int num)
{
  // type your code here
  int i;
  for(i=0;i<size;i++)
  {
      if(array[i]==num)
      {
          break;
      }
     }
    
         swap(&array[i],&array[size-1]);
         size--;
         for(i=size/2-1;i>=0;i--)
         {
             heapify(array,size,i);
         }
     
}
```
## Output:
![Screenshot 2025-04-29 213124](https://github.com/user-attachments/assets/fe7851e9-f91f-4dc4-88b3-c1df229d9f4f)


## Result:
Thus, the function to delete an element in a Heap Tree is implemented successfully.
