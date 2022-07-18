# React and forms

### Forms  
[React Docs - Forms](https://reactjs.org/docs/forms.html)

**What is a ‘Controlled Component’?**  
Its a element that has it's own state internally that becomes controlled by react so that they sync up and you can control the state.
**Should we wait to store the users responses from the form into state when they submit the form OR should we update the state with their responses as soon as they enter them? Why.**  
Update as soon as hey enter so that the information can be used in other UI elements such as a fuzzy search.  

**How do we target what the user is entering if we have an event handler on an input field?**  
by using the {e.value} tag. This can find the value in the form by it's assiged name so it can be used accordingly.  

### [The Conditional (Ternary) Operator Explained](https://codeburst.io/javascript-the-conditional-ternary-operator-explained-cac7218beeff)

**Why would we use a ternary operator?**  
It's a shorthand version of an if statement that can make your code more readable.  

**Rewrite the following statement using a ternary statement:**
```
  if(x===y){
    console.log(true);
  } else {
    console.log(false);
  }
  ```
  ```
    x===y ? console.log(true):console.log(false)
  ```
  

## Bookmark and Review
[React Bootstrap - Forms](https://react-bootstrap.github.io/forms/overview/)  
[React Docs - conditional rendering](https://reactjs.org/docs/conditional-rendering.html)  
