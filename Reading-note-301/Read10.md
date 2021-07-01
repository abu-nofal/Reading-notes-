# In memory storage 

## Understanding the JavaScript Call Stack 

**What is a ‘call’?**

- When a function is invoked 


**How many ‘calls’ can happen at once?**

- one at a time

**What does LIFO mean?**

- When we say that the call stack, operates by the data structure principle of Last In, First Out, it means that the last function that gets pushed into the stack is the first to be pop out, when the function returns.

**Draw an example of a call stack and the functions that would need to be invoked to generate that call stack.**

> `function firstFunction(){
  console.log("Hello from firstFunction");
}

function secondFunction(){
  firstFunction();
  console.log("The end from secondFunction");
}

secondFunction();`


**What causes a Stack Overflow?**


- A stack overflow occurs when there is a recursive function (a function that calls itself) without an exit point. The browser (hosting environment) has a maximum stack call that it can accomodate before throwing a stack error. 

> `function callMyself(){
  callMyself();
}

callMyself();` 


## JavaScript error messages 



**What is a ‘refrence error’?**

- when you try to use a variable that is not yet declared

- the fix is as simple has declaring the variable before any declaration is made.

**What is a ‘syntax error’?**

-  when you have something that cannot be parsed in terms of syntax 

- This can be solved by just fixing the syntax


**What is a ‘range error’?**

- Try to manipulate an object with some kind of length and give it an invalid length and this kind of errors will show up. 


**What is a ‘tyep error’?**

- when the types (number, string and so on) you are trying to use or access are incompatible 

**What is a breakpoint?**

- can also be achieved by putting a debugger statement in your code in the line you want to break 
- this is awesome for when you want to debug huge cycles for specific values

**What does the word ‘debugger’ do in your code?**
- The breakpoint can also be achieved

[Call Stack](https://codeburst.io/javascript-error-messages-debugging-d23f84f0ae7c)