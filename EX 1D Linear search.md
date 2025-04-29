# EX 1D Linear search
## DATE:
## AIM:
To write a python program to implement linear search on the given integer tuple.

## Algorithm
1. Start from the first element of the list.
2. Compare each element with the target value n.
3.If a match is found, print "Found" and exit the loop.
4. If loop completes without finding a match, print "Not found".
5. End the search process.

## Program:
```
/*
Program to implement a search function with parameter list name and the value to be searched using string values.
Developed by: SUROTHAAMAN R
Register Number:  212222103003
*/
```
```
def search(List,n):
    for i in List:
        if i==n:
            print(n,"Found")
            break
    else:
        print(n,"not found")
List=[input() for _ in range(int(input()))]
n=input()
search(List,n)
```
## Output:
![image](https://github.com/user-attachments/assets/3b29bf93-7ca4-4689-b04b-b3fafbb8f453)
## Result:
The program searches for a value in the given tuple and prints whether it was found or not.
