## Week Three - Module 4 Recap

Fork this respository. Answer the questions to the best of your ability. Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week. 

Note: When you're done, submit a PR. 

1. At a high level, what is Node?

  Node is a JavaScript compiler that allows JavaScript to be run independently of the browser.

2. What is Express? What is Express similar to in the Ruby world?

  Express is a web framework, similar to rails, that comes pre-built with a templating language (jade), router functionality, and some essential libraries.

3. How do we setup a route when creating an API with Node and Express? Please provide a code snippet.

  - require the appropriate file for the path base in app.js:

    app.use('/api/v1/foods', foods)

  - in foods.js in the routes directory (or whatever name is specified above), add the functions to the router object that correspond with the specfic path:

    e.g. router.get('/', function(req, res, next) {
           res.status(200).html('<h1>Dooooood</h1>')
         })

4. What do we use Knex for?

  Knex is an ORM, in that it builds SQL queries in JavaScript and returns results in JSON notation.

5. How could you organize your code to follow the MVC design pattern in your Quantified Self project?

  You could have the logic to query the database in a models directory organized by resource, and a controllers section used to define the funtions used in the routes file.

6. How do you execute raw SQL in node?

  In knex, where "database" is a variable pointing to the configured database, you can use database.raw('<<sqlQuery>>'), which returns a promise.
  
7. What are some advantages to having your front end and back end code live in separate applications? What are some disadvantages?
  
  Pros:
    * Applications can be specialized for performance (e.g. a JS front end makes on-click events easier than a rails app)
    * Front end applications (and probably back end) can retrieve information from multiple places, such as microservices or APIs
    * Applications can be more easily switched out and tested for performance

  Cons:
    * More work goes into matching the transmission of data
    * Problems can be harder to diagnose
    * Processes can be slower and more costly

#### Review  

8. Describe DNS.
  
  Domain Name System (I did have to look this up): the method by which computers identify themselves to each other and to services over the internet, using IP addresses.

9. What does writing clean code mean to you?
  
  To me, the cleanliness of code relies on its ability to account for changes with minimal effort and be reusable and extensible for other situations. Either as a bonus or as a result, code should then be encapsulated in minimal statements and relatively easy to understand.

10. If you were building an application that models hotels, what classes would you need? What classes would be responsible for what functionality?
  
  - Hotel:
    * Name
    * Rating

  - Guest:
    * Trip length
    * Satisfaction
    - Critic:
      * Rate

  - Service (directory or abstract class):
    * Wage
    * Hours
    * Calculate earnings
    * Disgruntled?
    * Call security
    - Concierge:
      * Check in Guest
      * Check out Guest
    - Valet: 
      * Park Car
    - Security: 
      * ignore super(call_security)
      * Forcibly check out guest
    - Manager:
      * Blame for problem

  - Maintenance:
    ...
