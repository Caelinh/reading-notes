# One to many relationships and tests

## One to many  

This relationship occurs when one record in table one is related to one or more in table 2. One record in table 2 cannot be related to more than one record in table 1.  

**Some examples:**  
- pages and the book they belong to 
- pupils and class
- orders and the customer that placed them

![example image](https://blog.devart.com/wp-content/uploads/2021/10/one-to-many-relation-diagram-1.png)

### Resources for a look at the code
**[SQL](https://blog.devart.com/types-of-relationships-in-sql-server-database.html) / [Spring](https://www.baeldung.com/spring-data-rest-relationships)**  

## Tests for REST

**The following needs to be added to the test class for JUNIT.**  
````
@ExtendWith(SpringExtension.class)
@ContextConfiguration(classes = { ApplicationConfig.class })
@WebAppConfiguration
public class GreetControllerIntegrationTest {
    ....
}
````
- Spring allows us to do testing using a mock database, saving on the time and energy of creating a real one to test. 
- In case theres dependencies that you can't work out Spring has helper classes than can help.

### Resources and a look at code
**[Testing](https://www.lambdatest.com/blog/spring-testing/) / [Code](https://www.baeldung.com/integration-testing-in-spring)**  



