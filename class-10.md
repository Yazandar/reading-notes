## Execution contexts

* To find the source of an error, it helps to know how scripts are processed. The order in which statements are executed can be complex; some tasks cannot complete until another statement or function has been run

* The JavaScript interpreter proccess one line of code at time. When a statement needs a data from another function, it ```stacks``` the new function on top of the current task.

* Each time a script enters a new execution context, there are two phases on activity :
    1. Prepare : the new scope is created then variables, functions and arguments are created then the value of the this keyword is determined.
    2. Execute : assign values to variables then reference function and run their code then excute statements.

* In the interpreter, each execution context has its own variables object. It holds the variables, functions, and parameters available within it. Each execution context can also access its parent's variables object.

* If a JavaScript statement generates an error, then it throws an exception. At that point, the interpreter stops and looks for exception-handl ing code.

* Error objects can help you find where your mistakes are and browsers have tools to help you read them.

* there are two things you can do with the errors:
    1. Debug the script to fix erorrs.
    2. Handle erorrs gracefully

* Debugging is about deduction: eliminating potential causes of an error.

* The JavaScript console will tell you when there is a problem with a script, where to look for the problem, and what kind of issue it seems to be.

* You can pause the execution of a script on any line using breakpoints. Then you can check the values stored in variables at that point in time.

* You can indicate that a breakpoint should be triggered only if a condition that you specify is met. The condition can use existing variables.

* If you know your code might fail, use ```try```, ```catch```, and ```finally```. Each one is given its own code block.

* If you know something might cause a problem for your script, you can generate your own errors before the interpreter creates them.

* Debugging tips
  * Some problems are browser-specific. Try the code in another browser to see which ones are causing a problem.

  * Write numbers to the console so you can see which the items get logged. It shows how far your code runs before errors stop it.

  * Remove parts of code, and strip it down to the minimum you need. You can do this either by removing the code altogether, or by just commenting it out using multi-line comments.

  * Programmers often report finding a solution to a problem while explaining the code to someone else.

  * Stack Overflow is a Q+A site for programmers.

  * If you want to ask about problematic code on a forum, in addition to pasting the code into a post, you could add it to a code playground site.

  [Back to Home](README.md)
