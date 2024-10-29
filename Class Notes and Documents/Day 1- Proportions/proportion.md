# Solving an unknown number (numerator or denominator) of a proportion with Python.

## What is a Proportion?  
A proportion is simply an equality between two sets of numbers that share the same ratio. For example, if two sets of numbers are written as a/b and c/d, and they have the same ratio, we write a/b=c/d. This equality is what we call a proportion.

## Solve an unknown number in a proportion  
In a proportion, let's say n1/d1=n2/d2 where ‘n’ means numerator and ‘d’ means denominator. If we are given the first fraction a/b which is known and another fraction x/d or c/x where one of the numbers is unknown ‘x’.

To solve for x for the given expression a/b = x/d, we can say x = (a*d)/b and for the expression a/b = c/x, (b*c)/a will be the solve for the x.

## Solving Proportion in Python  
To solve a proportion in Python, first, we will declare variables for the numerators and denominators n1, d1, n2, and d2 and assign values to them. For the unknown value, we will assign 0 to the variable.

```
n1 = 1
d1 = 2
n2 = 0
d2 = 16
```
As we might have an unknown numerator on a denominator for the second function, we have to check which one we have to solve for. We can use the “if else” condition to determine the unknown value ‘x’. For Now, since we have the numerator for the second fraction as the unknown value, we will use the (a*d)/b expression to solve for ‘x’.

```
if n2==0:
  answer = d2 * n1 / d1
  print("n2 = ", answer)

elif d2==0:
  answer = n2 * d1 / n1
  print("n2 = ", answer)
```
Here’s what the output looks like…

```
n2 =  8.0 
```
