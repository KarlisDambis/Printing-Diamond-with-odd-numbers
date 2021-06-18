# Printing-Diamond-with-odd-numbers
# This particular code only works with odd numbers. 
```
print("Give the value of n(odd):")
n=int(input())
```
The value n is going to be the height of the diamond and we store it in a variable 'n'.
```
x=n//2+1
```
We find n//3 and store it in x.
```
for i,j in zip(range(1,x+1),range(1,n+1,2)):
  print(' '*(x-i)+'*'*(j))
```
The number of white space is calculated at x+1 and the number of stars is n+1.
```
for i,j in zip(range(1,x+1),range(n-2,-1,-2)):
  print(' '*(i)+'*'*(j))
```
Need to use 2 loops, because of the diamond shape. First loop is going to give me enlarging pattern at first and the second loop gives me inverse pattern.
i and j are variables for nested loop till the ranges x+1 and n+1, this also happens at the second loop till ranges x+1 and -1.
And the stars print till x-iand j values(firts half of the diamond) and x and j values(second half of the diamond).
