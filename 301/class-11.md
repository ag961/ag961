# Authentication

## What is OAuth

Source: 
> https://www.csoonline.com/article/3216404/what-is-oauth-how-the-open-authorization-framework-works.html

1. What is OAuth?
    - Open Authorization, an open-standard authorization protocol or framework that describes how unrelated servers and services can safely allow authenticated access to their assets without actually sharing the initial, related, single logon credential.
1. Give an example of what using OAuth would look like.
    - Duo/Cisco SSO. Duo app installed on my smartphone. When I try to sogn into a website, the app on my phone asks me to onfirm the access by tapping a green button. Once I do, I logged into a website.
1. How does OAuth work? What are the steps that it takes to authenticate the user?
    - The first website connects to the second website on behalf of the user, using OAuth, providing the user’s verified identity.
    - The second site generates a one-time token and a one-time secret unique to the transaction and parties involved.
    - The first site gives this token and secret to the initiating user’s client software.
    - The client’s software presents the request token and secret to their authorization provider (which may or may not be the second site).
    - If not already authenticated to the authorization provider, the client may be asked to authenticate. After authentication, the client is asked to approve the authorization transaction to the second website.
    - The user approves (or their software silently approves) a particular transaction type at the first website.
    - The user is given an approved access token (notice it’s no longer a request token).
    - The user gives the approved access token to the first website.
    - The first website gives the access token to the second website as proof of authentication on behalf of the user.
    - The second website lets the first website access their site on behalf of the user.
    - The user sees a successfully completed transaction occurring.
1. What is OpenID?
    - OpenID is a method of authentication (loggin in), which is a layer in Oauth process, while OAuth is about authorising a transaction.

## Authorization and Authentication flows

Source:

> https://auth0.com/docs/flows

1. What is the difference between authorization and authentication?
    - authentication - logging in with a password, veryfying identity of a user. Authirization - giving permission to access something or conduct a transaction.
1. What is Authorization Code Flow?
    - a way of data flow between user, web app, Auth0 and API in order to access requested data
1. What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)?
    - it is a version of Authorization Code Flow that mitigates challenges with apps that have an additional layer of seciruty
1. What is Implicit Flow with Form Post?
    - Intended for Public Clients, or applications which are unable to securely store Client Secrets
1. What is Client Credentials Flow?
    - a system of authentication and authorization that machine-to-machine (M2M) applications use
1. What is Device Authorization Flow?
    - used by devices that don't allow for easy text input
1. What is Resource Owner Password Flow?
    - requests that users provide credentials (username and password), typically using an interactive form. Should only be used when redirect-based flows (like the Authorization Code Flow) cannot be used.


[**<== BACK**](301-toc.md)