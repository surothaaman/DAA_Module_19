# EX 1C Quick Sort
## DATE:
## AIM:
To write a python program to implement quick sort on the given array values.

## Algorithm
1. Choose a pivot element (e.g., the first element).
2.Partition the remaining elements into two sublists:
 Left: elements less than pivot
 Right: elements greater than or equal to pivot
3.Recursively apply quick sort to the left and right sublists.
4. Combine the sorted left sublist, pivot, and sorted right sublist.
5.Return the combined sorted list.
 
## Program:
```
/*
Program to implement implement quick sort using the last element as pivot on the list of float values.
Developed by: SUROTHAAMAN R
Register Number:  212222103003
*/
```
```
def qsort(L):
    if L==[]:
        return []
    pivot=L[0:1]
    left=qsort([x for x in L[1:] if x<L[0]])
    right=qsort([x for x in L[1:] if x>=L[0]])
    print("left: ",left)
    print("right: ",right)
    return left+pivot+right
arr=[]
n=int(input())
for i in range(n):
    arr.append(int(input()))
print(qsort(arr))
```

## Output:
![image](https://github.com/user-attachments/assets/8b85127f-f622-4767-8b57-dfbc9ef9abb9)
## Result:
The program sorts the given list using quick sort and prints the sorted array, showing how the list is split into left and right parts at each step.
