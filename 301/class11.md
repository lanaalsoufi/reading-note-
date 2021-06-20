# Authentication

## What is OAuth

**1. What is OAuth?**

OAuth is an open-standard authorization protocol or framework that describes how unrelated servers and services can safely allow authenticated access to their assets without actually sharing the initial, related, single logon credential. In authentication parlance, this is known as secure, third-party, user-agent, delegated authorization.

**2. Give an example of what using OAuth would look like.**

The simplest example of OAuth is when you go to log onto a website and it offers one or more opportunities to log on using another website’s/service’s logon. You then click on the button linked to the other website, the other website authenticates you, and the website you were originally connecting to logs you on itself afterward using permission gained from the second website.

**3. How does OAuth work? What are the steps that it takes to authenticate the user?**

1. The first website connects to the second website on behalf of the user, using OAuth, providing the user’s verified identity.

2. The second site generates a one-time token and a one-time secret unique to the transaction and parties involved.

3. The first site gives this token and secret to the initiating user’s client software.

4. The client’s software presents the request token and secret to their authorization provider (which may or may not be the second site).

5. If not already authenticated to the authorization provider, the client may be asked to authenticate. After authentication, the client is asked to approve the authorization transaction to the second website.

6. The user approves (or their software silently approves) a particular transaction type at the first website.

7. The user is given an approved access token (notice it’s no longer a request token).

8. The user gives the approved access token to the first website.

9. The first website gives the access token to the second website as proof of authentication on behalf of the user.

10. The second website lets the first website access their site on behalf of the user.

11. The user sees a successfully completed transaction occurring.

12. OAuth is not the first authentication/authorization system to work this way on behalf of the end-user.

**4. What is OpenID?**

OpenID is for humans logging into machines, OAuth is for machines logging into machines on behalf of humans."

## Authorization and Authentication flows

**1. What is the difference between authorization and authentication?**

***Authentication***

* Determines whether users are who they claim to be

* Challenges the user to validate credentials

* Usually done before authorization

* transmits info through an ID Token

* governed by the OpenID Connect

***uthorization***

* Determines what users can and cannot access

* Verifies whether access is allowed through policies and rules

* Usually done after successful authentication

* transmits info through an Access Token

* governed by the OAuth 2.0 framework

**2. What is Authorization Code Flow?**

Because regular web apps are server-side apps where the source code is not publicly exposed, they can use the Authorization Code Flow.

**3. What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)?**

The PKCE-enhanced Authorization Code Flow introduces a secret created by the calling application that can be verified by the authorization server; this secret is called the Code Verifier.

**4. What is Implicit Flow with Form Post?**

As an alternative to the Authorization Code Flow, OAuth 2.0 provides the Implicit Flow, which is intended for Public Clients, or applications which are unable to securely store Client Secrets.

**5. What is Client Credentials Flow?**

With machine-to-machine (M2M) applications, such as CLIs, daemons, or services running on your back-end, the system authenticates and authorizes the app rather than a user.

**6. What is Device Authorization Flow?**

With input-constrained devices that connect to the internet, rather than authenticate the user directly, the device asks the user to go to a link on their computer or smartphone and authorize the device.

**7. What is Resource Owner Password Flow?**

Though we do not recommend it, highly-trusted applications can use the Resource Owner Password Flow, which requests that users provide credentials (username and password), typically using an interactive form.