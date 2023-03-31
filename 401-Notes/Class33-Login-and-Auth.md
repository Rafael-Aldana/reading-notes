# Login and Auth

## What is Role Based Access Control (RBAC)?

What is Role Based Access Control (RBAC)?

Role-based access control (RBAC) restricts network access based on a person's role within an organization and has become one of the main methods for advanced access control. The roles in RBAC refer to the levels of access that employees have to the network.

Employees are only allowed to access the information necessary to effectively perform their job duties. Access can be based on several factors, such as authority, responsibility, and job competency. In addition, access to computer resources can be limited to specific tasks such as the ability to view, create, or modify a file.

As a result, lower-level employees usually do not have access to sensitive data if they do not need it to fulfill their responsibilities. This is especially helpful if you have many employees and use third-parties and contractors that make it difficult to closely monitor network access. Using RBAC will help in securing your company’s sensitive data and important applications.

Share some an example of RBAC including all possible CRUD operations and correlating roles.

- Admin: Can create, update,delete, read.
- Creator: Can create, read.
- Editor: Can update, read.
- User: Can read.
What are the Benefits of RBAC?

Managing and auditing network access is essential to information security. Access can and should be granted on a need-to-know basis. With hundreds or thousands of employees, security is more easily maintained by limiting unnecessary access to sensitive information based on each user’s established role within the organization. Other advantages include:

Reducing administrative work and IT support. With RBAC, you can reduce the need for paperwork and password changes when an employee is hired or changes their role. Instead, you can use RBAC to add and switch roles quickly and implement them globally across operating systems, platforms and applications. It also reduces the potential for error when assigning user permissions. This reduction in time spent on administrative tasks is just one of several economic benefits of RBAC. RBAC also helps to more easily integrate third-party users into your network by giving them pre-defined roles.
Maximizing operational efficiency. RBAC offers a streamlined approach that is logical in definition. Instead of trying to administer lower-level access control, all the roles can be aligned with the organizational structure of the business and users can do their jobs more efficiently and autonomously.
Improving compliance. All organizations are subject to federal, state and local regulations. With an RBAC system in place, companies can more easily meet statutory and regulatory requirements for privacy and confidentiality as IT departments and executives have the ability to manage how data is being accessed and used. This is especially significant for health care and financial institutions, which manage lots of sensitive data such as PHI and PCI data.

## Compare and Contrast the following two Libraries and the following questions. Yes, they are similarly named.

### react-cookie library && react-cookies component

Describe some react-cookie features.

- dependencies (optional)
- setCookie(name, value, [options])
- name (string): cookie name
- value (string|object): save the value and stringify the object if needed
- options (object): Support all the cookie options from RFC 6265
  - path (string): cookie path, use / as the path if you want your cookie to be accessible on all pages
  - expires (Date): absolute expiration date for the cookie
  - maxAge (number): relative max age of the cookie from when the client receives it in seconds
  - domain (string): domain for the cookie (sub.domain.com or .allsubdomains.com)
  - secure (boolean): Is only accessible through HTTPS?
  - httpOnly (boolean): Can only the server access the cookie? Note: You cannot get or set httpOnly cookies from the browser, only the server.
  - sameSite (boolean|none|lax|strict): Strict or Lax enforcement
- removeCookie(name, [options])
- name (string): cookie name
- options (object): Support all the cookie options from RFC 6265
  - path (string): cookie path, use / as the path if you want your cookie to be accessible on all pages
  - expires (Date): absolute expiration date for the cookie
  - maxAge (number): relative max age of the cookie from when the client receives it in seconds
  - domain (string): domain for the cookie (sub.domain.com or .allsubdomains.com)
  - secure (boolean): Is only accessible through HTTPS?
  - httpOnly (boolean): Can only the server access the cookie? Note: You cannot get or set httpOnly cookies from the browser, only the server.
  - sameSite (boolean|none|lax|strict): Strict or Lax enforcement
- withCookies(Component)
  - cookies: Cookies instance allowing you to get, set and remove cookies.
  - allCookies: All your current cookies in an object.
- get(name, [options])
Get a cookie value

  - name (string): cookie name
  - options (object):
  - doNotParse (boolean): do not convert the cookie into an object no matter what
- getAll([options])
Get all cookies

  - options (object):
  - doNotParse (boolean): do not convert the cookie into an object no matter what
- getAll([options])
Get all cookies

- options (object):
- doNotParse (boolean): do not convert the cookie into an object no matter what
- remove(name, [options])
Remove a cookie

  - name (string): cookie name
  - options (object): Support all the cookie options from RFC 6265
  - path (string): cookie path, use / as the path if you want your cookie to be accessible on all pages
  - expires (Date): absolute expiration date for the cookie
  - maxAge (number): relative max age of the cookie from when the client receives it in seconds
  - domain (string): domain for the cookie (sub.domain.com or .allsubdomains.com)
  - secure (boolean): Is only accessible through HTTPS?
  - httpOnly (boolean): Can only the server access the cookie? Note: You cannot get or set httpOnly cookies from the browser, only the server.
  - sameSite (boolean|none|lax|strict): Strict or Lax enforcement

Describe some react-cookies features.

- Isomorphic cookies!
  - To be able to access user cookies while doing server-rendering, you can use plugToRequest or setRawCookie.
- .load(name, [doNotParse])
  - Load the cookie value.
  - Returns undefined if the cookie does not exist.
  - Deserialize any cookie starting with { or [ unless dotNotParse is true.
- doNotParse
  - Type: boolean
  - Default: false
- .loadAll()
  - Load all available cookies.
  - Returns an object containing all cookies.
- .select([regex])
  - Find all the cookies with a name that match the regex.
  - Returns an object with the cookie name as the key.
- .save(name, value, [options])
Set a cookie.

name
Type: string
Required

value
Type: string||number||object
Required

options
Support all the cookie options from the RFC 6265.

Type: object

path
Cookie path.
Use / as the path if you want your cookie to be accessible on all pages.

Type: string

expires
Absolute expiration date for the cookie.

Type: object (date)

maxAge
Relative max age of the cookie from when the client receives it in seconds.

Type: number

domain
Domain for the cookie.
Use https://*.yourdomain.com if you want to access the cookie in all your subdomains.

Type: string

secure
If set true it will only be accessible through https.

Type: boolean

httpOnly
If set true it will only be accessible on the server.

Type: boolean 
- .plugToRequest(req, res): unplug()
  - Load the user cookies so you can do server-rendering and match the same result.
      Also send back to the user the new cookies.
      Work with connect or express.js by using the cookieParser middleware first.
      Use const unplug = plugToRequest(req, res) just before your renderToString.

  - Returns unplug() function so it stops setting cookies on the response.
- .setRawCookie(cookies)
  - Load the user cookies so you can do server-rendering and match the same result.
    Use setRawCookie(headers.cookie) just before your renderToString.
    Make sure it is the raw string from the request headers.

Which library would you prefer would you prefer? Why?

As a beginner level web developer I'm more familiar with seeing the react hooks syntax. For that reason I would use the first cookie library, however it looks like the second library is more decentrilized so as I gain experience I'd switch over to the second one.

[link-to-reding-notes](https://digitalguardian.com/blog/what-role-based-access-control-rbac-examples-benefits-and-more).
[link-to-reding-notes](https://www.npmjs.com/package/react-cookie).
[link-to-reding-notes](https://www.npmjs.com/package/react-cookies).

*************************************************************************************************************

### Things I want to know more about:

How will we be using this in class?
How is RBAC and Auth used in the wild.
How do you create the Auth so that not just anybody signs up and creates an admin account.