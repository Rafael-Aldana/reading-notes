# Express REST API

## Review: ES6 Classes

Classes are a template for creating ____.

Classes are a template for creating objects. They encapsulate data with code to work on that data. Classes in JS are built on prototypes but also have some syntax and semantics that are unique to classes.

Can a class declaration be hoisted?

Like function expressions, class expressions may be anonymous, or have a name that's different from the variable that it's assigned to. However, unlike function declarations, class declarations have the same temporal dead zone restrictions as let or const and behave as if they are not hoisted.

How would you describe a constructor and contextual “this” to a non-technical friend?

A constructor is a special function in JavaScript that is used to create objects. It is like a blueprint for creating objects of a specific type. When you call a constructor function, it creates a new object and sets its properties and methods according to the instructions in the constructor.

Contextual "this" is a concept in JavaScript that refers to the current object. It is a keyword that is used to refer to the object that the code is currently executing in. The value of "this" depends on the context in which it is used. In other words, it can change depending on how and where it is called.

So, when you use a constructor function to create a new object, you use the keyword "this" to refer to the new object that is being created. This allows you to set properties and methods on the new object, which can then be used later in your code.

## Using Express Routing

Within Express, what does routing refer to?

Routing refers to how an application’s endpoints (URIs) respond to client requests. For an introduction to routing, see Basic routing.

You define routing using methods of the Express app object that correspond to HTTP methods; for example, app.get() to handle GET requests and app.post to handle POST requests. For a full list, see app.METHOD. You can also use app.all() to handle all HTTP methods and app.use() to specify middleware as the callback function (See Using middleware for details).

These routing methods specify a callback function (sometimes called “handler functions”) called when the application receives a request to the specified route (endpoint) and HTTP method. In other words, the application “listens” for requests that match the specified route(s) and method(s), and when it detects a match, it calls the specified callback function.

In fact, the routing methods can have more than one callback function as arguments. With multiple callback functions, it is important to provide next as an argument to the callback function and then call next() within the body of the function to hand off control to the next callback.

What is the difference between a route path and a route method?

In Express, a route is a way to map incoming requests to specific actions in your application. It typically consists of two parts: a route path and a route method.

The route path in Express is a string that represents the URL path that the request should match. It can contain named parameters, optional parameters, and regular expressions to match specific patterns. For example, the route path /users/:userId would match any URL that has the /users/ path followed by a dynamic userId parameter.

The route method in Express specifies the HTTP method that the request should use. It can be any of the standard HTTP methods such as GET, POST, PUT, DELETE, etc. For example, the app.get() method specifies that this route should only respond to GET requests, while the app.post() method specifies that this route should only respond to POST requests.

When is it appropriate to add next as a parameter to a route handler and what must you do if next has been passed to your middleware as a parameter?

You can provide multiple callback functions that behave like middleware to handle a request. The only exception is that these callbacks might invoke next('route') to bypass the remaining route callbacks. You can use this mechanism to impose pre-conditions on a route, then pass control to subsequent routes if there’s no reason to proceed with the current route.

Route handlers can be in the form of a function, an array of functions, or combinations of both.

## Express Routing

What is an Express Router?

What exactly is the Express Router? It is a mini express application without all the bells and whistles of an express application, just the routing stuff. Let’s take a look at exactly what this means. We’ll go through each section of our site and use different features of the Router.

By what mean do we initialize express.Router() in an express server?

In Express, a Router is an instance of middleware that acts like a "mini" application with its own set of routes and middleware. It can be used to organize routes into separate modules or files, making your application easier to manage and maintain.

Initializing an Express Router means creating a new instance of the Router middleware, which can then be used to define routes and middleware specific to that router. To initialize an instance of the Express Router, you use the express.Router() method.

What do we use route middleware for?

In Express, route middleware is used to perform specific actions or add functionality to routes before or after the route handler function is executed. It can be used to modify the request or response objects, authenticate users, handle errors, or perform any other custom logic.

Route middleware in Express is defined using the app.use() or router.use() methods, which take a function that has access to the req, res, and next objects. The next function is used to pass control to the next middleware function or the route handler function.

[link-to-reading-notes](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Classes).
[link-to-reading-notes](https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Classes).
[link-to-reading-notes](https://scotch.io/tutorials/learn-to-use-the-new-router-in-expressjs-4).
*************************************************************************************************************

### Things I want to know more about:

How will we be using this in class?