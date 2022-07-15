What is the single responsibility principle and how does it apply to components?  
A component should ideally only do one thing. If it ends up growing, it should be decomposed into smaller subcomponents.  

What does it mean to build a ‘static’ version of your application?  
To build a base bones version of the app that displays but doesn't have any interactivity.  

Once you have a static application, what do you need to add?  
UI components and how they will interact.  

What are the three questions you can ask to determine if something is state? 
1. Is it passed in from a parent via props?
2. Does it remain unchanged over time?
3. Can you compute it based on any other state or props in your component?
