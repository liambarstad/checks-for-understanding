## Week Two - Module 4 Recap

Fork this respository. Answer the questions to the best of your ability. Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week. 

Note: When you're done, submit a PR. 

1. What's one difference between ES5 and ES6?

  - in ES6, you can declare functions with the fat arrow notation (() => {})
  - ES6 introduces require('..') and classes
  - ES5 requires the use of semi-colons in some instances

2. What's the difference between asynchronous and synchronous JavaScript? 

  Asynchronous JavaScript pops promises and API calls off the execution stack and adds them to an external queue. When the promise's conditions are met, the code block is re-added to the stack. Synchronous JavaScript, alternately, is put on the execution stack one by one in a predictable order.

3. What are the four pillars of Object Oriented programming?

  - Abstraction
  - Encapsulation
  - Inheritence
  - Polymorphism

4. What are some tools available in JavaScript to help you write object oriented code?

  - Objects/Prototypical inheritence
  - Classes/Classical inheritence

5. What are some key concepts to be aware of when refactoring your JavaScript?

  - divide by functionality
  - only augment DOM in one place/class type
  - diagram out the flow of the application and isolate the roles that will turn into classes

6. What's a callback function and what are some reasons when we use/need callback functions?

  A callback function is a function declaration that can be passed as a paramter to other functions/objects. This function can hence be executed in the scope where it is passed, using tools like bind to change the value of "this" in the callback. This can be used to create more versitile functions, that can take other functions as arguements.

7. What's the scope of variables in Javascript?

  The scope of a variable in JavaScript is the extent of the code block where it is defined. Global variables can also be declared anywhere, but this is commonly regarded as a bad practice.

8. What's the difference between `==` and `===` in JavaScript?

  == is more abstract than ===, which compares the memory addresses of the data being compared. For instance, 0 == [] but !(0 === [])

9. Why do front end frameworks exist?

#### Review  

10. Why do people say "HTTP is stateless"?

  A new instance of the application is generated upon request from the client, which does not know any of the local variable declarations that might have occured previously in a different instance of the app.

11. Describe a RESTful API.

  A RESTful API will conform to the 7 RESTful routes for resources or services, and will not include (for instance) a DELETE or PATCH route applying to all records in a resource.

12. What are some main characteristics of a team following an agile workflow?
13. What are some advantages **and** disadvantages to using OAuth to authenticate a user?
