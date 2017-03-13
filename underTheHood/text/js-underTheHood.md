# JS Under The Hood

> Understanding how JS works

# 1. Object {}

An Object: The most important of the communication data elements today. What is an object ?
> it's a 'name: value' pair.

#2. The Global environment and the Global Object.

Everytime we creat a .js file, always are created:

1. A 'Window' object.
2. A 'this' attribute.
3. A global 'environment'

#3. The Execution context: Creation + Context

> Everytime we execute a .js file happens the following:

1. A new Execution Context is created:
 > A window + this + environment is created
 > All functions are loaded to memory
 > All variables are set to 'undefined' by default

 This is what is called: 'hoisting'

 #4. Single Threated + Synchcronous Execution

 JS executes :
 1. One thing at a time
 2. One after the other

 #5. Function Invocation and the Execution Stack

 Everytime a function is called or Invoked:
 A new Execution Stack is created. They stack one over the 
 other until all of them are executed

 #6. Functions, Context, and Variable Environments

 A Function will look for it's attributes values in the following order:

 1. In the function itseld or it's execution context
 2. In it's direct upper environment.
 3. If not in the next one aso until the root itself.

 #7. Scope Chain

 > It's the chain of stacked functions executions
 any js file goes through until it arrives to the root.

 #8. Asynchcronous Callbacks

 They do not exist as such in the reality. JS is synchronous singled threated but calls can be made at the same time in other parallel engines like the Render or HTTP one. 

 This calls will be stacke on the 'Event Stack' and executed properly only when the Exectution Stack is finished.

 ##### END OF THE BASICS #####