# Authentication

This reading topic is important because going into project week we'll need to use a login/authenication feature in our app.

## What is OAuth

What is OAuth?
OAuth is an open-standard authorization protocol or framework that describes how unrelated servers and services can safely allow authenticated access to their assets without actually sharing the initial, related, single logon credential. In authentication parlance, this is known as secure, third-party, user-agent, delegated authorization

Give an example of what using OAuth would look like.
Using github to signin to a website like netlify or render.

How does OAuth work? What are the steps that it takes to authenticate the user?

The first website connects to the second website on behalf of the user, using OAuth, providing the user’s verified identity.
The second site generates a one-time token and a one-time secret unique to the transaction and parties involved.
The first site gives this token and secret to the initiating user’s client software.
The client’s software presents the request token and secret to their authorization provider (which may or may not be the second site).
If not already authenticated to the authorization provider, the client may be asked to authenticate. After authentication, the client is asked to approve the authorization transaction to the second website.
The user approves (or their software silently approves) a particular transaction type at the first website.
The user is given an approved access token (notice it’s no longer a request token).
The user gives the approved access token to the first website.
The first website gives the access token to the second website as proof of authentication on behalf of the user.
The second website lets the first website access their site on behalf of the user.
The user sees a successfully completed transaction occurring.
OAuth is not the first authentication/authorization system to work this way on behalf of the end-user. In fact, many authentication systems, notably Kerberos, work similarly. What is special about OAuth is its ability to work across the web and its wide adoption. It succeeded with adoption rates where previous attempts failed (for various reasons).

What is OpenID?
OpenID is an authentication for humans to sign in and use machines. OpenID was supposed to be a single sign in process for users instead of having multiple logins for different websites.

[link-to-reding-notes](https://www.csoonline.com/article/3216404/what-is-oauth-how-the-open-authorization-framework-works.html).

********************************************************************************************************************

## Authorization and Authentication flows

What is the difference between authorization and authentication?
Authorization is the process of verifying what a user has access to and authentication is the process of verifying who the user is.

What is Authorization Code Flow?

1. The user clicks Login within the regular web application.

2. Auth0's SDK redirects the user to the Auth0 Authorization Server (
/authorize
endpoint).

3. Your Auth0 Authorization Server redirects the user to the login and authorization prompt.

4. The user authenticates using one of the configured login options and may see a consent page listing the permissions Auth0 will give to the regular web application.

5. Your Auth0 Authorization Server redirects the user back to the application with an authorization code, which is good for one use.

6. Auth0's SDK sends this code to the Auth0 Authorization Server (
/oauth/token
endpoint) along with the application's Client ID and Client Secret.

7. Your Auth0 Authorization Server verifies the code, Client ID, and Client Secret.

8. Your Auth0 Authorization Server responds with an ID Token and Access Token (and optionally, a Refresh Token).

9. Your application can use the Access Token to call an API to access information about the user.

10. The API responds with requested data.

What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)?

1. The user clicks Login within the application.

2. Auth0's SDK creates a cryptographically-random code_verifier and from this generates a code_challenge.

3. Auth0's SDK redirects the user to the Auth0 Authorization Server (
/authorize
endpoint) along with the code_challenge.

4. Your Auth0 Authorization Server redirects the user to the login and authorization prompt.

5. The user authenticates using one of the configured login options and may see a consent page listing the permissions Auth0 will give to the application.

6. Your Auth0 Authorization Server stores the code_challenge and redirects the user back to the application with an authorization code, which is good for one use.

7. Auth0's SDK sends this code and the code_verifier (created in step 2) to the Auth0 Authorization Server (
/oauth/token
endpoint).

8. Your Auth0 Authorization Server verifies the code_challenge and code_verifier.

9. Your Auth0 Authorization Server responds with an ID token and access token (and optionally, a refresh token).

10. Your application can use the access token to call an API to access information about the user.

11. The API responds with requested data.

What is Implicit Flow with Form Post?

1. The user clicks Login in the app.

2. Auth0's SDK redirects the user to the Auth0 Authorization Server (/authorize endpoint) passing along a response_type parameter of id_token that indicates the type of requested credential. It also passes along a response_mode parameter of form_post to ensure security.

3. Your Auth0 Authorization Server redirects the user to the login and authorization prompt.

4. The user authenticates using one of the configured login options and may see a consent page listing the permissions Auth0 will give to the app.

5. Your Auth0 Authorization Server redirects the user back to the app with an ID Token.

What is Client Credentials Flow?

1. The application authenticates with the Auth0 Authorization Server using its Client ID and Client Secret (
/oauth/token
endpoint).

2. Auth0 Authorization Server validates the Client ID and Client Secret.

3. Auth0 Authorization Server responds with an Access Token.

4. The application can use the access token to call an API on behalf of itself.

5. The API responds with requested data.

What is Device Authorization Flow?

Device Flow

1. The user starts the app on the device.

2. The device app requests authorization from the Auth0 Authorization Server using its Client ID (/oauth/device/code endpoint).

3. The Auth0 Authorization Server responds with a device_code, user_code, verification_uri, verification_uri_complete expires_in (lifetime in seconds for device_code and user_code), and polling interval.

4. The device app asks the user to activate using their computer or smartphone. The app may accomplish this by:

    1. asking the user to visit the verification_uri and enter the user_code after displaying these values on-screen

    2. asking the user to interact with either a QR Code or shortened URL with embedded user code generated from the verification_uri_complete

    3. directly navigating to the verification page with embedded user code using verification_uri_complete, if running natively on a browser-based device

5. The device app begins polling your Auth0 Authorization Server for an Access Token (/oauth/token endpoint) using the time period specified by interval and counting from receipt of the last polling request's response. The device app continues polling until either the user completes the browser flow path or the user code expires.

6. When the user successfully completes the browser flow path, your Auth0 Authorization Server responds with an Access Token (and optionally, a Refresh Token). The device app should now forget its device_code because it will expire.

7. Your device app can use the Access Token to call an API to access information about the user.

8. The API responds with requested data.

Browser Flow

1. The user visits the verification_uri on their computer, enters the user_code and confirms that the device that is being activated is displaying the user_code. If the user visits the verification_uri_complete by any other mechanism (such as by scanning a QR code), only the device confirmation will be needed.

2. Your Auth0 Authorization Server redirects the user to the login and consent prompt, if needed.

3. The user authenticates using one of the configured login options and may see a consent page asking to authorize the device app.

4. Your device app is authorized to access the API.

What is Resource Owner Password Flow?

1. The user clicks Login within the application and enters their credentials.

2. Your application forwards the user's credentials to your Auth0 Authorization Server (
/oauth/token
endpoint).

3. Your Auth0 Authorization Server validates the credentials.

4. Your Auth0 Authorization Server responds with an Access Token (and optionally, a Refresh Token).

5. Your application can use the Access Token to call an API to access information about the user.

6. The API responds with requested data.

[link-to-reding-notes](https://auth0.com/docs/flows).

### Things I want to know more about

I want to know more about how Auth0 works with bigger applications like Facebook, Twitter, and Google.
