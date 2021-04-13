# Unit 7: Connecting to the Database, Session, and User authentication

In this unit, we learn how to do the actions that are necessary to service almost all web requests, namely: 
1. Connect to the database
1. Read the user session
1. Check if the user is logged in and read the user profile. 

We will also learn how to examine the database content, which is useful in debugging your code. 

## Resources

* [Fixtures](https://py4web.com/_documentation/static/en/chapter-06.html), in the py4web documentation.
* Remember: 
    * `@action.uses(auth, ...)` makes the user information available in the controller.  
    * `@action.uses(auth.user, ...)` enforces the fact that the user has to be logged in to visit that particular page. 
* [DAL: The Database Abstraction Layer](https://py4web.com/_documentation/static/en/chapter-07.html), in the py4web documentation.
* [sqlite](https://sqlite.org/index.html), the database server that is used for development.  sqlite locks the entire database when an operation is in progress, so it is not suited to multi-user sites; it is used only in development. 

## Videos

* [Fixtures, sessions, connection to the database, user auth](https://youtu.be/kSNrwf9pO3Q)

