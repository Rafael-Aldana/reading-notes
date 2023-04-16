# Express, NPM, TDD, CI/CD

## An introduction to NodeJS and Express

Explain middleware, answer as though I were a non-technical recruiter.

Middleware is a type of software that acts as a bridge between different computer applications or systems. Think of it like a translator who helps two people who speak different languages communicate with each other. Middleware helps different software programs "speak" to each other by translating the information they're sending back and forth.

Express the most popular __ __ ____.

Express is the most popular Node web framework, and is the underlying library for a number of other popular Node web frameworks. It provides mechanisms to:

Write handlers for requests with different HTTP verbs at different URL paths (routes).
Integrate with "view" rendering engines in order to generate responses by inserting data into templates.
Set common web application settings like the port to use for connecting, and the location of templates that are used for rendering the response.
Add additional request processing "middleware" at any point within the request handling pipeline.

Express is “unopinionated.” What does that mean?

Opinionated frameworks are those with opinions about the "right way" to handle any particular task. They often support rapid development in a particular domain (solving problems of a particular type) because the right way to do anything is usually well-understood and well-documented. However they can be less flexible at solving problems outside their main domain, and tend to offer fewer choices for what components and approaches they can use.

Unopinionated frameworks, by contrast, have far fewer restrictions on the best way to glue components together to achieve a goal, or even what components should be used. They make it easier for developers to use the most suitable tools to complete a particular task, albeit at the cost that you need to find those components yourself.

Express is unopinionated. You can insert almost any compatible middleware you like into the request handling chain, in almost any order you like. You can structure the app in one file or multiple files, and using any directory structure. You may sometimes feel that you have too many choices!

What is a module and why is modularity useful to us as developers?

A module is a JavaScript library/file that you can import into other code using Node's require() function. Express itself is a module, as are the middleware and database libraries that we use in our Express applications. You will want to create your own modules, because this allows you to organize your code into manageable parts — a monolithic single-file application is hard to understand and maintain. Using modules also helps you manage your namespace, because only the variables you explicitly export are imported when you use a module.

## What is NPM?

What version of npm are you running on your machine?

9.6.4

What command would you type to install a library/package called ‘jshint’ into your node project?

npm install jshint --save-dev

## What is TDD?

Explain why tests are important. Please explain as though I were your non technical elder.

Tests are important because they help catch bugs and errors, ensure that code changes don't break existing functionality, and can help save time and money in the long run. Just like a building inspection helps ensure that a house is safe and secure, tests help ensure that software is safe and functional.

What are three expected benefits of testing

- many teams report significant reductions in defect rates, at the cost of a moderate increase in initial development effort
- the same teams tend to report that these overheads are more than offset by a reduction in effort in projects’ final phases
- although empirical research has so far failed to confirm this, veteran practitioners report that TDD leads to improved design qualities in the code, and more generally a higher degree of “internal” or technical quality, for instance improving the metrics of cohesion and coupling


Name at lest 2 individual pitfalls and at least 2 team pitfalls commonly encountered while writing tests.

Typical individual mistakes include:

- forgetting to run tests frequently
- writing too many tests at once
- writing tests that are too large or coarse-grained
- writing overly trivial tests, for instance omitting assertions
- writing tests for trivial code, for instance accessors

Typical team pitfalls include:

- partial adoption – only a few developers on the team use TDD
- poor maintenance of the test suite – most commonly leading to a test suite with a prohibitively long running time
- abandoned test suite (i.e. seldom or never run) – sometimes as a result of poor maintenance, sometimes as a result of team turnover

## CI/CD

What are three benefits of Continuous Integration?

Early detection of issues: Continuous Integration (CI) helps detect issues early in the development cycle. With CI, code changes are automatically tested and integrated into the codebase, which helps identify errors and issues as soon as they occur. This can save developers time and effort by catching issues before they become bigger problems.

Faster feedback loop: CI provides a fast feedback loop for developers. By automatically testing and integrating code changes, CI provides developers with quick feedback on whether their changes are working or not. This can help developers make more informed decisions about what changes to make, and can help speed up the development process.

