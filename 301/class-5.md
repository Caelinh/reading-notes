**What is the single responsibility principle and how does it apply to components?**  
A component should ideally only do one thing. If it ends up growing, it should be decomposed into smaller subcomponents.  

**What does it mean to build a ‘static’ version of your application?**   
To build a base bones version of the app that displays but doesn't have any interactivity.  

**Once you have a static application, what do you need to add?**   
UI components and how they will interact.  

**What are the three questions you can ask to determine if something is state?**  

1. Is it passed in from a parent via props?
2. Does it remain unchanged over time?
3. Can you compute it based on any other state or props in your component?

**How can you identify where state needs to live?**
- Identify every component that renders something based on that state.
- Find a common owner component (a single component above all the components that need the state in the hierarchy).
- Either the common owner or another component higher up in the hierarchy should own the state.
- If you can’t find a component where it makes sense to own the state, create a new component solely for holding the state and add it somewhere in the hierarchy above the common owner component.  

**What is a “higher-order function”?**  
Functions that operate on other functions, either by taking them as arguments or by returning them.  

**Explore the greaterThan function as defined in the reading. In your own words, what is line 2 of this function doing?**  
```  return m => m > n;```
It's returning a function that determines if m is higher than whats input the greaterTHan function.  

**Explain how either map or reduce operates, with regards to higher-order functions.**  
The map method transforms an array by applying a function to all of its elements and building a new array from the returned values. The new array will have the same length as the input array, but its content will have been mapped to a new form by the function.
