# Access Control (ACL)

### Review, Research, and Discussion

1. When is Basic Authorization used vs. Bearer Authorization?

- basic authorization used when in sign-in process, after signing-up.
- bearer authorization used after basic auth done.

2. What does the JSON Web Token package do?

- generates a token that we can use with authorization and information exchange.

3. What considerations should we make when creating and storing a SECRET?

- don't create a weak secret.
- don't store it in a plain text.
- don't share your secret with anyone.
- make a rotation for your secret.
- don't use same secret for different accounts.

### Document the following Vocabulary Terms

1. encryption:
- it is a process that convert our passwords to hashed ones, with characters representation. to make our passwords secured. we use the bcrybt library to do this.

2. token:
- it an encoded json, that we use in beare authorization to ensure if the user is authorized or not.

3. bearer:
- it is an authorization process, that use the header, and create and compare the token for the users, to allow them to reach a certain endpionts or not.

4. secret:
- it is a signiture for the developper that make his token secure and no one can access his data when his secret is exists.

5. JSON Web Token
- it is an open standard (RFC 7519) that defines a compact and self-contained way for securely transmitting information between parties as a JSON object.

