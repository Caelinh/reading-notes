# [Javascript Object Basics](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Objects/Basics)
**How would you describe an object to a non-technical friend you grew up with?**  
An object is a container that can hold a variety of data types and attributess that relate to that object in whatever way you see fit.  
**What are some advantages to creating object literals?** 
It makes it easier and more efficient to transfer things between servers or databases if they are inside of objects than all seperated individually.  
**How do objects differ from arrays?**   
Objects can store arrays and functions. It's also easier to call what you want in an object with dot notation.    
**Give an example for when you would need to use bracket notation to access an object’s property instead of dot notation.**  

**Evaluate the code below. What does the term this refer to and what is the advantage to using this?**  

```
const dog = {
  name: 'Spot',
  age: 2,
  color: 'white with black spots',
  humanAge: function (){
    console.log(`${this.name} is ${this.age*7} in human years`);
  }
}
```

## [Introduction To The DOM](https://developer.mozilla.org/en-US/docs/Web/API/Document_Object_Model/Introduction)
**What is the DOM?**  
**Briefly describe the relationship between the DOM and JavaScript.**  


## Bookmark and Review ##
[Understanding the problem domain is the hardest part of programming](https://simpleprogrammer.com/understanding-the-problem-domain-is-the-hardest-part-of-programming)

[What’s the difference between primitive values and object references in JavaScript?](https://betterprogramming.pub/intermediate-javascript-whats-the-difference-between-primitive-values-and-object-references-e863d70677b)
