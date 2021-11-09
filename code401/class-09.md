# Authorization/Authentication

#### What header(s) are used in authentication and authorization

- The HTTP headers Authorization header is a request type header that used to contains the credentials information to authenticate a user through a server. If the server responds with 401 Unauthorized and the WWW-Authenticate header not usually.
- Basic authentication is a simple authentication scheme built into the HTTP protocol. The client sends HTTP requests with the Authorization header that contains the word Basic word followed by a space and a base64-encoded string username:password . For example, to authorize as demo / p@55w0rd the client would send.

#### What is safe to put into a JWT

-It should be unique to your application — it needs to be a secret, after all — but it won't be unique for each token.

#### How are JWTs validated

- Retrieve and parse your Okta JSON Web Keys (JWK), which should be checked periodically and cached by your application.
- Decode the access token, which is in JSON Web Token format
- Verify the signature used to sign the access token
- Verify the claims found inside the access token

#### Document the following Vocabulary Terms

- RBAC: Role-based access control (RBAC) restricts network access based on a person's role within an organization and has become one of the main methods for advanced access control. The roles in RBAC refer to the levels of access that employees have to the network.

- User Roles: levels of access that employees have to the network.
- JWT Token: JSON Web Token (JWT) is a JSON encoded representation of a claim(s) that can be transferred between two parties. The claim is digitally signed by the issuer of the token, and the party receiving this token can later use this digital signature to prove the ownership on the claim.
