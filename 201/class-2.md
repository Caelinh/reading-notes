# Basics of HTML, CSS and Javascript

## [HTML Fundamentals](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/HTML_text_fundamentals)
### Why is it important to use semantic elements in our HTML?
- Search engines will consider its contents as important keywords to influence the page's search rankings (see SEO)
- Screen readers can use it as a signpost to help visually impaired users navigate a page
- Finding blocks of meaningful code is significantly easier than searching through endless divs with or without semantic or namespaced classes
- Suggests to the developer the type of data that will be populated
- Semantic naming mirrors proper custom element/component naming
### How many levels of headings are there in HTML?
There are six levels.`<h1><h2><h3><h4><h5><h6>`
### What are some uses for the `<sup>` and `<sub>` elements?[ Good source](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Advanced_text_formatting)
`<sup>` is used for things like March 4<sup>th</sup>. `<sub>` is good for things like H<sub>2</sub>O.
### When using the `<abbr>` element, what attribute must be added to provide the full expansion of the term?
You can use the `<title>` attribute. <abbr title="Cascading style Sheets">CSS</abbr>.


## [Learning CSS](https://developer.mozilla.org/en-US/docs/Learn/CSS/First_steps/How_CSS_is_structured)
### What are ways we can apply CSS to our HTML?
- External stylesheet
- Internal stylesheet
- Inline
### Why should we avoid using inline styles?  
It's worst practice.
- least efficient implementation of CSS for maintenance.One styling change might require multiple edits within a single web page.
- Inline CSS also mixes (CSS) presentational code with HTML and content, making everything more difficult to read and understand.

### Review the block of code below and answer the following questions:  
     h2 {
     color: black;
     padding: 5px;
     }  
  - What is representing the selector?  
     h2
  - Which components are the CSS declarations? 
     ```json
        color:black;
        padding:5px;
      ```
  -  Which components are considered properties?  
     color and padding
## [Learning Javascript](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/JavaScript_basics)  
### What data type is a sequence of text enclosed in single quote marks? 
A string.  
### List 4 types of JavaScript operators.  
- `+`Addition
- `-`Subtraction
- `*`Multiplication
- `=`Assignment
### Describe a real world Problem you could solve with a Function. 
say I need a function that neds to take in a minimum value and a maximum value and return me a random number in between the two.  
#### [Conditionals](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Building_blocks/conditionals)  
### An if statement checks a \__ and if it evaluates to \___ then the code block will execute.  
expression; true
### What is the use of an `else if`?
Gives an alternative for the if statement if the value is false.
### List 3 different types of comparison operators.
`==`, `<`, `>`
### What is the difference between the logical operator `&&` and `||`?  
`&&` is true if both expressions are true. `||` is true if only one returns true.
### Writing [proper git commits](https://cbea.ms/git-commit/)
