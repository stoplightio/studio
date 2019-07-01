---
tags: []
---

# API Security Schemes

API security schemes protect your API resources by authenticating apps or users
that consume your API. There are a number of standard authentication protocols
you can pick from, each with their own strengths and weaknesses. To help you get
started, the section below outlines some common schemes in use.

## Authentication Schemes

### Basic API Authentication

* Easy to implement, and supported by nearly all web servers
* Entails sending base-64 encoded username and passwords
* Usually bundled with standard framework or language library
* Should not be used without SSL, or some other data-in-transit encryption mechanism
* Can easily be combined with other security methods

> **Note**: basic authentication is susceptible to hijacks and man-in-the-middle
> attacks when no encryption is in use. Due to this limitation, this method of
> authentication is only recommended when paired with SSL.

### OAuth1.0 (Digest Scheme)

* Popular, tested, secure, signature driven, protocol
* Uses cryptographic signature, which is a mix of token secret, nonce, and other request based information
* Can be used with or without SSL

### OAuth2 (Bearer Token Scheme)

* The current OAuth2 specification eliminates need for cryptographic signatures, passwords, and usernames
* OAuth2 works with authentication scenarios called flows, these flows include:
  * Authorization Code flow
  * Implicit flow
  * Resource Owner Password flow
  * Client Credentials flow
* The OAuth 2.0 server will distribute access tokens that a client application will use to access protected resources

> Additional Information on OAuth2.0 can be found [here](https://tools.ietf.org/html/rfc6749).

### OpenID Connect Discovery

* OpenID Connect Discovery (OIDC) is based on the OAuth 2.0 protocol
* Uses a sign-in flow that permits user authentication and information access by a client app
* The user information is encoded via a secure JSON Web Token (JWT)

> Additional Information on OpenID Connect Discovery can be found [here](https://openid.net/specs/openid-connect-discovery-1_0.html)

## Best Practices

### Sensitive Information in HTTP Request URLs

Ensure that your API will not expose important information such as passwords,
API keys, and security tokens in the URL. For example, this URL can be
considered insecure because it contains an API key as a query parameter:

```
/baseurl/<uid>q=?apiKey=2123223223
```

### API Keys

Reduce the likelihood of exposing your API keys by keeping them in a file or
storage mechanism that is accessible only by the owner.

> **Note**, API Keys can be duplicated or lost so it is important to use other
> security measures apart from API keys. Consider encryption to make your API
> keys more secure.

### Validation

It is beneficial to validate your inputs and access to resources using robust
parsers. Parsing requests can help verify the validity of user requests. API
designers can perform an implicit input validation to ensure the user inputs
data with permitted characters, right syntax, and character length. Using
regular expressions can also help validate string inputs.

### Audit log

Create audit logs before and after security related events. You can also log
validation errors to detect patterns or potential attacks.

### HTTP Status Codes

Use status codes and proper error handling techniques for incoming requests to
identify potential security risks.

