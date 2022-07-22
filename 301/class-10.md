# In memory storage 
[Understanding the JavaScript Call Stack](https://medium.freecodecamp.org/understanding-the-javascript-call-stack-861e41ae61d4)

**What is a ‘call’?**  
A function invocation.  

**How many ‘calls’ can happen at once?**  
One at a time, from top to bottom.  

**What does LIFO mean?**  
When we say that the call stack, operates by the data structure principle of Last In, First Out, it means that the last function that gets pushed into the stack is the first to be pop out, when the function returns.  

**Draw an example of a call stack and the functions that would need to be invoked to generate that call stack.**  
```
function firstFunction(){
  throw new Error('Stack Trace Error');
}

function secondFunction(){
  firstFunction();
}

function thirdFunction(){
  secondFunction();
}

thirdFunction();
```
![image](https://cdn-media-1.freecodecamp.org/images/QgR2uIk7tW0YNz0Xm8g0jAPeRFI0e4sCejsv)  

**What causes a Stack Overflow?**  
A stack overflow occurs when there is a recursive function (a function that calls itself) without an exit point. The browser (hosting environment) has a maximum stack call that it can accomodate before throwing a stack error.  

## [JavaScript error messages](https://codeburst.io/javascript-error-messages-debugging-d23f84f0ae7c)  

**What is a ‘reference error’?**  
This is as simple as when you try to use a variable that is not yet declared you get this type os errors.  

**What is a ‘syntax error’?**  
This occurs when you have something that cannot be parsed in terms of syntax, like when you try to parse an invalid object using JSON.parse.  

**What is a ‘range error’?**  
Try to manipulate an object with some kind of length and give it an invalid length and this kind of errors will show up.  

**What is a ‘type error’?**   
Like the name indicates, this types of errors show up when the types (number, string and so on) you are trying to use or access are incompatible, like accessing a property in an undefined type of variable.  

**What is a breakpoint?**  
Stops your code at a line fo your choosing.  

**What does the word ‘debugger’ do in your code?**  
Gives you a history of your call stack.  

## Bookmark and Review  
[JavaScript errors reference on MDN](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Errors)  
