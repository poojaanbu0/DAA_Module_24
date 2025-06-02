# EX 6D BRUTE FORCE ALGORITHM

## AIM:

To write a python program using brute force method of searching for the given substring in the main string.

## Algorithm
1. Start
2. Input the main string 'string'.
3. Input the substring 'sub'.
4. Initialize:
   - l ← length of string
   - ls ← length of sub
   - found ← false
5. For each index k from 0 to l - ls (inclusive), do:
   a. Extract the substring of 'string' from index k to k + ls.
   b. Compare it with 'sub'.
   c. If they are equal:
      i. Print "Found at index k"
      ii. Set found ← true
6. If found is still false after the loop ends:
   - Print "Substring not found"
7. End

## Program:

```
/*
# Developed by: Pooja A
# Register Number: 212222240072
*/

def match(string,sub):
    l = len(string)
    ls = len(sub)
    start = sub[0];

    for k in range(l-ls+1):
        if start==string[k]:

            if string[k:k+ls]==sub:
                print(f"Found at index {k}")
    # print("Substring not found")

str1=input()
str2=input()

```

## Output:
![447235462-4147a9db-7fd1-44cc-8b0c-6173a5d35215](https://github.com/user-attachments/assets/916669ea-6e60-4133-a358-b9147e1bdd86)

## Result:
Thus the above program was executed successfully for searching the substring at respective index.
