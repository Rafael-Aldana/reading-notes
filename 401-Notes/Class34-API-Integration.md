# API Integration

## Review API Server Build

1. Explain the different between a query string parameter and a path parameter.

- A query string parameter is apart of the URL that follows a question mark (?), it is used to pass data to a web server in the form of key-value pairs.
- A path perameter in the other hand is part of the URL used to identify a specific resource for modifying that resource or retrieving information from that specific resource. Path parameters appear after the base URL and are separated by /. 

In short query string parameters describe how to look for a resource and a path parameter show the program where to look.

2. What would our API URL with a path id parameter be given the following information:
Domain: http://our-site.com
v3
model name: stuff
id: things

http://our-site.com/api/v3/stuff/things

3. We have created a dynamic API with an “interface”. Describe how that interface works to a non-technical friend.

For this app the interface or also known as the front end, can perform all of the crud functionalities. A user can read what is stored in the server or api, the user can create new products and add them to the api, the user can update the existing products as a whole or patch them if they are only changing certain things, finally the user can remove/delete products from the api.

## Review Auth Server Build

1. Describe how you would use middleware to implement basic and bearer auth.

The middle ware is going to take in a signin route and signup route. The middle ware then iether create a user or pull the user up from the db. Further more it would supply the user with an encoded token if the user exists or create an encoded token if the user is signin up. 

2. Describe the handshake necessary to implement OAuth.

The third party authentication will require a token to verify the user's credentials.

3. Describe how Role Based Access Control works to a non-technical friend.

Role Based Access Control (RBAC) is the security guard to your application allowig certain individuals access to certain information according to their role in the app. Think of it like a security guard letting people into a night club. Not everyone is allowed to go to vip areas and not everyone is allowed in the back rooms but most everyone is allowed to be in the dance floor. 

[link-to-reading-notes](https://codefellows.github.io/code-401-javascript-guide/curriculum/apps-and-libraries/api-server/).
[link-to-reading-notes](https://codefellows.github.io/code-401-javascript-guide/curriculum/apps-and-libraries/auth-server/).


*************************************************************************************************************

### Things I want to know more about:

How will we be using this in class?