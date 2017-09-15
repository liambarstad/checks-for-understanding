1. How do we make flash messages display on a page?

2. Where is cart information/temporary information usually stored?

3. What might be some reasons not to store cart in our database? Are there any reasons why we would want to persist that information?

4. What is the purpose of the asset pipeline?

5. Why do we precompile our assets?

6. What do each of the following tags do?

```ruby
<%= stylesheet_link_tag "application" %>
<%= javascript_include_tag "application" %>
<%= image_tag "rails.png" %>
```

7. What are some of the elements of a great read me? What are some of the benefits of taking the time to update a readme for our project?

 - elements of a great readme include dependencies, code examples, possible implementations, and bug fixes/known errors
 - if a readme is updated frequently, it ensures that no functionality is overlooked

8. What are the top four accessibility issues that we as developers should be aware of?

  - Vision impairment
  - Motor function impairment/inability to use mouse
  - Auditory impairment

9. `before_save` is an example of a what? Where in our Rails application would we find a `before_save`?

  - 'before_save' is an example of a callback method, that can be used to instantiate an attribute with a value depending on other attributes or relationships in a model

10. Given the following object, how would we create a scope for all users who are active?

```ruby
User.create(name: "Happy", active: true)
```
```ruby
scope :active, where(active: true)
```

11. What is the difference between a scope and a class method?

  A scope makes a subset of saved instances of a given class, whereas a class method initially acts on all instances of a given class.
