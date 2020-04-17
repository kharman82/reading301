[README.MD](README.md)  
**Resources**  
[https://developer.mozilla.org/en-US/docs/Glossary/Call_stack](stack)   
[https://codeburst.io/javascript-error-messages-debugging-d23f84f0ae7c](JavaScript error messages && debugging)  
 
**Call Stack**  
- A call stack is a mechanism for an interpreter (like the JavaScript interpreter in a web browser) to keep track of its place in a script that calls multiple functions — what function is currently being run and what functions are called from within that function, etc.  
    - When a script calls a function, the interpreter adds it to the call stack and then starts carrying out the function.  
    - Any functions that are called by that function are added to the call stack further up, and run where their calls are reached.  
    - When the current function is finished, the interpreter takes it off the stack and resumes execution where it left off in the last code listing.  
    - If the stack takes up more space than it had assigned to it, it results in a "stack overflow" error.   
- The call stack is synchronous. 
- In Asynchronous JavaScript, we have a callback function, an event loop, and a task queue. The callback function is acted upon by the call stack during execution after the call back function has been pushed to the stack by the event loop.  

_LIFO_ :  When we say that the call stack, operates by the data structure principle of Last In, First Out, it means that the last function that gets pushed into the stack is the first to be pop out, when the function returns.  
_Temporarily store_: When a function is invoked (called), the function, its parameters, and variables are pushed into the call stack to form a stack frame. This stack frame is a memory location in the stack. The memory is cleared when the function returns as it is pop out of the stack.  

_Manage function invocation (call)_ : The call stack maintains a record of the position of each stack frame. It knows the next function to be executed (and will remove it after execution). This is what makes code execution in JavaScript synchronous.Manage function invocation (call): The call stack maintains a record of the position of each stack frame. It knows the next function to be executed (and will remove it after execution). This is what makes code execution in JavaScript synchronous.  
**What Causes a Stack Overflow?**  
- A stack overflow occurs when there is a recursive function (a function that calls itself) without an exit point. The browser (hosting environment) has a maximum stack call that it can accomodate before throwing a stack error.  

**Errors and types of them**  
_Reference Errors_ : Variable that is not yet declared. Result: os error.  
_Temporal Dead Zone_ happens when using _let_ and _const_ when you try to access them between the hosting and being declared.  
_Syntax errors_ : this occurs when you have something that cannot be parsed in terms of syntax, like when you try to parse an invalid object using JSON.parse.  
_Range Errors_ Try to manipulate an object with some kind of length and give it an invalid length and this kind of errors will show up.  
_Type Errors_ :Try to manipulate an object with some kind of length and give it an invalid length and this kind of errors will show up.  
