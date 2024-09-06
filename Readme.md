---

### What is OpenID Connect?

OpenID Connect (OIDC) is an identity layer built on top of the OAuth 2.0 protocol. It allows clients (such as web applications, mobile apps, etc.) to verify the identity of users based on the authentication performed by an authorization server, as well as to obtain basic profile information about the user in an interoperable and REST-like manner¹².

### Key Points of OpenID Connect

1. **Authentication**: OIDC provides a way to authenticate users securely. It answers the question, "Who is the user currently using the application?"
2. **Identity Tokens**: OIDC uses ID tokens, which are JSON Web Tokens (JWT) that contain information about the user and the authentication event.
3. **User Info**: It allows clients to request and receive information about authenticated sessions and end-users.
4. **Single Sign-On (SSO)**: OIDC supports SSO, enabling users to log in once and gain access to multiple applications.

### How OpenID Connect is Used

1. **User Initiates Login**: The user navigates to a website or application and initiates the login process.
2. **Client Requests Authentication**: The client (relying party) sends an authentication request to the OpenID Provider (OP).
3. **Authentication and Consent**: The OP authenticates the user and obtains their consent to share profile information.
4. **Tokens Issued**: The OP issues an ID token and, optionally, an access token to the client.
5. **Client Receives Tokens**: The client uses the ID token to verify the user's identity and may use the access token to access additional resources.

### Example Usage

In the example provided, OpenID Connect is used to authenticate users and obtain their profile information. The client application sends a request to the OpenID Provider, which authenticates the user and returns an ID token. The client then uses this token to verify the user's identity and access user-specific resources.

---

¹: [How OpenID Connect Works](https://openid.net/developers/how-connect-works/)
²: [What is OpenID Connect and what do you use it for? - Auth0](https://auth0.com/intro-to-iam/what-is-openid-connect-oidc)

(1) How OpenID Connect Works. https://openid.net/developers/how-connect-works/.
(2) What is OpenID Connect and what do you use it for? - Auth0. https://auth0.com/intro-to-iam/what-is-openid-connect-oidc.
(3) What Is OpenID Connect? - Postman Blog. https://blog.postman.com/what-is-openid-connect/.
(4) OpenID Connect on the Microsoft identity platform. https://learn.microsoft.com/en-us/entra/identity-platform/v2-protocols-oidc.
