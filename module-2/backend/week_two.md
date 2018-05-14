## Week Two - Module 2 Recap

Fork or re-pull this respository. Answer the questions to the best of your ability. Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week (which is a TON - YOU are a web developer!!!).

Note: When you're done, submit a PR.


### Week 2 Questions

1. At a high level, what is ActiveRecord? What does it do/allow you to do?

ActiveRecord is an ORM. It allows us to easily interact with our database.


2. Assume you have the following model:


```ruby
class Team << ActiveRecord::Base
end
```

What are some methods you can call on `Team`? If these methods aren't defined in the class, how do you have access to them?


Find, group, joins are all ActiveRecord methods which the above Team class inherits.

3. Assume that in your database, a team has the following attributes: "id", "name", owner_id". How would you find the name of a team with an id of 4? Assuming your class only included the code from question 2, how could you find the owner of the same team?

Team.find(4), Team.find(4).owner_id

4. Assume that you added a line to your `Team` class as follows:

```ruby
class Team << ActiveRecord::Base
  belongs_to :owner
end
```

Now how would you find the owner of the team with an id of 4?

Team.find(4).owner

5. In a database that's holding students and teachers, what will be the relationship between students and teachers? Draw the schema diagram.

One to Many


6. Define foreign key, primary key, and schema.

Primary key = key assigned by database to each row

Foreign key = key referencing a separate table

Schema = visual representation of most recent database


7. Describe the relationship between a foreign key on one table and a primary key on another table.

a foreign key on one table is a primary key on its own table


8. What are the parts of an HTTP response?

- Status Line

- Header

- Body


### Optional Questions

1. Name your five favorite ActiveRecord methods (i.e. methods your models inherit from ActiveRecord) and describe what they do.

sum (adds numbers together)
joins (for join tables)
find_by (allows to search by attribute)
create (instantiates and saves an object)
destroy (deletes an object or resource)

2. Name your three favorite ActiveRecord rake tasks and describe what they do.

rake db:reset (resets database)
rake db:rollback (undo recent migration)
rake db:migrate (commits changes made in migration)

3. What two columns does `t.timestamps null: false` create in our database?

created at and updated at

4. In a database that's holding schools and teachers, what will be the relationship between schools and teachers?

One to Many

5. In the same database, what will you need to do to create this relationship (draw a schema diagram)?

has_many and belongs_to

6. Give an example of when you might want to store information besides ids on a join table.

Students and courses may both have a grade


7. Describe and diagram the relationship between patients and doctors.

One to Many

8. Describe and diagram the relationship between museums and original_paintings.

One to many

9. What could you see in your code that would make you think you might want to create a partial?

Repetitive styling

### Self Assessment:

* I was able to answer most questions independently, but utilized outside resources for a few


Choose One:

* I feel comfortable with the content presented this week
* I feel overwhelmed by the content presented this week

Somewhere in between these two :)
