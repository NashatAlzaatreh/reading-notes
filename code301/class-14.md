# Authentication

## What is OAuth

#### - What is OAuth?

##### OAuth is an open-standard authorization protocol or framework that describes how unrelated servers and services can safely allow authenticated access to their assets without actually sharing the initial, related, single logon credential. In authentication parlance, this is known as secure, third-party, user-agent, delegated authorization.

#### - Give an example of what using OAuth would look like.

##### The simplest example of OAuth is when you go to log onto a website and it offers one or more opportunities to log on using another website’s/service’s logon. You then click on the button linked to the other website, the other website authenticates you, and the website you were originally connecting to logs you on itself afterward using permission gained from the second website.

#### - How does OAuth work? What are the steps that it takes to authenticate the user?

##### The first website connects to the second website on behalf of the user, using OAuth, providing the user’s verified identity.The second site generates a one-time token and a one-time secret unique to the transaction and parties involved.The first site gives this token and secret to the initiating user’s client software.The client’s software presents the request token and secret to their authorization provider (which may or may not be the second site).If not already authenticated to the authorization provider, the client may be asked to authenticate. After authentication, the client is asked to approve the authorization transaction to the second website.The user approves (or their software silently approves) a particular transaction type at the first website.The user is given an approved access token (notice it’s no longer a request token).The user gives the approved access token to the first website.The first website gives the access token to the second website as proof of authentication on behalf of the user.The second website lets the first website access their site on behalf of the user.The user sees a successfully completed transaction occurring.

#### - What is OpenID?

##### security technology

## Authorization and Authentication flows

#### - What is the difference between authorization and authentication?

##### Auth0 uses the OpenID Connect (OIDC) Protocol and OAuth 2.0 Authorization Framework to authenticate users and get their authorization to access protected resources.

#### - What is Authorization Code Flow?

##### Exchanges an Authorization Code for a token.

#### - What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)?

##### single-page apps have special challenges. To mitigate these, OAuth 2.0 provides a version of the Authorization Code Flow which makes use of a Proof Key for Code Exchange (PKCE)

#### - What is Implicit Flow with Form Post?

##### Implicit Flow with Form Post flow

#### - What is Client Credentials Flow?

##### Is a server to server flow. There is no user authentication involved in the process.

#### - What is Device Authorization Flow?

##### device flow", instructs the user to review the authorization request on a secondary device

#### - What is Resource Owner Password Flow?

##### Allows exchanging the username and password of a user for an access token and, optionally, a refresh token.
