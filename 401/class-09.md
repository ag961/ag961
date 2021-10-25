# Access Control (ACL)

1. What header(s) are used in authentication and authorization

```Req.headers.authorization``` is where either a username:password or a JWT token is sent. With basic authentication `Basic` is placed before encoded username:password combination. With token authentication, `Bearer` is placed in front of a token.
1. What is safe to put into a JWT

A combination of whatever is unique to a user, such as a username, and a secret string, stored in an envrironment variable.

1. How are JWTs validated

Using jwt.verify() method that accepts two parameters: a token and a secret.

## Vocabulary

- **RBAC**:  Role-based access control (RBAC) refers to the idea of assigning permissions to users based on their role within an organization. It offers a simple, manageable approach to access management that is less prone to error than assigning permissions to users individually. ([Source](https://auth0.com/docs/authorization/rbac/))
  
- **User Roles**: a collection of permissions that you can apply to users. ([Source](https://auth0.com/docs/authorization/rbac/))

- **JWT Token**: JSON web token (JWT), pronounced "jot", is an open standard (RFC 7519) that defines a compact and self-contained way for securely transmitting information between parties as a JSON object. Again, JWT is a standard, meaning that all JWTs are tokens, but not all tokens are JWTs. ([Source](https://auth0.com/docs/security/tokens/json-web-tokens))




[**<== BACK**](401-toc.md)