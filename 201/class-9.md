# Forms and JS Events

## [HTML Forms](https://developer.mozilla.org/en-US/docs/Learn/Forms)

### [Your first Web Form.](https://developer.mozilla.org/en-US/docs/Learn/Forms/Your_first_form) [How To Structure A Web Form](https://developer.mozilla.org/en-US/docs/Learn/Forms/How_to_structure_a_web_form)

**Why are forms so important in web development?**  
Forms allow the user to interact with your site and input data needed to perform whatever goal you have. As well as being able to create an account and have a personalized experience that can carry over data over a server.  

**When designing a form, what are some key things to keep in mind when it comes to user experience?**  
It's important to keep accessibilty features in mind when creating form elements. Making meaningful labels and a readable form is important for the user to know how to properly give whatever data is needed.   

**List 5 form elements and explain their importance.**  
1. `<fieldset>` is used to create a group of widgets that are convenient for semantic and styling purposes. Everytime you have a set of radio buttons they should be nested inside of a fieldset element.
2.  `<legend>` is used to label the container that all of the other labels are sitting inside inside. Very useful for screen readers. 
3.  `<label>` This is a formal way to define a label.  
4.  `<button>` Is used to submit form data usually.
5.  `<input>` A convenient way to allow a user to input data.  
## [Learn JS](https://developer.mozilla.org/en-US/docs/Learn/JavaScript)
### [Introduction To Events](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/Events)

**How would you describe events to a non-technical friend?** 
Events are reactionary to something you do to interact with the website. Such as what happens when I click this button or when I scroll down to a certain point on the page.  

**When using the `addEventListener()` method, what 2 arguments will you need to provide?**  
1. The event your listening for such as a click or hover etc..
2. A function that runs once that event happens.

**Describe the event object. Why is the target within the event object useful?**  
The event object references directly what is being interacted with and can make it easy to target an attribute you would like to collect or change.  

**What is the difference between event bubbling and event capturing?**  
In the **capturing phase**:  
- The browser checks to see if the element's outer-most ancestor (<html>) has a click event handler registered on it for the capturing phase, and runs it if so.  
- Then it moves on to the next element inside <html> and does the same thing, then the next one, and so on until it reaches the direct parent of the element that was actually clicked.  
 
 In the **bubbling phase**, the exact opposite of the capturing phase occurs:

- The browser checks to see if the direct parent of the clicked element has a click event handler registered on it for the bubbling phase, and runs it if so.
- Then it moves on to the next immediate ancestor element and does the same thing, then the next one, and so on until it reaches the <html> element.  
  
#### Bookmark and Review

[HTML5 Input Types](https://developer.mozilla.org/en-US/docs/Learn/Forms/HTML5_input_types)  

[Event Reference and listings](https://developer.mozilla.org/en-US/docs/Web/Events)

