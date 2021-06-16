error handling and debuging 

EXECUTION CONTEXTS

The JavaScript interpreter uses the concept of execution contexts.
There is one global execution context; plus, each function creates a new execution context. They correspond to variable scope.

GLOBAL CONTEXT

Code that is in the script, but not in a function.
There is only one global context in any page.

FUNCTION CONTEXT
Code that is being run within a function.
Each function has its own function context.

EVAL CONTEXT (NOT SHOWN)
Text is executed like code in an internal function
called eval .

GLOBAL SCOPE
If a variable is declared outside a function, it can
be used anywhere because it has global scope.
If you do not use the var keyword when creating
a variable, it is placed in global scope.

FUNCTION-LEVEL SCOPE
When a variable is declared within a function,
it can only be used within that function. This is
because it has function-level scope.

UNDERSTANDING SCOPE

each execution context has its own va ri ables object.
It holds the variables, functions, and parameters available within it.
Each execution context can also access its parent's v a ri ables object.

Functions in JavaScript are said to have lexical scope.
They are linked to the object they were defined within.
So, for each execution context, the scope is the
current execution context's variables object, plus the
variables object for each parent execution context.

ERROR OBJECTS

Error objects can help you find where your mistakes are
and browsers have tools to help you read them.

Syntax Error:This is caused by incorrect use of the rules of the
language. It is often the result of a simple typo.

Reference Error:This is caused by a variable that is not declared or is out of scope

Eval Error : The eva l () function evaluates text through the
interpreter and runs it as code (it is not discussed
in this book). It is rare that you would see this type
of error, as browsers often throw other errors when
they are supposed to throw an Eva 1 Error.

URI Error : If these characters are not escaped in URls, they will
cause an error: / ? & I : ;

Type Error : This is often caused by trying to use an object or
method that does not exist.

Range Error : If you call a function using numbers outside of its
accepted range.

Error : The generic Error object is the template (or
prototype) from which all other error objects are
created.

NaN :Note: If you perform a mathematical operation using
a value that is not a number, you end up with the
value of NaN, not a type error.

A DEBUGGING WORK FLOW: Debugging is about deduction: eliminating potential causes of an error.

BROWSER DEV TOOLS & JAVASCRIPT CONSOLE: The JavaScript console will tell you when there is a problem with a script,
where to look for the problem, and what kind of issue it seems to be.