# HTTP Status Codes

 **status code is a number higher than 100 and smaller than 600 that is part of a HTTP response. The first digit defines the class of the status. A status code comes with a reason phrase. The code is for programmatic recognition the phrase is for humans to understand what happened.**

## Status Classes

* **`100 - 199`**
 **tell the client that the header part of the request has been received and the server will try to comply with a transmission demand of the client. Like using a different protocol or telling the client that its request will fail before they start sending the body.**

* **`200 - 299`**
**it met all validation requirements at the time of sending.**

* **`300 - 399`**
**the resource they are requested isn’t available at the expected location anymore.**

* **`400 - 499`**
**invalid requests a client sent to a server.**

* **`500 - 599`**
**the server error codes,problems with overwhelmed servers or unreachable servers behind proxies,**

## Status Codes

* **`202 Accepted -` Often used for asynchronous processing. This code tells the client that the request was valid, but its processing will finish sometime in the future. The response body should include an URL to the finished resource with some information about when it will be available, or an URL to some monitoring endpoint that tells the client when the resource is available.**

* **`308 Permanent Redirect -` This tells the client to use another URL to access the resource and not use the current URL anymore. It’s helpful when we have multiple endpoints for one resource, but don’t want to implement reading from all of them.**

* **`204 No Content -` A proper code for updates that don’t return data to the client, for example when just saving a currently edited document.**

* **`308 Permanent Redirect -` This is the right code if the resource will now be available at a new URL and the client should directly access it via the new URL in the future. The current endpoint can’t control the clients’ behavior after the request and a subsequent redirect if the resource URL changes again have to be issued from the new URL.**


## Middleware 

**Middleware** _is software that provides common services and capabilities to applications outside of what’s offered by the operating system. Data management, application services, messaging, authentication, and API management are all commonly handled by middleware._

**Middleware** _helps developers build applications more efficiently. It acts like the connective tissue between applications, data, and users._

_For organizations with multi-cloud and containerized environments, middleware can make it cost-effective to develop and run applications at scale._

## app.use(express.json())

**express. json()** _is a method inbuilt in express to recognize the incoming Request Object as a JSON Object. This method is called as a middleware in your application using the code: app._

## Difference between PUT and PATCH

**The main difference between the PUT and PATCH method is that the PUT method uses the request URI to supply a modified version of the requested resource which replaces the original version of the resource, whereas the PATCH method supplies a set of instructions to modify the resource.**
