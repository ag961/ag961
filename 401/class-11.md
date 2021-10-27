# Read 11: Event Driven Applications

1. Why is access control important?

Because if anyone could do anything they want with the data, the internet would be a scary place.

2. Describe an application that would need access control.

A blog site, where users can register, sign in, create a blog, edit it, and delete it if they want. Regular users only have access to modify their own blog posts, but not the others'. Admins, on the other hand, have permissions to delete/hide anyone's blog post, but not to edit them.

3. What is a role used for?

Role is used to tie the permissions/capabilites to the certain role.

4. Why is role based access control more scalable than discretionary or mandatory access control?

Because RBAC relies on user roles, two different user assigned the same role is authorized to do exactly the same thing. So, when new data is added, there is no need to add specific permissions on who can access that data specifically. Roles will dictate the access.

## Vocabulary

- **Authorization**: Allowing authenticated users to do something, based on their role;
- **Role Based Access Control**: Role-based access control (RBAC) refers to the idea of assigning permissions to users based on their role within an organization. It offers a simple, manageable approach to access management that is less prone to error than assigning permissions to users individually. ([Source](https://auth0.com/docs/authorization/rbac/))

- **Capabilities**: Capailities are tied to the role. They are whatever the role has permissions to do.




[**<== BACK**](401-toc.md)