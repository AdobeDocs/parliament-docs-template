# How to write effective Authorization/Authentication

Before users can make requests with your API, they'll usually need to register for an API key or learn other ways to authenticate the requests. APIs vary in the way they authenticate users. Some APIs require you to include an API key in the request header, while other APIs require elaborate security due to the need to protect sensitive data, prove identity, and ensure the requests aren't tampered with. In this section, you'll learn more about authentication and authorization and what you should focus on in documentation.

## Defining terms

First, let's define some key terms:

* **Authentication**: Refers to proving correct identity
* **Authorization**: Refers to allowing a certain action

## Consequences if an API lacks security

Why do APIs even need authentication? For read-only APIs, sometimes users don't need keys. But most commercial APIs do require authorization in the form of API keys or other methods. If you *didn't* have any security with your API, users could make unlimited amounts of API calls without any kind of registration. Allowing unrestricted requests would make a revenue model for your API difficult.

Additionally, without authentication, there wouldn't be an easy way to associate requests with specific user data. And there wouldn't be a way to protect against requests from malicious users that might delete another user's data (such as by making DELETE requests on another's account).

Finally, you couldn't track who is using your API, or what endpoints are most used. Clearly, API developers must think about ways to authenticate and authorize requests made to their API.

Overall, authentication and authorization with APIs serves the following purposes:

* Authenticate calls to the API to registered users only
* Track who is making the requests
* Track usage of the API
* Block or throttle any requester who exceeds the rate limits
* Apply different permission levels to different users

## What to document with authentication

In API documentation, you don't need to explain how your authentication works in detail to outside users. In fact, *not* explaining the internal details of your authentication process is probably a best practice as it would make it harder for hackers to abuse the API.

However, you do need to explain some necessary information such as:

* How to get API keys
* How to authenticate requests
* Error messages related to invalid authentication
* Sensitivity around authentication information
* Token expiration times

If you have public and private keys, you should explain where each key should be used, and note that private keys should not be shared. If different license tiers provide different access to the API calls, these licensing tiers should be explicit in your authorization section or elsewhere.

Since the API keys section is usually essential before developers can start using the API, this section needs to appear at the beginning of your help.

Your audience should be able to identify the information about authorization for requests to the API. Make sure you cover the topics that answers the following questions:

1. What kind of authorization is required to make requests to the API?
2. Are there different access levels within the authorization (for example, free versus pro tiers) that determine how many requests you can make or the types of information you can access?
3. Are you able to get an API key or whatever authorization method is required to make test calls to the API?
4. How is the information about authorization integrated into the getting started tutorial?