# EX 1B Merge Sort
## DATE:
## AIM:
To write a python program for the implementation of merge sort on the given list of values.

## Algorithm
1.Divide the array into two halves recursively until each subarray has one element.
2.Conquer by merging sorted subarrays using the merge() function:
3.Compare elements from left and right subarrays.
4.Copy the smaller one into the original array.
5.Continue until all elements are merged.
6.Repeat until the whole array is sorted.

## Program:
```
/*
Program to implement Merge Sort
Developed by:  SUROTHAAMAN R
Register Number:  212222103003
*/
```
```
def merge(arr,l,m,r):
    n1 = m-l+1
    n2 = r-m
    L = [0] * (n1)
    R = [0] * (n2)
    for i in range(0,n1):
        L[i] = arr[l+i]
    for j in range(0,n2):
        R[j] = arr[m+1+j]
    i=0
    j=0
    k=l
    while i<n1 and j< n2:
        if L[i] <= R[j]:
            arr[k] = L[i]
            i+=1
        else:
            arr[k] = R[j]
            j+=1
        k+=1
    while i<n1:
        arr[k] = L[i]
        i+=1
        k+=1
    while j<n2:
        arr[k] = R[j]
        j+=1
        k+=1
def mergesort(arr,l,r):
    if l<r:
        m=l+(r-l)//2
        mergesort(arr,l,m)
        mergesort(arr,m+1,r)
        merge(arr,l,m,r)
arr = []
n = int(input())
for i in range(n):
     arr.append(float(input()))
print("Given array is")
for i in range(n):
    print("%d" % arr[i],end=" ")
mergesort(arr,0,n-1)
print("\nSorted array is")
for i in range(n):
    print("%d" % arr[i],end=" ")
```

## Output:

![image](https://github.com/user-attachments/assets/173637b1-1a9d-4ad6-96ae-4c852a14b9b9)

## Result:
The program successfully sorts the entire array using merge sort, arranging all elements in non-decreasing order.