Improved code quality: CI helps improve code quality by ensuring that code changes are tested and integrated into the codebase in a consistent and standardized way. This can help catch issues related to code style, formatting, and organization, which can lead to more readable, maintainable, and bug-free code.

What is the difference between Continuos Delivery and Continuous Deployment?

Continuous Delivery (CD) and Continuous Deployment (CI) are two related but distinct practices in the software development process.

Continuous Delivery (CD) is a practice where code changes are automatically built, tested, and prepared for release to production. The goal of CD is to ensure that code changes are always in a releasable state and can be deployed to production at any time. With CD, there is still a manual step to actually deploy the code changes to production.

Continuous Deployment (CI), on the other hand, is a practice where code changes are automatically built, tested, and deployed to production without any manual intervention. With CI, code changes are automatically released to production as soon as they pass the automated tests.

The main difference between CD and CI is that CD involves a manual step to deploy code changes to production, while CI automates the deployment process. Both practices are intended to speed up the release process and reduce the risk of errors or bugs in the production environment, but they differ in terms of the level of automation involved.

In summary, Continuous Delivery (CD) is a practice that prepares code changes for release to production, while Continuous Deployment (CI) is a practice that automates the deployment of code changes to production without any manual intervention.

Explain how GitHub fits into this process assuming the listener comes from a non-technical background

GitHub is a popular platform that provides version control, collaboration, and code hosting services. It also provides a number of features that are useful for implementing Continuous Integration (CI) and Continuous Deployment (CD) practices.

Here are a few ways that GitHub can fit into a CI/CD workflow:

Version Control: GitHub provides a powerful version control system that enables developers to track changes to their codebase over time. This is essential for implementing CI/CD practices because it allows developers to easily track changes to the code and collaborate with other team members.

Pull Requests: GitHub also provides a pull request feature that enables developers to propose changes to the codebase and have those changes reviewed by other team members. This can help ensure that code changes are thoroughly reviewed and tested before being merged into the main branch.

Integration with CI/CD tools: GitHub can integrate with a variety of CI/CD tools such as Travis CI, CircleCI, and Jenkins. This allows developers to automatically build, test, and deploy code changes as part of the development process. For example, developers can set up workflows in GitHub that trigger automated tests and deployments whenever changes are pushed to the codebase.

Deployment Environments: GitHub also provides a way to manage deployment environments using its "Environments" feature. Developers can set up different environments for testing, staging, and production, and control access to those environments using role-based access control (RBAC).

[link-to-reading-notes](https://developer.mozilla.org/en-US/docs/Learn/Server-side/Express_Nodejs/Introduction).
[link-to-reading-notes](https://docs.npmjs.com/getting-started/what-is-npm).
[link-to-reading-notes](https://www.agilealliance.org/glossary/tdd/).
[link-to-reading-notes](https://www.youtube.com/watch?v=xSv_m3KhUO8).

## Bookmark and Review

[link-to-reading-notes](https://nodejs.org/en/docs/).
[link-to-reading-notes](https://docs.npmjs.com/).
[link-to-reading-notes](https://expressjs.com/en/4x/api.html).
[link-to-reading-notes](https://www.restapitutorial.com/httpstatuscodes.html).
[link-to-reading-notes](https://github.com/visionmedia/supertest).
*************************************************************************************************************

### Things I want to know more about:

How will we be using this in class?
npm consists of three distinct components:

the website
the Command Line Interface (CLI)
the registry
npm stands for Node Package Manager. It is a command-line tool that comes with Node.js and allows developers to easily install, manage, and share packages or libraries of code that can be used in their Node.js projects.

npm has a large and growing repository of open-source packages that can be installed and used in Node.js projects. Developers can use npm to search for packages, install them in their projects, and manage dependencies between packages.

npm also allows developers to publish their own packages to the npm registry so that other developers can use them in their projects. This makes it easy for developers to share code and collaborate on projects.

In addition to managing packages, npm also provides a number of other useful features such as version management, scripts, and package publishing. Overall, npm is an essential tool for Node.js developers and plays a critical role in the Node.js ecosystem.