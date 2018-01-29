## Week One - Module 4 Recap

Fork this respository. Answer the questions to the best of your ability. Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week. 

Note: When you're done, submit a PR. 

1. What's the most useful thing you learned from completing the intermission week work?

  I really enjoyed learning about non-relational databases with Neo4j and (FINALLY) implementing the Interactive Broker API. It was also very useful to get comfortable with writing python scripts without a web framework. I also took part of a datacamp course, which gave me a good understanding of how to create hacker data and interpret results.

2. What are some tools to help debug JavaScript code?

  - Developer tools (with many different functions)
  - console.log(...)
  - debugger

3. What are some tools you need in order to unit test your JavaScript?

  Mocha and chai, as well as decent enough compartmentalization of JavaScript code.

4. What is the syntax for invoking a function?

  invokeThisFunction() -> invokes

5. What is CORS?

  CORS allows HTTP requests to gain access to assets from a different server than the one currently in use. 
    e.g. "POST" requests to an external API

6. How do we enable CORS?

  - installing browser extension
  - adding development hash in webpack config file
  - adding "Allow-Access-Origin": "..." to headers

7. What's `this` in JavaScript?

  `this` refers to the object that a function is called upon, when being referenced within the function declaration block.

8. What is Webpack and why is it useful?

  webpack is a mini web framework that compiles javascript modules to display content in the browser.

9. When/why do you want to use event delegation?

  Event delegation is useful when one wants to add an event listener that targets certain different child nodes of a common parent node. The event can be set to the parent node in question and then filter out events by using event.target and event.currentTarget.

10. What's `npm` and what do we use it for?

  npm, which I assume stands for node package manager, it used to download and update javascript libraries 

#### Review  
11. What's the MVC design pattern? Describe each part of MVC.
12. What are a few ways to optimize a Rails application?

  - organize controller logic into services and html blocks into helpers, etc.
  - check the newrelic analysis of the performance of specific methods on the web page
  - use caching on the page (cache do...) or through a key-value database such as redis
  - combine multiple images into a single, larger image, which can be displayed part by part to avoid extraneous asset requests

13. What's a background worker? When would we want to use a background worker?

  A background worker is a task that runs periodically in the background of a web application. This can be used for sending emails, checking a queue or API, or making API calls, among other purposes. we would use a background worker when we want to do a task that doesn't need to be triggered by an HTTP request.

