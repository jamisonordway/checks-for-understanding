week_one.md

## Week One - Module 2 Recap

Fork this respository. Answer the questions to the best of your ability. Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week (which is a TON!).

Note: When you're done, submit a PR.

### Week 1 Questions

1. List the five common HTTP verbs and what the purpose is of each verb.

GET, retrieves a page from server
POST, sends information to server
PUT, edits entirety of information sent to server
PATCH, edits a specific part of information sent to server
DELETE, removes resource from the server/database

2. What is Sinatra?

A web application library written in Ruby

4. What is MVC?

Model, View, Controller


5. Why do we follow conventions when creating our actions/path names in our Sinatra routes?

ReSTful routes

6. What types of variables are accessible in our view templates without explicitly passing them?



7. Given the following block of code, how would I pass an instance variable `count` with a value of `1` to my `index.erb` template?

  ```ruby
  get '/horses' do
    erb :index
  end
  ```


  <%= horses.count %>

8. In the same code block, how would I pass a local variable `name` with a value of `Mr. Ed` to the view?

<%= horses.find(name: 'Mr. Ed')%>

9. What's the purpose of ERB?

To imbed Ruby into HTML code which is rendered in View.

10. Why do I need a development AND test database?

In order to test without affecting any important data.

11. What is CRUD and why is it important?

Create, Read, Update, Delete: this is the list of operations that can be performed on a resource

12. What does HTTP stand for?

Hypertext Transfer Protocol

13. What are the two ways to interpolate Ruby in an ERB view template? What's the difference between these two ways?

<% something %> will not return 'something' but <%= something %> will return 'something'


14. What's an ORM?

Object Relational  Mapper


15. What's the most commonly used ORM in ruby (Sinatra & Rails)?

ActiveRecord


16. Let's say we have an application with restaurants. There are seven verb + path combinations necessary to provide full CRUD functionality for our restaurant application. List each of the seven combinations, and explain what each is for.

GET '/restaurants/'         <- to list all restaurants
GET '/restaurants/new'      <- to show new restaurant form
POST '/restaurants'         <- to submit and create new restaurant
GET '/restaurants/:id'      <- to show a specific restaurant
GET '/restaurants/:id/edit' <- to get edit restaurant form
PUT '/restaurants/:id'      <- to submit and edit restaurant
DELETE '/restaurants/:id'   <- to delete a restaurant

17. What's a migration?

Like a version control commit for databases -- allows updates


18. When you create a migration, does it automatically modify your database?

No, the migration must be edited in the 'change' block and then rake db:migrate must be run


19. How does a model relate to a database?

The model retreives information from the database and returns it to the controller.


20. What is the difference between `#new` and `#create`?

New does not add an instance to the database table.

### Review Questions:  
21. Given a CSV file (“films.csv”) with these headers [id, title, description], how would you load these into your database to create new instances of Film?  

I can't do this from memory and I would really like to go over it again in flex hour :)


22. Given the following hash:
```
activities = {
  hiking: {cost: $0, supplies: ['hiking shoes', 'water', 'compass']},
  karaoke: {cost: $10, supplies: ['courage', 'microphone'],
  brunch: {cost: $35, supplies: ['mimosa flutes'],
  antiquing: {cost: $200, supplies: ['list of antique stores']
}
```
How would I add 'granola bar' to things you should have when hiking?

'granola bar' = activities[0][supplies]


23. What are the 4 Principles of OOP? Give a one sentence explanation of each.

Encapsulation = scope & proper protection of data
Inheritance = elements can inherit methods/behaviors from each other
Abstraction = using encapsulation to divide program into logical components
Polymorphism =


### Self Assessment:
Choose One:

* I was able to answer most questions independently, but utilized outside resources for a few

Choose One:

* I feel comfortable with the content presented this week
