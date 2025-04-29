# EX 1A Reverse a String
## DATE:
## AIM: To Write a Program to Create a recursive function to reverse a string
## Algorithm

1. Take input string s.
2. If length of s is 0 or 1, return s (base case).
3. Otherwise, recursively call the function with s[1:].
4. Append s[0] to the result of the recursive call.
5. Return the final reversed string. 

## Program:
```
/*
Program to implement Reverse a String
Developed by: SUROTHAAMAN R
Register Number: 212222103003
*/
```
```

def reverse_string(s):
    if len(s) == 0:  
        return s
    else:
        return s[-1] + reverse_string(s[:-1]) 

input_string = input()
reversed_string = reverse_string(input_string)
print(reversed_string)

```

## Output:
![image](https://github.com/user-attachments/assets/d167cae5-99fd-4089-b4ba-0e3fd5d166ed)

## Result:
The program successfully reverses the input string using recursion. When the user provides an input string, the output displays the reversed version of the string
