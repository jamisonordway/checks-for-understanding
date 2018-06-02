### Week 5 Questions

Re-pull from this respository. Answer the questions to the best of your ability. Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week (which is a TON!).

Note: When you're done, submit a PR.

### Week 5 Questions
# 1. How do we make flash messages display on a page?

flash[:message] = "You have successfully logged out."

# 2. Where is cart information/temporary information usually stored?

Session

# 3. What might be some reasons not to store a cart in our database? Are there any reasons why we would want to persist that information?

In case there is too much data for a single database to handle. Some sites may want to persist the information for analytics or for user experience.

# 4. What is the purpose of the asset pipeline?

To make the response and request cycle faster by compressing multiple files of the same type down to a smaller file which can be sent in fewer requests.

# 5. Why do we precompile our assets?

To update changes in production environments/server

6. What do each of the following tags do?


#7. What are some of the elements of a great read me? What are some of the benefits of taking the time to update a readme for our project?

Information about where project is deployed, how to run program and tests, where to report bugs, which technology is being used, the purpose of the project

# 8. What are the top four accessibility issues that we as developers should be aware of?

Visual impairment, making sure functionality is available from a keyboard, graphics which are not likely to trigger a seizure

# 9. `before_save` is an example of a what? Where in our Rails application would we find a `before_save`?

callback, model

# 10. Given the following object, how would we create a scope for all users who are active?

```ruby
User.create(name: "Happy", active: true)
```


# 11. What is the difference between a scope and a class method?

scopes are chainable active record queries


### Review Questions:  
12. Given the following hash:  

```ruby
{cart: {"17" => 4, "204" => 52, "29" => 22}}
```

  12a. How would you add item with id of 48 with a quantity of 4?  
  12b. How would you increase the quantity of item 29?  
  12c. How would you find out how many items your user is thinking about purchasing?   

13. What is polymorphism? How does it relate to duck-typing? What are two ways you use this in everyday Rails applications?  
14. How would you clean the string "(630) 854-5483" to "630.854.5483"?  


### Self Assessment:
Choose One:

* I was able to answer a few questions independently, but relied heavily on outside resources

Choose One:

* I feel comfortable with the content presented this week


```ruby
<%= stylesheet_link_tag "application" %>
<%= javascript_include_tag "application" %>
<%= image_tag "rails.png" %>
```

allows application to use javascript and a stylesheet, third tag renders an image
