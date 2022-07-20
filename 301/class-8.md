# API's  

### [API Design Best Practices](https://docs.microsoft.com/en-us/azure/architecture/best-practices/api-design)
**What does REST stand for?**  
Representational State Transfer  

**REST APIs are designed around** resources, which are any kind of object, data, or service that can be accessed by the client.  

**What is an identifier of a resource? Give an example.**   
It's a URI that uniquelly identifies the resource. for example https://adventure-works.com/orders/1 ```/orders/1```  

**What are the most common HTTP verbs?**  
- get
- post
- put
- patch
- delete  

**What should the URIs be based on?**  
URIs should be based on nouns (the resource).  

**Give an example of a good URI.**  
```https://adventure-works.com/orders```  

**What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?**  
It means having a lot of small resources that need multiple requests to be called. This can create a large load and be bad for the client as well as your API.  

**What status code does a successful GET request return?**  
HTTP status code 200  

**What status code does an unsuccessful GET request return?**   
HTTP status code 204 (No Content)  

**What status code does a successful POST request return?**  
HTTP status code 201 (Created)  

**What status code does a successful DELETE request return?**  
HTTP status code 204 (No Content)  

## Bookmark and Review
[RegExr - Pay particular attention to the cheatsheet](https://regexr.com/)  
[Regex Tutorial](https://medium.com/factory-mind/regex-tutorial-a-simple-cheatsheet-by-examples-649dc1c3f285)  
[Regex 101](https://regex101.com/)  
