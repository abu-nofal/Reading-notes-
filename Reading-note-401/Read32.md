# Context API - Behaviors

---  

### Review, Research, and Discussion 

**When you have multiple contexts, what component type should you use (class/function) and why?**

- you can use any one of theme  
- if you use the function you will use (useContext()) hook  
- if you use class you will use (consumer)

**What are some good use cases for using the Context API for global state?**

- for themes  
- authorization  

**How can you best test context?**

- The best way to test Context is to make our tests unaware of its existence and avoiding mocks  

---
### Document the following Vocabulary Terms

**context** 

- rovides a way to share values like these between components without having to explicitly pass a prop through every level of the tree.

**useContext()**

- ***useContext*** hook is used to create common data that can be accessed throughout the component hierarchy without passing the props down manually to each level.

**static context**

- it used when you have one context 
- A static method or, block belongs to the class and these will be loaded into the memory along with the class. You can invoke static methods without creating an object. … But static contexts(methods and blocks) doesn’t have any instance they belong to the class.


