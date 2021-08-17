# Rest

**REST is an architectural style for building distributed systems based on hypermedia. REST is independent of any underlying protocol and is not necessarily tied to HTTP. However, most common REST API implementations use HTTP as the application protocol, and this guide focuses on designing REST APIs for HTTP.**

## Principles of RESTful APIs using HTTP

* _REST APIs are designed around resources, which are any kind of object, data, or service that can be accessed by the client._

* _A resource has an identifier, which is a URI that uniquely identifies that resource. For example, the URI for a particular customer order might be_

* _Clients interact with a service by exchanging representations of resources. Many web APIs use JSON as the exchange format. For example, a GET request to the URI listed above might return this response body_

## URLs

**URIs are at the heart of the Web: we use them both intentionally and without realising it every time we take advantage of the myriad possibilities the Web offers us. Their use is evolving in a number of directions, not all obviously compatible with one another, or with their original conception and the basic technical framework which supported them when the Web was young. Understanding all this is a necessary and worthwhile challenge, both from the perspective of scientific enquiry (just what are these things?) and from the perspective of stewardship (how do we ensure that the Web will continue to work well for everyone?). Insights into these questions may come from surprisingly distant quarters, as well as from observation of everyday use and practice.**

### Factors that makes up a good URI

*_Stability over time_

* _Short_
* _Give the user an idea what is linked
* _Easy to type_
* _Easy to guess (relevant only for a few links like "/jobs")_
* _Search engine friendly_
* _URI schema should be consistent over the whole site_
* _URI schema should allow future extensions_


#### **Examples**

`example.com/articles/3252`
`example.com/articles/how+to+design+good``+uri`
`example.com/articles/3252/how+to+design+good+uri`
`example.com/good-uri-design`
`example.com/articles/good-uri-design`
`example.com/a/good-uri-design`

## API operations in terms of HTTP methods

* _GET retrieves a representation of the resource at the specified URI. The body of the response message contains the details of the requested resource._

* _POST creates a new resource at the specified URI. The body of the request message provides the details of the new resource. Note that POST can also be used to trigger operations that don't actually create resources._

* _PUT either creates or replaces the resource at the specified URI. The body of the request message specifies the resource to be created or updated._

* _PATCH performs a partial update of a resource. The request body specifies the set of changes to apply to the resource._

* _DELETE removes the resource at the specified URI._

