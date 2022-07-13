# Passing Functions as Props

[React Docs - lists and keys](https://reactjs.org/docs/lists-and-keys.html)

**What does .map() return?**  
a new array using the values of the one passed through it.  

**If I want to loop through an array and display each value in JSX, how do I do that in React?**  
  ```
    let array = [1,2,3,4,5];
    const list = array.map((number) =>
      <li>{number}</li>
      );
      <ul>{list}</ul>
  ````

**Each list item needs a unique _key___.**  

**What is the purpose of a key?**  
Keys help React identify which items have changed, are added, or are removed. Keys should be given to the elements inside the array to give the elements a stable identity:

[The Spread Operator](https://medium.com/coding-at-dawn/how-to-use-the-spread-operator-in-javascript-b9e4a8b06fab)

**What is the spread operator?**
**List 4 things that the spread operator can do.**  
**Give an example of using the spread operator to combine two arrays.**  
**Give an example of using the spread operator to add a new item to an array.**  
**Give an example of using the spread operator to combine two objects into one.**  

## Videos

[How to Pass Functions Between Components](https://www.youtube.com/watch?v=c05OL7XbwXU)

**In the video, what is the first step that the developer does to pass functions between components?**  
**In your own words, what does the increment function do?**  
**How can you pass a method from a parent component into a child component?**  
**How does the child component invoke a method that was passed to it from a parent component?**  

## Bookmark and Review

[React Tutorial through ‘Declaring a Winner’](https://reactjs.org/tutorial/tutorial.html)  
[React Docs - Lifting State Up](https://reactjs.org/docs/lifting-state-up.html)  
