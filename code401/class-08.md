# Access Control (ACL)

## Review, Research, and Discussion

1. When is Basic Authorization used vs. Bearer Authorization?

If you think that a password might be intercepted, use basic authentication with SSL.
Bearer distinguishes the type of Authorization you're using, so it's important.

2. What does the JSON Web Token package do?

that defines a compact and self-contained way for securely transmitting information between parties as a JSON object. This information can be verified and trusted because it is digitally signed.

3. What considerations should we make when creating and storing a SECRET?

- Never store unencrypted secrets in .git repositories. Avoid git add \* commands on git. Add sensitive files in .gitignore.

- Don't rely on code reviews to discover secrets.

- Don't share your secrets unencrypted in messaging systems like slack.

## Vocabulary Terms

|      Word      |                                                                                                 Definition                                                                                                  |
| :------------: | :---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------: |
|   Encryption   |                                                 is the method by which information is converted into secret code that hides the information's true meaning.                                                 |
|     Token      |                                          used in bearer authentication, a token is a cryptic string that is generated by the server in response to a login request                                          |
|     bearer     | is dedicated to the authentication using a token. Even if this scheme comes from an OAuth2 specification, you can still use it in any other context where tokens are exchange between a client and a server |
|     Secret     |                                                   is what is paired with a token, a secret string stored on the server used to sign and encode the token.                                                   |
| JSON Web Token |                     is an Internet proposed standard for creating data with optional signature and/or optional encryption whose payload holds JSON that asserts some number of claims.                      |

## RBAC

`RBAC` is the idea of assigning system access to users based on their role in an organization. It's important to remember that not every employee needs a starring role.

It's nothing more than the idea of assigning system access to users based on their role within an organization. The system needs of a given workforce are analyzed, with users grouped into roles based on common job responsibilities and system access needs.

`Role-based access control` (RBAC) is a policy-neutral access-control mechanism defined around roles and privileges. The components of RBAC such as role-permissions, user-role and role-role relationships make it simple to perform user assignments. A study by NIST has demonstrated that RBAC addresses many needs of commercial and government organizations.