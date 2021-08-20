# Memory Storage

## Call Stack

**call stack is a data structure that uses the Last In, First Out (LIFO) principle to temporarily store and manage function invocation (call).**

## Types Of Call

* **LIFO:** _When we say that the call stack, operates by the data structure principle of Last In, First Out, it means that the last function that gets pushed into the stack is the first to be pop out, when the function returns._

* **Temporarily store:**_When a function is invoked (called), the function, its parameters, and variables are pushed into the call stack to form a stack frame. This stack frame is a memory location in the stack. The memory is cleared when the function returns as it is pop out of the stack._

* **Manage function invocation (call):** _The call stack maintains a record of the position of each stack frame. It knows the next function to be executed (and will remove it after execution). This is what makes code execution in JavaScript synchronous._


## Stack Overflow

**A stack overflow occurs when there is a recursive function (a function that calls itself) without an exit point. The browser (hosting environment) has a maximum stack call that it can accomodate before throwing a stack error.**



## Type JavaScript error messages


* **Reference errors**
_This is as simple as when you try to use a variable that is not yet declared you get this type os errors._

* **Syntax errors**
_I know it’s in the name of the errors, but like it says itself, this occurs when you have something that cannot be parsed in terms of syntax, like when you try to parse an invalid object using JSON.parse._

* **Range errors**
_manipulate an object with some kind of length and give it an invalid length and this kind of errors will show up._


* **Type errors**
_Like the name indicates, this types of errors show up when the types (number, string and so on) you are trying to use or access are incompatible, like accessing a property in an undefined type of variable._


## Debugging

**debugging is a multistep process that involves identifying a problem, isolating the source of the problem, and then either correcting the problem or determining a way to work around it. The final step of debugging is to test the correction or workaround and make sure it works.**