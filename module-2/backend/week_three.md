## Week Three Recap

### Instructions
Fork this repository. Be sure to pull the latest changes to your local repo. Answer the questions to the best of your ability.

Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week.

Note: When you're done, submit a PR with a reflection in the comments about how this exercise went for you.

### Week 3 Questions

1. What is the entry at the command line to create a new rails app?

rails new app_name


2. What do Models generally inherit from in rails?

ApplicationRecord


3. What do Controllers generally inherit from in a rails project?

ApplicationController


4. How would I create a route if I wanted to see a specific horse in my routes file assuming I'm sticking to standard conventions and that I didn't want other CRUD functionality?

resources :horse, only :show

5. What rake task is useful when looking at routes, and what information does it give you?

rails routes

gives infomation about prefix, uri, and action#Controller


6. What is an example of a route helper? When would you use them?

visit horses_path (shows an index of horses)


7. What's the difference between what `_url` and `_path` return when combined with a routes prefix?

path will return a specific path within application, url will return entire link


8. What are strong params and why are they necessary?

strong params are necessary for security, the restrict what resources can be modified by the user and which attributes are allowed


9. What role does `form_for` play in helping us create our forms?

Creates a form for a resource without having to write the whole thing in HTML


10. How does `form_for` know where to submit the user's input?


11. Create a form using a `form_for` helper to create a new `Horse`.

<%= form_for @horse |do| %>
<%= f.label :name %>
<%= f.text_field :name %>
<%= f.submit %>
<% end %>

12. Why do we want to validate our models?

to make sure all the information we are counting on ends up in the database


13. What are the steps of the DNS lookup?


### Review Questions
14. How would you call the method `prance` from within the method `move` on a `Horse` instance?

horse.move.prance

15. Given the following hash:

```ruby
furniture = {table: {height: 3, color: "red"}, purchased: true}
```
What is the different between how you would return true vs returning 3?  

furniture.purchased
furniture.table.height

16. What is inheritance?

when a class takes on the same behavior from another class

### Self Assessment:
Choose One:

* I was able to answer most questions independently, but utilized outside resources for a few

Choose One:

* I feel comfortable with the content presented this week
