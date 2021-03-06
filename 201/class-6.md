# JS Object Literals and The DOM
## [Javascript Object Basics](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Objects/Basics)
**How would you describe an object to a non-technical friend you grew up with?**  
An object is a container that can hold a variety of data types and attributess that relate to that object in whatever way you see fit.  
**What are some advantages to creating object literals?** 
It makes it easier and more efficient to transfer things between servers or databases if they are inside of objects than all seperated individually.  
**How do objects differ from arrays?**   
Objects can store arrays and functions. It's also easier to call what you want in an object with dot notation.    
**Give an example for when you would need to use bracket notation to access an object’s property instead of dot notation.**  
Dot notation to bracket notation.
```
person.age
person.name.first
person['age']
person['name']['first']
```
**Evaluate the code below. What does the term this refer to and what is the advantage to using this?**  
The `this` keyword refers to the current object the code is being written inside. In this example it is the object dog. It'd udeful wheneever your using constructors and creating multiple objects using the same code.  
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
The Document Object Model (DOM) is a programming interface for web documents. It represents the page so that programs can change the document structure, style, and content. The DOM represents the document as nodes and objects; that way, programming languages can interact with the page.  
**Briefly describe the relationship between the DOM and JavaScript.**  
The DOM creates objects out of all the elements on a webpage that can be accessed by any programming language to be manipulated or read from using api's.  

## Bookmark and Review ##
[Understanding the problem domain is the hardest part of programming](https://simpleprogrammer.com/understanding-the-problem-domain-is-the-hardest-part-of-programming)

[What’s the difference between primitive values and object references in JavaScript?](https://betterprogramming.pub/intermediate-javascript-whats-the-difference-between-primitive-values-and-object-references-e863d70677b)
