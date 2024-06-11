# RPN to Infix
***Start:** April 1<sup>st</sup> 2023, **Finish:** April 15<sup>th</sup> 2023*

For a second-year course: Algorithms & Data Structures

This program reads an arithmetic expression in reverse polish notation from standard input, and prints out the same expression using infix notation with brackets using trees. The only integers appearing in the expression will be single-digit (0-9). Error handling is not yet implemented.

## Procedure
1) Read input into string variable `input`.
2) Read the string variable character by character.
**a)** If the current character is a number, push it to stack `S` and create a new null tree.
**b)** If the current character is an operator, pop the top two numbers in the stack and push a new tree (with the two trees as the branches) to the stack.
4) Display the tree via in-order traversal.
**a)** If the currently-displayed tree's data is not a number, add brackets to the display before the next tree.

## Example
Example 1:
```
10/3+ // Input
((1/0)+3) // Output
```
Example 2:
```
123*4-+ // Input
(1+((2*3)-4)) // Output
```

## What I learnt:
- How to implement class `Tree` for expression trees
- Understanding of RPN and infix notations and how to convert from one to the other
