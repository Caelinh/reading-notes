# Introductory HTML and JavaScript

## [Getting started](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Getting_started)

### Describe how HTML, CSS, and JS files are “parsed” in the browser.  

They are parse in the following order.  
- HTML as that leads to the css and javascript links being read.  
- As its read requests are sent for the css that was linked. Followed by the javascript.  

### How can you find images to add to a Website?  
Google images is a great source for images and can even be filtered for non copyright images.  

### How do you create a String vs a Number in JavaScript?  
A string is encased in "" while a number uses actual numbers with no quotations.  

### What is a Variable and why are they important in JavaScript?  
A variable is a store of value defined by you. It can be anything.  

## Introduction to HTML  

### What is an HTML attribute? [source](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Getting_started#see_also)
Attributes contain extra information about the element that won't appear in the content.  
<br>
### Describe the Anatomy of an HTMl element.  
>The opening tag: This consists of the name of the element (in this example, p for paragraph), wrapped in opening and closing angle brackets.  
>This opening tag marks where the element begins or starts to take effect.
>The content: What's inside of the tags.
>The closing tag: This is the same as the opening tag, except that it includes a forward slash before the element name. This marks where the element ends.  

### What is the Difference between `<article>` and `<section>` element tags?
An `<article>` represents a self contained composition of a document. It should be easily distrubutable.  
A `<section>` is a broader element that which doesn't have anything too specific but usually holds a group of content. It usally has a header as well.

### What Elements does a “typical” website include? [source](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/Document_and_website_structure)
- A header
- navigation bar
- main content/article
- sidebar
- footer  
### How does [metadata](https://developer.mozilla.org/en-US/docs/Learn/HTML/Introduction_to_HTML/The_head_metadata_in_HTML) influence Search Engine Optimization?
Search engines use meta data while searching for sites so it's important to use good tags that defines your content so the site shows in results.  
### How is the <meta> HTML tag used when specifying metadata?
This tag is used to define language tags and allows your site to be translated to any language in the specific ruleset defined.  

## some use cases for `<section>`  
- If the contents of the element represent a standalone, atomic unit of content that makes sense syndicated as a standalone piece (e.g. a blog post or blog comment, or a newspaper article), the `<article>` element would be a better choice.
- If the contents represent useful tangential information that works alongside the main content, but is not directly part of it (like related links, or an author bio), use an `<aside>`.
- If the contents represent the main content area of a document, use `<main>`.
- If you are only using the element as a styling wrapper, use a `<div>`. An unwritten rule is that a `<section>` should logically appear in the outline of a document.

## [Designing a website](https://developer.mozilla.org/en-US/docs/Learn/Common_questions/Thinking_before_coding)

### What is the first step to designing a Website?  
What do you want the site to accomplish? Think about these things.  
- What exactly do I want to accomplish?
- How will a website help me reach my goals?
- What needs to be done, and in what order, to reach my goals?  <br>
### What is the most important question to answer when designing a Website?  
What exactly it is you want to accomplish and how you can solve those problems with the content of your site.  

## [Semantics](https://developer.mozilla.org/en-US/docs/Glossary/Semantics)  
### Why should you use an `<h1>` element over a `<span>` element to display a top level heading?  
Using the correct tag to suit the job intended is useful for accecibility reasons, search engines, other people reading code, and it just organizes content in a better way period. 

### What are the benefits of using semantic tags in our HTML
Things to consider.  
- Search engines will consider its contents as important keywords to influence the page's search rankings (see SEO)
- Screen readers can use it as a signpost to help visually impaired users navigate a page
- Finding blocks of meaningful code is significantly easier than searching through endless divs with or without semantic or namespaced classes
- Suggests to the developer the type of data that will be populated
- Semantic naming mirrors proper custom element/component naming  
