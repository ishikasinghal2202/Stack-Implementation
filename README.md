/*
===============================================================
                STACK IMPLEMENTATION IN C++
===============================================================

---------------------------------------------------------------
Aim:
---------------------------------------------------------------
To study and implement the concept of Stack in C++ using arrays 
and functions with operations such as PUSH, POP, and PEEK.

---------------------------------------------------------------
Software Used:
---------------------------------------------------------------
- VS Code

---------------------------------------------------------------
Objectives:
---------------------------------------------------------------
1. To understand the concept of Stack as an Abstract Data Type.
2. To implement Stack operations using arrays.
3. To study the behavior of LIFO (Last In, First Out).
4. To handle Stack Overflow and Underflow conditions.
5. To analyze real-life applications of Stack.

---------------------------------------------------------------
Theory:
---------------------------------------------------------------
A Stack is a linear data structure that follows the LIFO principle.
In this structure, insertion (PUSH) and deletion (POP) operations 
are performed from only one end called the "TOP".

Key Operations:
1. PUSH: Insert an element into the stack.
2. POP: Remove the top element from the stack.
3. PEEK/TOP: Retrieve the top element without removing it.
4. isEmpty: Check if the stack is empty.
5. isFull: Check if the stack is full.

Applications of Stack:
- Expression evaluation (postfix, prefix, infix).
- Function call management in recursion.
- Undo/Redo operations in text editors.
- Backtracking algorithms (maze solving, DFS).
- Browser history navigation.

---------------------------------------------------------------
Algorithm (for Array-based Stack):
---------------------------------------------------------------
1. Initialize stack with maximum size and top = -1.
2. PUSH Operation:
   - If top == MAX-1 → Stack Overflow.
   - Else increment top and insert element.
3. POP Operation:
   - If top == -1 → Stack Underflow.
   - Else return element at top and decrement top.
4. PEEK Operation:
   - If stack not empty → return element at top.
   - Else → stack empty message.
5. Repeat as per user choice.

---------------------------------------------------------------
Flowchart (Stack Operations):
---------------------------------------------------------------

                +-------------------+
                |   START PROGRAM   |
                +-------------------+
                          |
                          v
                +-------------------+
                | Initialize STACK  |
                |    top = -1       |
                +-------------------+
                          |
                          v
        +--------------------------------+
        |   User Choice: PUSH / POP /    |
        |   PEEK / DISPLAY / EXIT        |
        +--------------------------------+
              /        |        \
             /         |         \
            v          v          v
   +--------------+ +--------------+ +-----------------+
   |    PUSH      | |     POP      | |      PEEK       |
   +--------------+ +--------------+ +-----------------+
   | Is Full?     | | Is Empty?    | | Is Empty?       |
   | Yes: Overflow| | Yes: Underflow| | Yes: Empty Msg |
   | No: Insert   | | No: Remove    | | No: Show Top   |
   +--------------+ +--------------+ +-----------------+
                          |
                          v
                +-------------------+
                | Continue / Exit ? |
                +-------------------+
                          |
                          v
                +-------------------+
                |      END          |
                +-------------------+

---------------------------------------------------------------
Table: Stack Operations Example
---------------------------------------------------------------

Operation    | Stack Content (Top at Right)
-------------|---------------------------------
PUSH(10)     | 10
PUSH(20)     | 10, 20
PUSH(30)     | 10, 20, 30
POP()        | 10, 20
PUSH(40)     | 10, 20, 40
PEEK() → 40  | 10, 20, 40

---------------------------------------------------------------
Conclusion:
---------------------------------------------------------------
- Stack is a simple but powerful data structure that works on LIFO.
- It is widely used in memory management, expression evaluation,
  function calls, and backtracking problems.
- Implementation using arrays is simple, but has a fixed size.
- For dynamic sizing, linked list based implementation is preferred.
- Understanding Stack forms the foundation of advanced DS & Algorithms.

===============================================================
*/
