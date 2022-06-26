# HTML Tables; JS Constructor Functions  
## Domain modeling and HTML tables  
### [Domain Modeling](https://github.com/codefellows/domain_modeling#domain-modeling)
**Explain why we need domain modeling.**  
We need it because the problems that we are trying to solve with programming need to be broken down into simpler parts in order to figure out all the problems we need to solve in the broad picture. Modeling it out makes for a more efficient program and can squash problems youn might run into just winging it.  
### [HTML Table Basics](https://developer.mozilla.org/en-US/docs/Learn/HTML/Tables/Basics)  

**Why should tables not be used for page layouts?**
1. Layout tables reduce accessibility for visually impaired users.  
2. Tables produce tag soup. The code is harder to read and troubleshoot.  
3. Tables are not automatically responsive. tables are sized to their content naturally so extra measures have to be made to style.  

**List and describe 3 different semantic HTML elements used in an HTML `<table>`.**  
1. `<th>` Table header is used to create a row that sits on top of the table that has the styling youd expect from the label row.
2. `<tr>` Creates a row for the table.
3. `<td>` Table data creates a cell and is nested inside of each row.   
## [Introducing Constructors](https://developer.mozilla.org/en-US/docs/Learn/JavaScript/Objects/Basics#introducing_constructors)

**What is a constructor and what are some advantages to using it?**  
A constructor is a function that makes it easy to create new objects with some predetirmed attributes that can also be added to later.  
**How does the term this differ when used in an object literal versus when used in a constructor?**  
When used in a literal it's only going to work for that specific object. In a constructor it can repurpose any function you have to work for a new object created.  
### [Object Prototypes Using A Constructor](https://ui.dev/beginners-guide-to-javascript-prototype)

**Explain prototypes and inheritance via an analogy from your previous work experience.**  

#### Bookmark and review
[HTML Table Advanced Features and Accessibility](https://developer.mozilla.org/en-US/docs/Learn/HTML/Tables/Advanced)
