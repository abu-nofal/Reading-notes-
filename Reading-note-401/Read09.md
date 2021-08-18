# Authorization/Authentication

### Review, Research, and Discussion

1. What header(s) are used in authentication and authorization

- basic encode(username:password) 
- Bearer Token


2. What is safe to put into a JWT

- Data token: As the JWT serialized form is compact and easy to integrate in HTTP request JWT are often used as a mechanism of data interchange.
- ID token: Issued by an Identity Manager, on behalf of a client application, after authenticating the user. It allows the client application to get user information from the token in a safe way without the need of managing user credentials.
- Access token: Issued by an authorization server, on behalf of a client application, it allows the client application to access a protected resource on behalf of a user. This kind of token is used as an authentication and authorization mechanism by the client application towards the server holding the resource.

3. How are JWTs validated
**In order to validate a JWT, you must know the content of JWT.**

- Header
  - The contents of the Header describe the cryptographic operations to the JWT data. 
- Payload
  - The payload is the central part of the JWT which contains verifiable security statements 
  - Registered Claim Names
  - Public Claim Names
  - Private Claim Names

- Signature 
  - HS256 algorithm, which is short for HMAC-SHA256
  - RS256 signing algorithm, which is short for RSA-SHA256 



### Document the following Vocabulary Terms

1. **RBAC**
- In computer systems security, role-based access control (RBAC) or role-based security is an approach to restricting system access to authorized users. It is an approach to implement mandatory access control (MAC) or discretionary access control (DAC).
2. **User Roles**
- A user role defines permissions for users to perform a group of tasks. In a default WordPress installation there are some predefined roles with a predefined set of permissions. These roles are Super Admin, Administrator, Editor, Author, Contributor, and Subscriber
3. **JWT Token**
- JSON Web Token (JWT) is an open standard (RFC 7519) that defines a compact and self-contained way for securely transmitting information between parties as a JSON object. This information can be verified and trusted because it is digitally signed. JWTs can be signed using a secret (with the HMAC algorithm) or a public/private key pair using RSA or ECDSA.