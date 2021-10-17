# Bearer Authorization

1. Write the following steps in the correct order ([source](https://auth0.com/docs/authorization/flows/authorization-code-flow#how-it-works)):

    - Register your application to get a client_id and client_secret

    - Ask the client if they want to sign in via a third party

    - Redirect to a third party authentication endpoint

    - Receive authorization code

    - Make a request to the access token endpoint

    - Receive access token

    - Make a request to a third-party API endpoint

2. What can you do with an authorization code?

    - Exchange it for access token
 
3. What can you do with an access token?

    - Use it to access routes that require authentication/authorization

4. What’s a benefit of using OAuth instead of your own basic authentication?

    - It allows delegated authorization to third-party apps on behalf of a user, without actually giving that app the username/password combination. ([source](https://developer.okta.com/blog/2017/06/21/what-the-heck-is-oauth))

## Vocabulary

- Client ID - public identifier for the app using the authorization service
- Client Secret - a secret known only to the application and the authorization server.
- Authentication Endpoint - it is a URL where the user is sent to get the authorization code
- Access Token Endpoint - the endpoint to receive an access token
- API Endpoint - final destination once access has been granted
- Authorization Code - a one time code to be exchanged for a token
- Access Token - allows to perform authorized actions

([source](https://www.oauth.com/))

## Resources

[JWTs Explained](https://www.youtube.com/watch?v=926mknSW9Lo)
[Intro to JWT](https://jwt.io/introduction/)
[Are JWTs Secure?](https://stackoverflow.com/questions/27301557/if-you-can-decode-jwt-how-are-they-secure)
[npm jsonwebtoken docs](https://www.npmjs.com/package/jsonwebtoken)

[**<== BACK**](401-toc.md)