# Class 10 – Error Handling & Debugging

## Reading Overview 10

### JavaScript book

#### Order of Execution

- Order of execution is the order in which statements are run.
- Execution contexts are where code gets executed.
- There are three execution contexts where every statement in a script resides: global, function, eval.
- Variable scope pertains to the availability of variables within certain parts of the code.
- There are two types of variable scope: global and function-level.
- JavaScript processes one line of code at a time. It will stack, or pile, new functions on top of the current function it’s working on, then move on the next one in the stack.
- New statements that need data create a new execution context.
- When a script enters a new execution context, two phases of activity occur: 1. Prepare, 2. Execute.
- In the prepare phase, the new scope is created, and variables, functions, and arguments are created.
- In the execute phase, the execution context can assign values to variables, reference functions and run their code, and execute statements.
- Hoisting is when the interpreter moves the declaration functions to the top of the top of the variable scope before their executed.

#### Errors

- When there’s an error in the code, JavaScript will throw an exception.
- During this time, JavaScript will stop processing the function.
- When there is an error, an error object is created to help you diagnose and resolve the error.
- An error object contains the property and description of the error, including the type of error, name of the JavaScript file, and the line number of the error.
- There are seven types of built-in error objects in JavaScript: Error, SyntaxError, ReferencedError, TypeError, RangeError, URIError, and EvalError.

#### Handling Errors

- To deal with errors, you need to debug the script to fix errors and handle errors gracefully.
- You also need to design a workflow to identify where the problem is and what exactly is the problem.
- Breakpoints allow you to pause the execution of a script on any line to check the values stored in the variables at that point.
- Using breakpoints allow you to step through the code one-by-one to see where values change, and a problem might occur.
- Using the keyword “debugger” allows you to create the breakpoints.
- To handle exceptions, you use keywords “try,” catch,” and “finally.”
- When you “try,” you specify the code you think might thrown an exception within the “try” block.
- If the “try” code throws up an exception, then the “catch” step will propose an alternative.
- In the “finally” step, the contents in this code block will run either way, whether the “try” block succeeded or failed.
- You can always throw an error on purpose if you think an error might occur and be caught by the interpreter.
- Doing this ahead of time can stop further errors down in the script.
