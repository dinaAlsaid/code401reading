# Code 401

[PREVIOUS](https://dinaalsaid.github.io/code401reading/class-12) &nbsp;[HOME](https://dinaalsaid.github.io/reading-notes/)&nbsp;[NEXT](https://dinaalsaid.github.io/code401reading/class-14)

[table of contents](https://dinaalsaid.github.io/code401reading/)

## Review

1. Write the following steps in the correct order:

* Register your application to get a client_id and client_secret
* Ask the client if they want to sign in via a third party
* Make a request to a third-party API endpoint
* Receive authorization code
* Redirect to a third party authentication endpoint
* Make a request to the access token endpoint
* Receive access token

2. What can you do with an authorization code?
exchange it for an access token, where the user can see what the information the client is requesting, and approve or deny the request.
3. What can you do with an access token?
Allows an application to access an API
4. What’s a benefit of using OAuth instead of your own basic authentication?

## Terms

* Client ID: public information used to build login URLs
* Client Secret: will help granting tokens to only the authorised requesters
* Authentication Endpoint: where the authentication for the users is granted
* Access Token Endpoint: used by an appliction to use/ acsses the token
* API Endpoint: the point of entry in a communiction channel
* Authorization Code: exchange it for an access token, where the user can see what the information the client is requesting, and approve or deny the request.
* Access Token: a string that allows an application to access an API

## Bearer Authorization

### JWT (JSON Web Token)

Is an open standard that will help protect information sent between ant two users, where the information is digitally signed therefore trusted and secured.

can be sent in the URLs and requests. And enables fast transmission. Used with Authorization and information exchange.

structure:
1. header: contains the used encoding algorithm and the type of the token
2. payload: json format, consists of registered claims, public claims and private claims.
3. signture: will depend on the header and the payload and a secret.

Security:
*  can be either signed, encrypted or both
* if signed only, anyone can read it but it can't be changed(will know if changed)

