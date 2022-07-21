# Functional Programming

[Functional Programming Concepts](https://medium.com/the-renaissance-developer/concepts-of-functional-programming-in-javascript-6bc84220d2aa)

**What is functional programming?**  
Functional programming is a programming paradigm — a style of building the structure and elements of computer programs — that treats computation as the evaluation of mathematical functions and avoids changing-state and mutable data.  

**What is a pure function and how do we know if something is a pure function?**  
- It returns the same result if given the same arguments (it is also referred as deterministic)
- It does not cause any observable side effects  

**What are the benefits of a pure function?**  
- Code is easier to test.
- The funciton is immutable.( state cannot change after it’s created)
**What is immutability?**  
When data is immutable, its state cannot change after it’s created. If you want to change an immutable object, you can’t. Instead, you create a new object with the new value.  
**What is Referential transparency?**  
pure functions + immutable data = referential transparency.  

### Videos
[Node JS Tutorial for Beginners #6 - Modules and require()](https://www.youtube.com/watch?v=xHLd36QoS4k)

**What is a module?**  
It's another javascript file created to comoplete a certain task.  

**What does the word ‘require’ do?**  
it imports another file.  

**How do we bring another module into the file the we are working in?**  
By using require and importing the file needed. You have to make sure to export the module.  

**What do we have to do to make a module available?**  
module.exports= function name. Set it to a variable.  

