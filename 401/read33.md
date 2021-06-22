# Authentication & Production Server
## JSON Web Token
### JSON Web Token (JWT) is an open standard (RFC 7519) that defines a compact and self-contained way for securely transmitting information between parties as a JSON object. JWTs can be signed using a secret (with the HMAC algorithm) or a public/private key pair using RSA or ECDSA
## When should you use JSON Web Tokens?
### JSON Web Tokens are useful for:
- **Authorization**: This is the most common scenario for using JWT. Once the user is logged in, each subsequent request will include the JWT, allowing the user to access routes, services, and resources that are permitted with that token.
- **Information Exchange**: JSON Web Tokens are a good way of securely transmitting information between parties.
## What is the JSON Web Token structure?
### In its compact form, JSON Web Tokens consist of three parts separated by dots `.`, which are:
- Header
- Payload
- Signature
## How do JSON Web Tokens work?
### In authentication, when the user successfully logs in using their credentials, a JSON Web Token will be returned. Since tokens are credentials, great care must be taken to prevent security issues. In general, you should not keep tokens longer than required.
- The JWT is acquired by exchanging an username + password for an access token and an refresh token.
- The access token is usually short-lived.
- The refresh token lives a little bit longe. It is comparable to an authentication session. After it expires, you need a full login with username + password again.
## Why should we use JSON Web Tokens?
### As JSON is less verbose than XML, when it is encoded its size is also smaller, making JWT more compact than SAML. This makes JWT a good choice to be passed in HTML and HTTP environments.
