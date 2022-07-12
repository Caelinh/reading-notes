# State and Props

[React lifecycle](https://medium.com/@joshuablankenshipnola/react-component-lifecycle-events-cb77e670a093)

**Based off the diagram, what happens first, the ‘render’ or the ‘componentDidMount’?**  
The render happens first.

**What is the very first thing to happen in the lifecycle of React?**  
Mounting
**Put the following things in the order that they happen: `componentDidMount`, `render`, `constructor`, `componentWillUnmount`, `React Updates`**  
1. `constructor`
2. `render`
3. `react updates`
4. `componentdidmount`
5. `componentwillunmount`  

**What does `componentDidMount` do?**  
This method is invoked immediately after a component is mounted. If you need to load anything using a network request or initialize the DOM, it should go here. This method is a good place to set up any subscriptions  

## Videos

[React State Vs Props](https://www.youtube.com/watch?v=IYvD9oBCuJI)

**What types of things can you pass in the props?**  
counters, titles, subtitles, any initialized data.  

**What is the big difference between props and state?**  
props are handles outside a component and must be updated outside the component, state is inside. Props are passed into a component.  

**When do we re-render our application?**  
When the user has done something that requires the display to update with the changes.  

**What are some examples of things that we could store in state?**  
inside of a form so elements can be updated as the user innteracts with it.  
A counter that is updated based on what the user is doing


### Bookmark and Review
[React Docs - State and Lifecycle](https://reactjs.org/docs/state-and-lifecycle.html)  
[React Docs - handling events](https://reactjs.org/docs/handling-events.html)  
[React Tutorial through ‘Developer Tools’](https://reactjs.org/tutorial/tutorial.html)  
[React Bootstrap Documentation](https://react-bootstrap.github.io/)  
[Boootstrap Cheatsheet](https://getbootstrap.com/docs/5.0/examples/cheatsheet/)  
[Bootstrap Shuffle - a class “sandbox”](https://bootstrapshuffle.com/classes)  
[Netlify](https://www.netlify.com/)  
