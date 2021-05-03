# Testing and Modules
## Testing
#### Unit tests are parts of code written by a programmer to exercise the input, the output and how the code behaves. if a client has a website and want to change the website functionalties or what it recives and how it store it then the clinet has to hires a programmer to do that. for that programmer he has to test the code so he can know how it works then makes the changes. in python tests are done on a file its name is similar to the file name to be tested but it exsits in a tests folder. the implementation has a convention arrangement which is:
- **Arrange** the data needed to execute
- **Act** to execute the code being tested
- **Assert** after executing the code
#### the test process has a cycle of:
1. Write a unit test and make it fail 
2. Write the feature and make the test pass
3. Refactor the code
## Recursion
#### Recursion happens when a function calls itself directly or indirectly. use a recursive algorithm can make some problems as:
- Towers of Hanoi (TOH)
- Inorder
- Preorder
- Postorder Tree Traversals
- DFS of Graph
#### however these problems can be solved 
#### base condition in recursion is the condition that will break the recursion process so it must has a base condition to avoid infinte loop or errors. as mentioned recurion can be done directly by the same function or indirect by other function. When a function is called, the memory allocated it on the stack. when a recursive function calls itself, the memory for the new calling is allocated on top of previous one and different copy of local variables is created for each function call. When the base condition is reached, the function returns the condition base value. a recursive code can be written iteratively and vice versa. recursion can provide clean and simple code as in coding mathimatical factorial