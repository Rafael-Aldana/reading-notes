# Event Driven Applications

## Event Driven Programming

What native Node.js module allows us to get started with Event Driven Programming?

EventEmitter
Node.js natively provides us with a useful module called EventEmitter that allows us to get started incorporating Event-Driven Programming in our project right away. Of course, creating our own version of EventEmitter wouldn’t be much of a challange, and in fact there are several modules published on npm such as EventEmitter2 and EventEmitter3 which promise a faster performance than the native EventEmitter.

What is the value of Object Oriented Programming used in tandem with Event Driven Programming?

Object Oriented Programming + Event-Driven Programming
The last thing I want to touch on here is the combination of the Object Oriented and Event-driven programming paradigms. These two make for a very valuable combination in a wide variety of situations and I think it can be beneficial to understand and conceptualize why.

The Object Oriented approach promotes the idea that all behavior of an individual unit (or object) be handled from code within that unit. Using this approach, applications are built with many different units that all speak to and interact with each other.

Imagine we’re building a mail application. We might have an object whose sole purpose is to process the incoming and outgoing mail messages for our client. This object would contain all of its own behavioral functions. We might have a sendMail function that delivers our mail to a server. We might also have a receiveMail function that tells the server to deliver us any new mail it has for us. We’ll call the object responsible for these server interactions our Mailbox.

Consider your knowledge of Event Driven Programming in the Web Browser, now explain to a non-technical friend how Event Driven Programming might be useful on the backend using Node.js.

Event-driven programming can be just as useful on the backend as it is on the frontend. It allows for asynchronous, non-blocking processing of requests and can help create more modular, scalable code that is easier to maintain and modify.

[link-to-reading-notes](https://www.digitalocean.com/community/tutorials/nodejs-event-driven-programming).

## Bookmark and Review

[link-to-reading-notes](https://nodejs.org/api/events.html).

*************************************************************************************************************

### Things I want to know more about:

How will we be using this in class?