# Authentication 

## Review, Research, and Discussion


1. Explain what a “Singleton” is (in Computer Science terms) 
- A singleton is a class that allows only a single instance of itself to be created and gives access to that created instance. It contains static variables that can accommodate unique and private instances of itself. It is used in scenarios when a user wants to restrict instantiation of a class to only one object. This is helpful usually when a single object is required to coordinate actions across a system.

[ref1](https://www.techopedia.com/definition/15830/singleton)


2. Explain how the Singleton pattern can be used with Node modules, specifically with classes 

- The singleton pattern is used in programming languages such as Java and .NET to define a global variable. A single object used across systems remains constant and needs to be defined only once rather than many times.

- A singleton is intended to provide only one instance of itself while facilitating a global point of access. Implementing a singleton pattern involves creating a class with a method that creates a new instance of the class. In order to implement a singleton pattern, principles of single instance and global access must be satisfied. 

- The singleton class is like a global repository for an instance of itself, making the constructor private. Therefore, an instance outside the class cannot be created at all, and a singleton can contain only one instance. A singleton class instantiates itself and maintains that instance across systems.


3. If you were tasked with building a middleware system like Express uses, what approach might you take to construct/operate it?

- ok there is tow type of middelware the first one is global and the secound is to be scoupe or to specific route or end point 
- so if i want to build one globel i will make a folder and put inside it the function i will use 
- the function will be for all route and metode (get , post ,put, delete)
- the fuction take three parameter (request , response , next)


## Document the following Vocabulary Terms

**Router Middleware** 
- Router-level middleware works in the same way as application-level middleware, except it is bound to an instance of express.Router().
**Dynamic Module Loading**
- Dynamic loading is a mechanism by which a computer program can, at run time, load a library (or other binary) into memory, retrieve the addresses of functions and variables contained in the library, execute those functions or access those variables, and unload the library from memory.
**Singleton Pattern**
- In software engineering, the singleton pattern is a software design pattern that restricts the instantiation of a class to one "single" instance. This is useful when exactly one object is needed to coordinate actions across the system. The term comes from the mathematical concept of a singleton.
**CRUD -> REST Method Matches**
- C:=> create ,post
- R:=> retrieve , get 
- U:=> update , put 
- D:=> delete , delete


## Preparation Materials

1. Securing Passwords 

- We all know storing passwords in clear text in your database is ridiculous. Many desktop applications and almost every web service including, blogs, forums eventually need to store a collection of user data and the passwords, that has to be stored using a hashing algorithm.

- Cryptographic hash algorithms MD5, SHA1, SHA256, SHA512, SHA-3 are general purpose hash functions, designed to calculate a digest of huge amounts of data in as short a time as possible. Hashing is the greatest way for protecting passwords and considered to be pretty safe for ensuring the integrity of data or password.

- The benefit of hashing is that if someone steals the database with hashed passwords, they only make off with the hashes and not the actual plaintext passwords. But why do we always hear about passwords being cracked? There are some weaknesses in cryptographic hash algorithm that allows an attacker to calculate the original value of a hashed password .

> PROBLEMS WITH CRYPTOGRAPHIC HASH ALGORITHM 

- Brute Force attack
- Hash Collision attack


2. Basic access authentication 

- In the context of an HTTP transaction, basic access authentication is a method for an HTTP user agent (e.g. a web browser) to provide a user name and password when making a request. In basic HTTP authentication, a request contains a header field in the form of Authorization: Basic `<credentials>`, where credentials is the Base64 encoding of ID and password joined by a single colon :.

It is specified in RFC 7617 from 2015, which obsoletes RFC 2617 from 1999.

3. bcrypt docs
- (bcrypt)A library to help you hash passwords.
- bcrypt is a password-hashing function designed by Niels Provos and David Mazières, based on the Blowfish cipher and presented at USENIX in 1999  Besides incorporating a salt to protect against rainbow table attacks, bcrypt is an adaptive function: over time, the iteration count can be increased to make it slower, so it remains resistant to brute-force search attacks even with increasing computation power.