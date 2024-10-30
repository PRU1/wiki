---
Link: https://www.freecodecamp.org/news/recursion-is-not-hard-858a48830d83/
---
- When you call a function it goes into an execution stack
- Last in, first out. The last function called is the first function to run
- Execution runs a function
- Execution context: forms once a function is call. The context is like an order of operations. “The item that is always first in this stack is the global execution context” <oh this is js specific>

### What is recursion

- function calls itself until a base case is true, then execution stops
- without base case you’ll get stack overflow (when your computer runs out of memory to store all the items in the stack)

![[/Untitled 8.png|Untitled 8.png]]