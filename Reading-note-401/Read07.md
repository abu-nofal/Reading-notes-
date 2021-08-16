# Bearer Authorization

### Review, Research, and Discussion

1. Write the following steps in the correct order:



- Register your application to get a client_id and client_secret

- Make a request to a third-party API endpoint

- Ask the client if they want to sign in via a third party

- Redirect to a third party authentication endpoint

- Make a request to the access token endpoint

- Receive authorization code

2. What can you do with an authorization code?

- you can access the data and you will be an authorized user for that server.

3. What can you do with an access token 

- if this token match the token of arigistered user, then this user can be access data and make requests for the server.

3. What’s a benefit of using OAuth instead of your own basic authentication?

- beacuase it is a common used in the world, and can access most of the websites that might you deal with.

### Document the following Vocabulary Terms

1. Client ID: 
- it is a public identifier for apps

2. Client Secret: 
- The Client Secret is a secret known only to the OAuth Client and the Authorization Server.
- it is a secret used by the OAuth Client to Authenticate to the Authorization Server.


3. Authentication Endpoint:
- it is a security mechanism designed to ensure that only authorized devices can connect to a given network, site or service.

4. Access Token Endpoint:
- it is where apps make a request to get an access token for a user.



5. Authorization Code:
- it is a temporary code that the client will exchange for an access token. The code itself is obtained from the authorization server where the user gets a chance to see what the information the client is requesting, and approve or deny the request.

6. Access Token:
- it is the thing that applications use to make API requests on behalf of a user. The access token represents the authorization of a specific application to access specific parts of a user’s data.




### Intro to JWT

- main types of used algorithms in jwt :

  - HMAC
  - RSA
  - ECDSA

- jwt is most useful in :

  - Authorization : only one sign-in, then each request will compare the access token.
  - information exchange : it is useful when sending or transmitting data between applications.

- payload contains claims.

- Claims are statements about an entity (typically, the user) and additional data.


### Are JWTs Secure?

- when jwt generates a token, will use smething called secret.
  and you can decode the token and change the data in payload, but this secret you can't know its value. therefore, your token will still safe untill anyone know your secret.


[ref1](https://jwt.io/introduction/)
[ref2](https://stackoverflow.com/questions/27301557/if-you-can-decode-jwt-how-are-they-secure)