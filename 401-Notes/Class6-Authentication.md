# Authentication

## Securing Passwords

Explain to a non-technical friend how you would safely hash and store a password.

When it comes to password storage, the most important thing is to keep passwords safe and secure, so that even if someone gains unauthorized access to the database, they won't be able to read the passwords in plain text.

One way to achieve this is by using a hashing algorithm to encrypt the passwords before storing them in the database. A hash function is a one-way function that takes an input (in this case, a password) and produces a fixed-size output (the hash value). Hash functions are designed in such a way that it's computationally infeasible to reverse the process and obtain the original input from the hash value.

To safely hash and store a password, we typically follow the following steps:

Generate a random salt: A salt is a random string that's added to the password before hashing to make it harder to crack. Salting the password means that even if two users have the same password, their hash values will be different because of the different salts used.

Hash the password: Use a secure hashing algorithm like bcrypt or scrypt to generate a hash value of the password combined with the salt.

Store the salt and the hash value: Store both the salt and the hash value in the database. This way, when a user logs in, we can retrieve the salt and the hash value for that user, combine the password they entered with the salt, and compare the resulting hash value with the one stored in the database. If they match, we know the password is correct.

By using a salt and a secure hashing algorithm, we can ensure that even if someone gains access to the database, they won't be able to read the passwords in plain text. Instead, they will see only the salt and the hash value, which are essentially useless without knowing the original password.

What is Bcrypt?

Bcrypt is an adaptive hash function based on the Blowfish symmetric block cipher cryptographic algorithm and introduces a work factor (also known as security factor), which allows you to determine how expensive the hash function will be.

Why might you use something like Bcrypt?

One reason to use Bcrypt over other hashing algorithms is that it uses a salt and a cost parameter, both of which add an extra layer of security. The salt is a random string that's added to the password before hashing, which makes it impossible for two users with the same password to have the same hash value. The cost parameter determines how many times the password is hashed, which can be adjusted to make the hash function even slower.

Another reason to use Bcrypt is that it's a well-known and tested algorithm that's been around for a long time. This means that there are no known vulnerabilities or weaknesses that attackers can exploit.

Overall, Bcrypt is a good choice for password hashing because it's slow, uses a salt and a cost parameter, and has a proven track record of security. It's important to note that while Bcrypt is a great tool for securing passwords, it's not a silver bullet. It's still important to follow best practices for web application security, such as using SSL/TLS encryption, implementing two-factor authentication, and keeping software up-to-date.

## Basic Auth

What is Basic Authentication?

 Basic authentication (BA) implementation is the simplest technique for enforcing access controls to web resources because it does not require cookies, session identifiers, or login pages; rather, HTTP Basic authentication uses standard fields in the HTTP header.

What properties are necessary in the header of a Basic Auth request?

The header of a Basic Auth request should contain the Authorization property, which is used to authenticate a user. The Authorization property consists of the word "Basic" followed by a space and then the Base64-encoded string of the username and password.

How are username:password in Basic Auth encoded?

In Basic Auth, the username and password are combined into a single string of the form "username:password". This string is then Base64-encoded before being sent in the Authorization header of an HTTP request.

For example, if the username is "john" and the password is "pass123", the combined string would be "john:pass123". This string is then Base64-encoded, resulting in the string "am9objpwYXNzMTIz". This encoded string is then included in the Authorization header of the HTTP request, preceded by the word "Basic" and a space.

## OWASP auth cheatsheet

Define the authentication process to a non-technical recruiter.

Authentication is the process of verifying that an individual, entity or website is whom it claims to be. Authentication in the context of web applications is commonly performed by submitting a username or ID and one or more items of private information that only a given user should know.

How should your error messaging respond (both HTTP and HTML)? Why?

Authentication and Error Messages¶
Incorrectly implemented error messages in the case of authentication functionality can be used for the purposes of user ID and password enumeration. An application should respond (both HTTP and HTML) in a generic manner.

Authentication Responses¶
Using any of the authentication mechanisms (login, password reset or password recovery), an application must respond with a generic error message regardless of whether:

The user ID or password was incorrect.
The account does not exist.
The account is locked or disabled.
The account registration feature should also be taken into consideration, and the same approach of generic error message can be applied regarding the case in which the user exists.

The objective is to prevent the creation of a discrepancy factor, allowing an attacker to mount a user enumeration action against the application.

It is interesting to note that the business logic itself can bring a discrepancy factor related to the processing time taken. Indeed, depending on the implementation, the processing time can be significantly different according to the case (success vs failure) allowing an attacker to mount a time-based attack (delta of some seconds for example).

Bookmark this link also and consider OWASP fundamentals any time you interact with authentication. Applications developed with security in mind from inception have fewer vulnerabilities throughout their lifecycle.

This code will go through the same process no matter what the user or the password is, allowing the application to return in approximately the same response time.

The problem with returning a generic error message for the user is a User Experience (UX) matter. A legitimate user might feel confused with the generic messages, thus making it hard for them to use the application, and might after several retries, leave the application because of its complexity. The decision to return a generic error message can be determined based on the criticality of the application and its data. For example, for critical applications, the team can decide that under the failure scenario, a user will always be redirected to the support page and a generic error message will be returned.

Regarding the user enumeration itself, protection against brute-force attack is also effective because they prevent an attacker from applying the enumeration at scale. Usage of CAPTCHA can be applied on a feature for which a generic error message cannot be returned because the user experience must be preserved.

[link-to-reading-notes](https://thehackernews.com/2014/04/securing-passwords-with-bcrypt-hashing.html).
[link-to-reading-notes](https://en.wikipedia.org/wiki/Basic_access_authentication).
[link-to-reading-notes](https://www.owasp.org/index.php/Authentication_Cheat_Sheet).

## Bookmark and Review

[link-to-reading-notes](https://www.npmjs.com/package/bcrypt).

*************************************************************************************************************

### Things I want to know more about:

How will we be using this in class?