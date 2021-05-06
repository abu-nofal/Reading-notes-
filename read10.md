# ERROR HANDLING & DEBUGGING

> ORDER OF EXECUTION

To find the source of an error, it helps to know how scripts are processed. The order in which statements are executed can be complex; some tasks cannot complete until another statement or function has been run:

![img](https://learning.oreilly.com/library/view/javascript-and-jquery/9781118531648/images/p452-001.jpg)

This script above creates a greeting message, then writes it to an alert box (see right-hand page). In order to create that greeting, two functions are used: greetUser() and getName().

You might think that the order of execution (the order in which statements are processed) would be as numbered: one through to four. However, it is a little more complicated.

To complete step one, the interpreter needs the results of the functions in steps two and three (because the message contains values returned by those functions). The order of execution is more like this: 1, 2, 3, 2, 1, 4.

1. The greeting variable gets its value from the greetUser() function.

2. greetUser() creates the message by combining the string ‘Hello ’ with the result of getName().

3. getName() returns the name to greetUser().

2. greetUser() now knows the name, and combines it with the string. It then returns the message to the statement that called it in step 1.

1. The value of the greeting is stored in memory.

4. This greeting variable is written to an alert box.

> EXECUTION CONTEXTS

The JavaScript interpreter uses the concept of execution contexts. There is one global execution context; plus, each function creates a new new execution context. They correspond to variable scope. 

![](https://learning.oreilly.com/library/view/javascript-and-jquery/9781118531648/images/p453-001.jpg)

### EXECUTION CONTEXT

Every statement in a script lives in one of three execution contexts:
1. GLOBAL CONTEXT
  - Code that is in the script, but not in a function. There is only one global context in any page.
2. FUNCTION CONTEXT
  - Code that is being run within a function. Each function has its own function context.
3. EVAL CONTEXT (NOT SHOWN)
  - Text is executed like code in an internal function called eval() (which is not covered in this book).


### VARIABLE SCOPE
The first two execution contexts correspond with the notion of scope (which you met on p98):

1.  GLOBAL SCOPE

If a variable is declared outside a function, it can be used anywhere because it has global scope. If you do not use the var keyword when creating a variable, it is placed in global scope.

2. FUNCTION-LEVEL SCOPE

When a variable is declared within a function, it can only be used within that function. This is because it has function-level scope.


> EXECUTION CONTEXT & HOISTING
Each time a script enters a new execution context, there are two phases of activity:

1: PREPARE

- The new scope is created
- Variables, functions, and arguments are created
- The value of the this keyword is determined

2: EXECUTE

- Now it can assign values to variables
- Reference functions and run their code
- Execute statements