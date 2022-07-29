# Authentication

## [What is OAuth](https://www.csoonline.com/article/3216404/what-is-oauth-how-the-open-authorization-framework-works.html)

**What is OAuth?**  
OAuth is an open-standard authorization protocol or framework that describes how unrelated servers and services can safely allow authenticated access to their assets without actually sharing the initial, related, single logon credential.  

**Give an example of what using OAuth would look like.**  
Anytime we go to a website that allows a login through facebook or google that is using an authentication token from that website. To gain authentication to the current one.  

**How does OAuth work? What are the steps that it takes to authenticate the user?**  
1. The first website connects to the second website on behalf of the user, using OAuth, providing the user’s verified identity.  
3. The second site generates a one-time token and a one-time secret unique to the transaction and parties involved.  
4. The first site gives this token and secret to the initiating user’s client software.  
5. The client’s software presents the request token and secret to their authorization provider (which may or may not be the second site).  
6. If not already authenticated to the authorization provider, the client may be asked to authenticate. After authentication, the client is asked to approve the authorization transaction to the second website.  
7. The user approves (or their software silently approves) a particular transaction type at the first website.  
8. The user is given an approved access token (notice it’s no longer a request token).  
9. The user gives the approved access token to the first website.  
10. The first website gives the access token to the second website as proof of authentication on behalf of the user.  
11. The second website lets the first website access their site on behalf of the user.  
12. The user sees a successfully completed transaction occurring.  
13. OAuth is not the first authentication/authorization system to work this way on behalf of the end-user. In fact, many authentication systems, notably Kerberos, work similarly. What is special about OAuth is its ability to work across the web and its wide adoption. It succeeded with adoption rates where previous attempts failed (for various reasons).  


**What is OpenID?**  
OpenID is about authentication.  "OpenID is for humans logging into machines, OAuth is for machines logging into machines on behalf of humans."  

## [Authorization and Authentication flows](https://auth0.com/docs/flows)

**What is the difference between authorization and authentication?**  
authentication is for humans logging into machines, authorization is for machines logging into machines on behalf of humans.  

**What is Authorization Code Flow?**  
![auth-sequence-auth-code](https://user-images.githubusercontent.com/106052558/181788555-23931268-0d03-4bbf-b1ac-26ef43767734.png)
1. The user clicks Login within the regular web application.

2. Auth0's SDK redirects the user to the Auth0 Authorization Server (
/authorize
endpoint).

3. Your Auth0 Authorization Server redirects the user to the login and authorization prompt.

4. The user authenticates using one of the configured login options and may see a consent page listing the permissions Auth0 will give to the regular web application.

5. Your Auth0 Authorization Server redirects the user back to the application with an authorization code, which is good for one use.

6. Auth0's SDK sends this code to the Auth0 Authorization Server (
/oauth/token
endpoint) along with the application's Client ID and Client Secret.

7. Your Auth0 Authorization Server verifies the code, Client ID, and Client Secret.

8. Your Auth0 Authorization Server responds with an ID Token and Access Token (and optionally, a Refresh Token).

9. Your application can use the Access Token to call an API to access information about the user.

10. The API responds with requested data.  


**What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)?**  
![auth-sequence-auth-code-pkce](https://user-images.githubusercontent.com/106052558/181788656-b2230df4-8dc7-4ccb-bb60-f6671edc6542.png)

1. The user clicks Login within the application.

2. Auth0's SDK creates a cryptographically-random code_verifier and from this generates a code_challenge.

3. Auth0's SDK redirects the user to the Auth0 Authorization Server (
/authorize
endpoint) along with the code_challenge.

4. Your Auth0 Authorization Server redirects the user to the login and authorization prompt.

5. The user authenticates using one of the configured login options and may see a consent page listing the permissions Auth0 will give to the application.

6. Your Auth0 Authorization Server stores the code_challenge and redirects the user back to the application with an authorization code, which is good for one use.

7. Auth0's SDK sends this code and the code_verifier (created in step 2) to the Auth0 Authorization Server (
/oauth/token
endpoint).

8. Your Auth0 Authorization Server verifies the code_challenge and code_verifier.

9. Your Auth0 Authorization Server responds with an ID Token and Access Token (and optionally, a Refresh Token).

10. Your application can use the Access Token to call an API to access information about the user.

11. The API responds with requested data.  


**What is Implicit Flow with Form Post?**  
![auth-sequence-implicit-form-post](https://user-images.githubusercontent.com/106052558/181788721-81a4acef-08b9-44c4-b589-beeecd589575.png)

1. The user clicks Login in the app.

2. Auth0's SDK redirects the user to the Auth0 Authorization Server (/authorize endpoint) passing along a response_type parameter of id_token that indicates the type of requested credential. It also passes along a response_mode parameter of form_post to ensure security.

3. Your Auth0 Authorization Server redirects the user to the login and authorization prompt.

4. The user authenticates using one of the configured login options and may see a consent page listing the permissions Auth0 will give to the app.

5. Your Auth0 Authorization Server redirects the user back to the app with an ID Token.  

**What is Client Credentials Flow?**  
With machine-to-machine (M2M) applications, such as CLIs, daemons, or services running on your back-end, the system authenticates and authorizes the app rather than a user. For this scenario, typical authentication schemes like username + password or social logins don't make sense. Instead, M2M apps use the Client Credentials Flow (defined in OAuth 2.0 RFC 6749, section 4.4), in which they pass along their Client ID and Client Secret to authenticate themselves and get a token.  

**What is Device Authorization Flow?**  
With input-constrained devices that connect to the internet, rather than authenticate the user directly, the device asks the user to go to a link on their computer or smartphone and authorize the device. This avoids a poor user experience for devices that do not have an easy way to enter text. To do this, device apps use the Device Authorization Flow (drafted in OAuth 2.0). For use with mobile/native applications.  

**What is Resource Owner Password Flow?**  
Though we do not recommend it, highly-trusted applications can use the Resource Owner Password Flow, which requests that users provide credentials (username and password), typically using an interactive form. The Resource Owner Password Flow should only be used when redirect-based flows (like the Authorization Code Flow) cannot be used.  

## Bookmark and Review

[Auth0 for single page apps](https://auth0.com/docs/libraries/auth0-react)
