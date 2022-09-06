# Spring Security

**AUthentication v authorization  
Who are you and what are you allowed to do?  

The main method for authentication is the authentication manager.  
````
public interface AuthenticationManager {

  Authentication authenticate(Authentication authentication)
    throws AuthenticationException;
}
````
Authentication manager can do three things.  
- return an `Authentication` if it can verify input is true.  
- Throws an `AuthenticationException` if invalid.(Runtime exception)
- returns null if undecided.  

![Authentication Chart](https://github.com/spring-guides/top-spring-security-architecture/raw/main/images/authentication.png)

###  Resources  
 
[Cheatsheet](https://github.com/codefellows/seattle-java-401d2/blob/master/SpringAuthCheatSheet.md)  
[Spring Security docs](https://spring.io/guides/topicals/spring-security-architecture/)  
