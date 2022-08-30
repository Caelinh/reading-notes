# Storing data in a site

### Accessing data in spring io with JPA

Annotations for a data class are  
````
@Entity
public class Example {

@Id
@GeneratedValue

````
Spring JPA database is a relational databased. It's able to create repository inplementations autmatically at runtime.

**Resource for more in depth [reading](https://spring.io/guides/gs/accessing-data-jpa/)  

**CRUD FUNCTIONALITY AVAILABLE TO JPA**  

- save(…) – save an Iterable of entities. Here, we can pass multiple objects to save them in a batch  
- findOne(…) – get a single entity based on passed primary key value  
- findAll() – get an Iterable of all available entities in database  
- count() – return the count of total entities in a table  
- delete(…) – delete an entity based on the passed object  
- exists(…) – verify if an entity exists based on the passed primary key value  

**jpa Respository methods**  
- findAll() – get a List of all available entities in database
- findAll(…) – get a List of all available entities and sort them using the provided condition
- save(…) – save an Iterable of entities. Here, we can pass multiple objects to save them in a batch
- flush() – flush all pending task to the database
- saveAndFlush(…) – save the entity and flush changes immediately
- deleteInBatch(…) – delete an Iterable of entities. Here, we can pass multiple objects to delete them in a batch

