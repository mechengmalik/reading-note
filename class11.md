# Authentication

## OAuth

**OAuth is an open-standard authorization protocol or framework that provides applications the ability for “secure designated access.” For example, you can tell Facebook that it’s OK for ESPN.com to access your profile or post updates to your timeline without having to give ESPN your Facebook password. This minimizes risk in a major way: In the event ESPN suffers a breach, your Facebook password remains safe.**

_OAuth doesn’t share password data but instead uses authorization tokens to prove an identity between consumers and service providers. OAuth is an authentication protocol that allows you to approve one application interacting with another on your behalf without giving away your password._

## OAuth Examples

Facebook apps are a good OAuth use case example. Say you’re using an app on Facebook, and it asks you to share your profile and pictures. Facebook is, in this case, the service provider: it has your login data and your pictures. The app is the consumer, and as the user, you want to use the app to do something with your pictures. You specifically gave this app access to your pictures, which OAuth is managing in the background.

## How OAuth works

* **The first website connects to the second website on behalf of the user, using OAuth, providing the user’s verified identity.**

* **The second site generates a one-time token and a one-time secret unique to the transaction and parties involved.**

* **The first site gives this token and secret to the initiating user’s client software.**

* **The client’s software presents the request token and secret to their authorization provider (which may or may not be the second site).**

* **If not already authenticated to the authorization provider, the client may be asked to authenticate.**

* **After authentication, the client is asked to approve the authorization transaction to the second website.**

* **The user approves (or their software silently approves) a particular transaction type at the first website.**

* **The user is given an approved access token (notice it’s no longer a request token).**

* **The user gives the approved access token to the first website.**

* **The first website gives the access token to the second website as proof of authentication on behalf of the user.**

* **The second website lets the first website access their site on behalf of the user.**

* **The user sees a successfully completed transaction occurring.**

## Authorization

What's the difference between authentication and authorization?

**`**Authentication**` confirms that users are who they say they are. `**Authorization**` gives those users permission to access a resource.**

_While `authentication` and `authorization` might sound similar, they are distinct security processes in the world of identity and access management (IAM)._

## Authorization Code Flow

**Because regular web apps are server-side apps where the source code is not publicly exposed, they can use the Authorization Code Flow, which exchanges an Authorization Code for a token.**
**During authentication, mobile and native applications can use the Authorization Code Flow, but they require additional security. Additionally, single-page apps have special challenges. To mitigate these, OAuth 2.0 provides a version of the Authorization Code Flow which makes use of a Proof Key for Code Exchange `(PKCE).`**

## Implicit Flow with Form Post

**As an alternative to authorization token flow, OAuth 2.0 provides implicit flow, intended for global clients, or applications that cannot store client secrets. While this is no longer considered a best practice for requesting access tokens, when used with the form post response mode, it provides a streamlined workflow if the application only needs an ID token to perform user authentication.**

## Client Credentials Flow

**With machine-to-machine (M2M) applications, such as CLIs, daemons, or services running on your back-end, the system authenticates and authorizes the app rather than a user. For this scenario, typical authentication schemes like username + password or social logins don't make sense. Instead, M2M apps use the Client Credentials Flow**

## Device Authorization Flow

**With input-constrained devices that connect to the internet, rather than authenticate the user directly, the device asks the user to go to a link on their computer or smartphone and authorize the device. This avoids a poor user experience for devices that do not have an easy way to enter text. To do this, device apps use the Device Authorization Flow (drafted in OAuth 2.0). For use with mobile/native applications.**
