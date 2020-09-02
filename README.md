# unit-14-hw

Reverser Engineering Authentication Homework Assignment

Server.js

-This file is responsible for the configuration of the server that will be used for the api. This file also contains the functionality for requiring all the npm packages and routes that are also needed for the developer. The console.log displays the port being used as well. 

Package.json

-Lists all the dependencies for our web application and also contains all relevant script tags used by the developer. 

Html-routes.js

-This file contains the endpoints that the user will use to access the specific files needed to display the relevant information. There are 3 endpoints that are linked to “get” api call methods in order to retrieve the desired member, login and sign-out functionalities that are embedded in the front end markup HTML files that will take information to be later manipulated on the back end. These endpoints check to see if a member exists and/or is logged in. If a member exists they will be directed to the members html page, else they will be redirected to the sign-up page. If a member exists, and is logged in they will be redirected to the members page but if a member tries to access the members page while not logged in they will be redirected to the login page. If a user who is not logged in tries to access the members page they will be redirected to the signup page. 

Api-routes.js

- There are 4  api endpoints to “pos”t and to “get.” The endpoints are used to authenticate the login credentials of the user. The first post method checks for valid login credentials, and if the login credentials are validated it sends the user to the members page, else the credentials are invalid. The second post method is used to create login credentials via the sign-in endpoints. The email and password are the keys created on the request.body object. The user is redirected to the login endpoint, and if there is an error, the user will receive an error message. The first get method is used for logout functionality. The user is redirected to the login page. The last get method returns their email and id. If they are not logged in, they will receive an empty object. 

Login.js

The login.js file includes logic to validate the email and password, and then takes the user data and posts it to the api route that was specified in the back-end. It then updates the html on the page using the login.html file.







Members.js

The members.js file includes logic to identify which user is logged in. It then updates the html on the page using the members.html file.






Signup.js

The signup.js file includes logic to validate a new user, and then takes the user data and posts it to the api route that was specified in the back-end. It then updates the html on the page using the signup.html file.


Stylesheet

Indicates the style layout for the web page. 

Index.js

Sets up and connects to a database and creates a Sequelize instance.

User.js

Sets up a model for how user information gets input into the database.
Passport.js
Sets up the logic and the requirements for the logging in credentials of the user. 


Config.json

Setting up a mysql connection .


isAuthenticated.js

The isAuthenticated.js file includes the logic to restrict routes based on whether or not someone is logged in. If a user is logged in they are allowed access, if not they are redirected to the login page.


