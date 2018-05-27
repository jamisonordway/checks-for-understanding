## Week Four Recap

### Instructions
Fork or re-pull this repository. Answer the questions to the best of your ability.

Try to answer them with limited amount of external research. These questions cover the majority of what we've learned this week.

Note: When you're done, submit a PR with a reflection in the comments about how this exercise went for you.

### Week 4 Questions

1. What is a cookie?

  a small piece of data sent from a server and stored on the client's browser

2. What’s the difference between a session and a cookie?

sessions are stored in the server and can store more data

3. What’s a flash and when do you want to use flashes?

for a popup message, such as "could not log in"

4. Why do people say “HTTP is stateless”?

it does not retain session information once the connection ends

5. What’s authentication? Explain.

Authentication is about recognizing who the user is.

6. What’s the difference between authentication and authorization?

Authorization is what that user is allowed to do.

7. What’s a before filter?

executes a piece of code before running an action from the controller.

8. How do we keep track of a user once they’ve logged in?

Using sessions (session should contain User id)

9. When do you want to namespace a resource? When do you want to nest a resource? What's the differences between those two approaches?

namespacing allows for group and as, which is better for authorization purposes. nesting may be more appropriate for connecting one-to-many relationships and routing appropriately.

10. At a high level, what tools can you use to implement authorization? How would you use them?

before_action, a method to check if a current user is logged in or an admin, namespacing and branch logic to keep private pages only visible to authorized users

11. What's an enum, and what advantages does it offer? What data type needs to be in your database to use an enum? Where do you declare an enum?

An enum is declared in the model. In the database, it is an integer. With an enum, the integer in the database will be translated to a string. This is great for authorizing types of users.

12. What are some strategies you can use to keep your views DRY?

using partials and putting universal elements such as a nav bar in the application.html.erb file

### Reviews Questions
13. Given the following array of hashes, how would I print an alphabetical list of holidays?
```ruby
[
 {holiday: {name: "St Patrick's Day", supplies: ["Corned Beef and Cabbage"]},
 {holiday: {name: "Halloween", supplies: ["Candy", "Costume"]},
 {holiday: {name: "Hanukkah", supplies: ["Menorah"]}
]
```  

holidays = _
holidays.each do |holiday|
holiday.order(name ASC)
end

14. How would you clean incoming data to ensure "$300" or "300.00" is stored as 300?

I don't know and I don't know what to google :(

  
### Self Assessment:

* I was able to answer a few questions independently, but relied heavily on outside resources

Choose One:

* I feel overwhelmed by the content presented this week
