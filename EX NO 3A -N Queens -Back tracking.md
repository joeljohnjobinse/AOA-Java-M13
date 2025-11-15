# EX 3A N Queens Problem - Backtracking Approach.
## DATE: 12/09/2025
## AIM:
To write a Java program for N-Queens using a backtracking approach.
You are given an integer N. For a given N x N chessboard, find a way to place N queens such that no queen can attack any other queen on the chessboard.
A queen can be attacked when it lies in the same row, column, or the same diagonal as any of the other queens. You have to print one such configuration.

Chess Board
<img width="241" height="209" alt="image" src="https://github.com/user-attachments/assets/96aacb61-4f34-423f-b324-5e34454e42b8" />

Note:

- Get the input from the user for N. The value of N must be from 1 to 4.
- If a solution exists print a binary matrix as output that has 1s for the cells where queens are placed.
- If there is no solution to the problem print: "Solution does not exist"

---

## Algorithm
1. Start the program and read integer N from the user (1 ≤ N ≤ 4).  
2. Initialize an N × N board with all zeros.  
3. Use backtracking to try placing a queen row by row:
   - For each row, iterate over all columns.
   - For each column, check if placing a queen at (row, col) is safe (no other queen in same column, left diagonal or right diagonal).
   - If safe, place the queen (set board[row][col] = 1) and recursively try to place queens in the next row.
   - If recursion succeeds, return true; otherwise remove the queen (backtrack) and try next column.
4. If all N queens are placed (row == N), print the board and return success.
5. If no placement works for a row, return failure and eventually print "Solution does not exist".

---

## Program:
```
/*
Program to implement N-Queens (Backtracking Approach)
Developed by: Joel John Jobinse
Register Number: 212223240062
*/

```
---

## Output:

---

## Result:
The program implements the N-Queens problem using backtracking.
