Q no 1:- What is API:

API stands for application programming interface, a concept that applies everywhere from command-line tools to enterprise Java code to Ruby on Rails web apps. An API is a way to programmatically interact with a separate software component or resource.Unless you write every single line of code from scratch, you’re going to be interacting with external software components, each with its own API. Even if you do write something entirely from scratch, a well-designed software application will have internal APIs to help organize code and make components more reusable. And there are numerous public APIs that allow you to tap into functionality developed elsewhere over the web.

An API is defined as a specification of possible interactions with a software component. What does that mean, exactly? Well, imagine that a car was a software component. Its API would include information about what it can do—accelerate, brake, turn on the radio, etc. It would also include information about how you could make it do those things. For instance, to accelerate, you put your foot on the gas pedal and push.

The API doesn’t have to explain what happens inside the engine when you put your foot on the accelerator. That’s why, if you learned to drive a car with an internal combustion engine, you can get behind the wheel of an electric car without having to learn a whole new set of skills. The what and how information come together in the API definition, which is abstract and separate from the car itself.

 Give 3 real-life examples of usage of API:



(1). Weather Snippets

Google utilizes APIs to display relevant data from user search queries.
One common API usage example we come across on a daily basis is weather data. Rich weather snippets seem to be commonplace, found on all platforms, like Google Search, Apple’s Weather app, or even from your smart home device. For example, if you search “weather + [your city’s name]” on Google, you’ll see a dedicated box at the top of the search results (called a rich snippet) with the current weather conditions and forecast. As an example, here’s the search for “weather new york”.
Google isn’t in the business of weather data (yet!), so they source this information from a third party. They do so by means of an API, which sends them the latest weather details in a way that’s easy for them to reformat. As we’ve previously covered, there are many weather APIs that power this kind of functionality.
Clarification: Previously, Google used the Weather Underground API. That service is now a part of IBM’s The Weather Company, which the weather snippet currently links to in the bottom left corner.



(2). Log-in Using XYZ

Taken from Buffer’s social login
Another prominent example of API usage is the “log-in using Facebook/Twitter/Google/Github” functionality you see on so many websites. It’s incredibly convenient, but have you ever wondered how it works?
Instead of actually logging-in to users’ social media accounts (which would pose a serious security concern), applications with this functionality leverage these platforms’ APIs to authenticate the user with each login. For example, here’s the Facebook Login API.
The way it works is pretty simple. Every time the application loads, it uses the API to check whether the user is already logged in by means of whatever social media platform. If not, when the user clicks the “Log-in Using XYZ” button, a pop-up opens where they are asked to confirm they actually want to log-in with that social media profile. When the user confirms, the API provides the application with identification information, so it knows who’s logging in.
Also Read: 5 Powerful Alternatives to Google Maps API




(3). Pay with PayPal

Most online stores offer Paypal and other payment methods, utilizing API connections to these services.
Ever used PayPal to pay for something, directly within an eCommerce store? Yep, that’s also an API at work. Just like with logging-in using a social media service, the “Pay with PayPal” functionality is built with APIs to ensure that the end application can only do what it needs to, without being exposed to sensitive data or gaining access to unintended permissions.
In terms of the inner-workings of this handy function, it’s very similar to the log-in process described above. When the user clicks the “Pay with PayPal” button, the application sends an “order” request to the PayPal API, specifying the amount owed and other important details. Then, a pop-up authenticates the user and confirms their purchase. Finally, if everything goes to plan, the API sends confirmation of payment back to the application.
 
 
2APIs have become the center of software development, connecting and transferring data and logic across disparate systems and applications. Luckily, testing them can greatly improve the efficiency of your testing strategy as a whole, helping you deliver software faster than ever.
APIs, or Application Programming Interfaces, are the connecting tissue between different systems or layers of an application. Applications often have three layers: a data layer, a service (API) layer, and a presentation (UI) layer. The API layer contains the business logic of an application - the rules of how users can interact with services, data, or functions of the app.  Because the API or service layer directly touches both the data layer and the presentation layer, it presents the sweet spot of continuous testing for QA and Development teams. While traditional testing has been focused on the UI, the advantages of API testing are becoming well known.
While there are many aspects of API testing, it generally consists of make requests to a single or sometimes multiple API endpoints and validate the response - whether for performance, security, functional correctness, or just a status check. While UI testing may focus on validating the look and feel of a web interface or that a particular payment button works - API testing puts much more emphasis on the testing of business logic, data responses and security, and performance bottlenecks.




Q No-2:- What is API testing and name some types of API testing:

APIs have become the center of software development, connecting and transferring data and logic across disparate systems and applications. Luckily, testing them can greatly improve the efficiency of your testing strategy as a whole, helping you deliver software faster than ever.

APIs, or Application Programming Interfaces, are the connecting tissue between different systems or layers of an application. Applications often have three layers: a data layer, a service (API) layer, and a presentation (UI) layer. The API layer contains the business logic of an application - the rules of how users can interact with services, data, or functions of the app.  Because the API or service layer directly touches both the data layer and the presentation layer, it presents the sweet spot of continuous testing for QA and Development teams. While traditional testing has been focused on the UI, the advantages of API testing are becoming well known.

While there are many aspects of API testing, it generally consists of make requests to a single or sometimes multiple API endpoints and validate the response - whether for performance, security, functional correctness, or just a status check. While UI testing may focus on validating the look and feel of a web interface or that a particular payment button works - API testing puts much more emphasis on the testing of business logic, data responses and security, and performance bottlenecks.
name some types of API testing:
9 Types of Tests For Holistic API Testing
With all of this being said, what specific types of tests can an API provider expect to run on their codebase? While there are certainly specialty tests, and no list can be asked to be comprehensive in this realm, most tests fit broadly into one of nine categories.

1. Validation Testing
Validation testing is one of the last steps in the development process, but it is one of the more important tests that can be run. Validation testing is typically done at the very end of the basic development process, specifically after verification of the API’s constituent parts and functions is completed. Whereas many of the tests we’ll discuss throughout this piece deal with specific facets of the codebase or specific functions, validation testing is a much more high-level consideration.

Validation testing is essentially a set of simple questions applied to the entirety of the project. These questions include:

Product: Did we build the correct product? Is the API itself the correct product for the issue that was provided, and did the API experience any significant code bloat or feature creep that took an otherwise lean and focused implementation into an untenable direction?
Behavior: Is the API accessing the correct data in the correctly defined manner? Is the API accessing too much data, is it storing this data correctly given the confidentiality and integrity requirements of the dataset?
Efficiency: Is the API the most accurate, optimized, and efficient method of doing what is required? Can any codebase be removed or altered to remove impairments to the general service?
All of these questions essentially serve to validate the API as a holistic solution, and are performed after the API is developed against an established and agreed upon criteria to ensure correct environment integration, adherence to standards, and deliverance of specific end goals and results. Ultimately, this test can be simply said to be an assurance of correct development against the stated user needs and requirements.

2. Functional Testing
Functional testing is still a very broad methodology of testing, but is less broad than those under Validation testing. Functional testing is simply a test of specific functions within the codebase. These functions in turn represent specific scenarios to ensure that the API functions within expected parameters, and that errors are handled well when the results are outside of the expected parameters.

Functional testing is much easier to explain with a scenario. Let’s assume our API processes music for ordering via an online portal. When a user searches for a song, they search by Track Name and Artist Name. Functional testing in this case takes a layered approach, and handles a few specific scenarios.

First, the function of the API is tested with proper inputs – for example, Song 2 by Blur. The API validates the request and serves the expected results. Additional testing is needed, however – our testing thus also includes errata, searching Song2, song2, or song lyrics.

Due to the nature of the test, we should expect a few stated responses. We should expect either an error (and thus, the appropriate error codes and handling instructions) or a corrected response that bears the material we’ve requested.

Functional testing should deliver on all of these points – not only should the regular test case be included, but scenarios of both errata and edge cases should be implemented in the testing regimen.

More on API Testing: 9 Most Common API Errors That Aren’t Caught
3. UI Testing
While both validation and functional testing are somewhat generalized in their approaches, UI testing is more specific. UI testing is exactly what it says on the tin – a test of the user interface for your API and its constituent parts. This test is specifically concerned with the function of the UI, whether that interface is graphical in nature or depends upon command-line endpoint calls.

This is in many ways less of a test of the API itself, and more a test of the interface that ties into the API and the developer experience of using that interface. Though not a direct test of the API in terms of codebase, this gives a very generalized view of the health, usability, and efficiency of both the front-end and the back-end.

In fact, this is why UI testing is often used as a substitute for functional testing – in many ways, this test serves the same function, albeit in a less complete and more general sense. That being said, this is a poor approach in modern testing, and UI testing should be strictly limited to ensuring that the UI itself functions as intended.

It should be mentioned that web UI testing is a subset of this type of test, and is concerned more with the end-to-end integrations between web instances the the APIs they represent. Though web UI testing is indeed a subset that is distinct from other UI testing, it bears mentioning and inclusion in this category.

Read more: Automatic Testing For API Documentation
4. Load Testing
Load testing is a test obsessed with reality – it purposely eschews the theoretical (does this code work in theory?) and errs on the practical (will this code work with 1k requests 10k requests, and 100k requests?). Load testing is thus typically done after the completion of a specific unit or the codebase as a whole, testing whether the theoretical solution works as a practical solution under a given load.

Load testing takes on a few different scenarios in order to ensure peak performance. The first of these scenarios is called the “baseline“, and tests the API against the theoretical regular traffic the API expects in normal, day-to-day usage. This includes regular sized tests peppered with some extremely large requests in an effort to measure any impact between the two request types in practice.

A second load test is typically done with the theoretical maximum traffic. This is done to ensure that, even during times of full load, methods are in place to safely throttle requests. While the API may never actually reach this theoretical maximum, it is at least good to ensure it can be safely reached with the API reacting in an adequate fashion.

Finally, an overload test is typically done, testing to the theoretical maximum and adding 10–20% additional traffic on the top. While this type of testing all but anticipates some sort of failure, it is as much a test of the API function as it is a test of the error code generation and handling built into the API, and as such, almost becomes a hybrid test, concerned with what occurs during high load operation and how any failures are handled during said high load operation.

Related: How To Handle High Traffic APIs
5. Runtime/Error Detection
This type of test is entirely concerned with the actual running of the API. Whereas most of our other tests are chiefly concerned with the result of implementing the API in an environment or scenario, this test is chiefly concerned with the universal results of utilizing the API codebase. These types of tests generally follow one of a few focuses:

Monitoring: The runtime of the compiled code is tested for various implementation errors, handler failures, and other intrinsic issues with the implementation to ensure there is no insecurity in the codebase through malfunction.
Execution Errors: The code should respond to valid requests in a predictable, known way, and should fail invalid requests just the same; predictably, and with a known pattern.
Resource Leaks: Invalid requests, purposefully overflowing commands, and other “illegal but common” types of requests are submitted to the API to test for memory, resource, data, or operational leaks and insecurities.
Error Detection: The code is put through known failure scenarios to ensure that errors are properly detected, handled, and routed.
Note that many of these could arguably be considered part of previous categories; this is because runtime/error detection is a near final review of the known errors and issues generated by previous tests, and is designed to holistically ensure resolutions have been applied successfully.

Related: 6 Techniques For 99.999% Uptime
6. Security Testing
Security testing, penetration testing, and fuzz testing are often launched as three separate components of a greater security auditing process, and for this reason, they’ll be discussed jointly. These types of tests are designed to ensure that the implementation of the API is secure from external threats.

Security testing, as previously mentioned, encompasses penetration and fuzz testing, but entails additional steps, including validation of encryption methodologies and validating the design of the access control solution for the API. This includes user rights management and validating authorization checks for resource access.

7. Penetration Testing
Penetration testing takes this a step further, and is generally the second step in the greater auditing process. In this type of test, the API is attacked by someone who has limited working knowledge of the API itself in order to assess the threat vector from an outside perspective. These attacks can be limited to certain functions, resources, or processes, or can target the entirety of the API and its constituent parts.

8. Fuzz Testing
Finally, fuzz testing is typically a later step in the overall security audit, and is certainly less refined than Penetrating testing or the previous tests mentioned. In Fuzz testing, massive amounts of purely random data, sometimes referred to as “noise” or “fuzz,” is forcibly input into the system in order to attempt a forced crash, overflow, or other negative behavior. This is done to test the API at its absolute limits, and serves somewhat as a “worst case scenario.”

9. Interoperability and WS Compliance Testing
While this is not necessarily a common series of tests, nor is it one that RESTful API providers will likely come up against, it’s something that should be discussed given the still wide use of SOAP in the enterprise environment. Interoperability and WS Compliance Testing is a type of testing that really only applies to SOAP APIs, and specifically checks for two general fields of function.

First, Interoperability between SOAP APIs is checked by ensuring conformance to the Web Services Interoperability profiles. By conforming to these guidelines and utilizing these tests, interoperability between SOAP APIs can be confirmed and supported. This also has the added benefit of assuring that your APIs are compatible with some relatively large members of the consortium that stated these standards, including IBM, Microsoft, BEA Systems, Oracle, Intel, and more.

Secondly, WS-* compliance is tested to ensure standards such as WS-Addressing, WS-Discovery, WS-Federation, WS-Policy, WS-Security, and WS-Trust are properly implemented and utilized. This is a general step in assuring that your specific SOAP implementation matches the current industry standards, and is secure in its operations.t


Q No-3:-What is the difference between REST and SOAP APIs? 
As we know that each machine understand and deals in its different language or input so web-services are something which are required for inter communication between machines and to exchange data between them. In order to implement some set of restrictions over their communication some set of rules and regulations are defined which are known as web-services which basically defines the format and type of data that need to be exchanged and specifically a contract which both machines should be aware of before taking part in communication.

This communication system can be categorized into two types, namely Simple Object Access Protocol or SOAP, and Representational State Transfer or REST.

Following are the important differences between REST API and SOAP API.

<img width="478" alt="image" src="https://user-images.githubusercontent.com/102998720/164865853-a6a44594-cde5-4751-99cf-2f78f9318d65.png">

Q No-4:- What are common HTTP methods? Explain with examples:

The set of common methods for HTTP/1.1 is defined below. Although this set can be expanded, additional methods cannot be assumed to share the same semantics for separately extended clients and servers.

The Host request-header field (section 14.23) MUST accompany all HTTP/1.1 requests.

9.1 Safe and Idempotent Methods
9.1.1 Safe Methods
Implementors should be aware that the software represents the user in their interactions over the Internet, and should be careful to allow the user to be aware of any actions they might take which may have an unexpected significance to themselves or others.

In particular, the convention has been established that the GET and HEAD methods SHOULD NOT have the significance of taking an action other than retrieval. These methods ought to be considered "safe". This allows user agents to represent other methods, such as POST, PUT and DELETE, in a special way, so that the user is made aware of the fact that a possibly unsafe action is being requested.

Naturally, it is not possible to ensure that the server does not generate side-effects as a result of performing a GET request; in fact, some dynamic resources consider that a feature. The important distinction here is that the user did not request the side-effects, so therefore cannot be held accountable for them.

9.1.2 Idempotent Methods
Methods can also have the property of "idempotence" in that (aside from error or expiration issues) the side-effects of N > 0 identical requests is the same as for a single request. The methods GET, HEAD, PUT and DELETE share this property. Also, the methods OPTIONS and TRACE SHOULD NOT have side effects, and so are inherently idempotent.

However, it is possible that a sequence of several requests is non- idempotent, even if all of the methods executed in that sequence are idempotent. (A sequence is idempotent if a single execution of the entire sequence always yields a result that is not changed by a reexecution of all, or part, of that sequence.) For example, a sequence is non-idempotent if its result depends on a value that is later modified in the same sequence.

A sequence that never has side effects is idempotent, by definition (provided that no concurrent operations are being executed on the same set of resources).

9.2 OPTIONS
The OPTIONS method represents a request for information about the communication options available on the request/response chain identified by the Request-URI. This method allows the client to determine the options and/or requirements associated with a resource, or the capabilities of a server, without implying a resource action or initiating a resource retrieval.

Responses to this method are not cacheable.

If the OPTIONS request includes an entity-body (as indicated by the presence of Content-Length or Transfer-Encoding), then the media type MUST be indicated by a Content-Type field. Although this specification does not define any use for such a body, future extensions to HTTP might use the OPTIONS body to make more detailed queries on the server. A server that does not support such an extension MAY discard the request body.

If the Request-URI is an asterisk ("*"), the OPTIONS request is intended to apply to the server in general rather than to a specific resource. Since a server's communication options typically depend on the resource, the "*" request is only useful as a "ping" or "no-op" type of method; it does nothing beyond allowing the client to test the capabilities of the server. For example, this can be used to test a proxy for HTTP/1.1 compliance (or lack thereof).

If the Request-URI is not an asterisk, the OPTIONS request applies only to the options that are available when communicating with that resource.

A 200 response SHOULD include any header fields that indicate optional features implemented by the server and applicable to that resource (e.g., Allow), possibly including extensions not defined by this specification. The response body, if any, SHOULD also include information about the communication options. The format for such a

body is not defined by this specification, but might be defined by future extensions to HTTP. Content negotiation MAY be used to select the appropriate response format. If no response body is included, the response MUST include a Content-Length field with a field-value of "0".

The Max-Forwards request-header field MAY be used to target a specific proxy in the request chain. When a proxy receives an OPTIONS request on an absoluteURI for which request forwarding is permitted, the proxy MUST check for a Max-Forwards field. If the Max-Forwards field-value is zero ("0"), the proxy MUST NOT forward the message; instead, the proxy SHOULD respond with its own communication options. If the Max-Forwards field-value is an integer greater than zero, the proxy MUST decrement the field-value when it forwards the request. If no Max-Forwards field is present in the request, then the forwarded request MUST NOT include a Max-Forwards field.

9.3 GET
The GET method means retrieve whatever information (in the form of an entity) is identified by the Request-URI. If the Request-URI refers to a data-producing process, it is the produced data which shall be returned as the entity in the response and not the source text of the process, unless that text happens to be the output of the process.

The semantics of the GET method change to a "conditional GET" if the request message includes an If-Modified-Since, If-Unmodified-Since, If-Match, If-None-Match, or If-Range header field. A conditional GET method requests that the entity be transferred only under the circumstances described by the conditional header field(s). The conditional GET method is intended to reduce unnecessary network usage by allowing cached entities to be refreshed without requiring multiple requests or transferring data already held by the client.

The semantics of the GET method change to a "partial GET" if the request message includes a Range header field. A partial GET requests that only part of the entity be transferred, as described in section 14.35. The partial GET method is intended to reduce unnecessary network usage by allowing partially-retrieved entities to be completed without transferring data already held by the client.

The response to a GET request is cacheable if and only if it meets the requirements for HTTP caching described in section 13.

See section 15.1.3 for security considerations when used for forms.

9.4 HEAD
The HEAD method is identical to GET except that the server MUST NOT return a message-body in the response. The metainformation contained in the HTTP headers in response to a HEAD request SHOULD be identical to the information sent in response to a GET request. This method can be used for obtaining metainformation about the entity implied by the request without transferring the entity-body itself. This method is often used for testing hypertext links for validity, accessibility, and recent modification.

The response to a HEAD request MAY be cacheable in the sense that the information contained in the response MAY be used to update a previously cached entity from that resource. If the new field values indicate that the cached entity differs from the current entity (as would be indicated by a change in Content-Length, Content-MD5, ETag or Last-Modified), then the cache MUST treat the cache entry as stale.

9.5 POST
The POST method is used to request that the origin server accept the entity enclosed in the request as a new subordinate of the resource identified by the Request-URI in the Request-Line. POST is designed to allow a uniform method to cover the following functions:

      - Annotation of existing resources;
      - Posting a message to a bulletin board, newsgroup, mailing list,
        or similar group of articles;
      - Providing a block of data, such as the result of submitting a
        form, to a data-handling process;
      - Extending a database through an append operation.
The actual function performed by the POST method is determined by the server and is usually dependent on the Request-URI. The posted entity is subordinate to that URI in the same way that a file is subordinate to a directory containing it, a news article is subordinate to a newsgroup to which it is posted, or a record is subordinate to a database.

The action performed by the POST method might not result in a resource that can be identified by a URI. In this case, either 200 (OK) or 204 (No Content) is the appropriate response status, depending on whether or not the response includes an entity that describes the result.

If a resource has been created on the origin server, the response SHOULD be 201 (Created) and contain an entity which describes the status of the request and refers to the new resource, and a Location header (see section 14.30).

Responses to this method are not cacheable, unless the response includes appropriate Cache-Control or Expires header fields. However, the 303 (See Other) response can be used to direct the user agent to retrieve a cacheable resource.

POST requests MUST obey the message transmission requirements set out in section 8.2.

See section 15.1.3 for security considerations.

9.6 PUT
The PUT method requests that the enclosed entity be stored under the supplied Request-URI. If the Request-URI refers to an already existing resource, the enclosed entity SHOULD be considered as a modified version of the one residing on the origin server. If the Request-URI does not point to an existing resource, and that URI is capable of being defined as a new resource by the requesting user agent, the origin server can create the resource with that URI. If a new resource is created, the origin server MUST inform the user agent via the 201 (Created) response. If an existing resource is modified, either the 200 (OK) or 204 (No Content) response codes SHOULD be sent to indicate successful completion of the request. If the resource could not be created or modified with the Request-URI, an appropriate error response SHOULD be given that reflects the nature of the problem. The recipient of the entity MUST NOT ignore any Content-* (e.g. Content-Range) headers that it does not understand or implement and MUST return a 501 (Not Implemented) response in such cases.

If the request passes through a cache and the Request-URI identifies one or more currently cached entities, those entries SHOULD be treated as stale. Responses to this method are not cacheable.

The fundamental difference between the POST and PUT requests is reflected in the different meaning of the Request-URI. The URI in a POST request identifies the resource that will handle the enclosed entity. That resource might be a data-accepting process, a gateway to some other protocol, or a separate entity that accepts annotations. In contrast, the URI in a PUT request identifies the entity enclosed with the request -- the user agent knows what URI is intended and the server MUST NOT attempt to apply the request to some other resource. If the server desires that the request be applied to a different URI,

it MUST send a 301 (Moved Permanently) response; the user agent MAY then make its own decision regarding whether or not to redirect the request.

A single resource MAY be identified by many different URIs. For example, an article might have a URI for identifying "the current version" which is separate from the URI identifying each particular version. In this case, a PUT request on a general URI might result in several other URIs being defined by the origin server.

HTTP/1.1 does not define how a PUT method affects the state of an origin server.

PUT requests MUST obey the message transmission requirements set out in section 8.2.

Unless otherwise specified for a particular entity-header, the entity-headers in the PUT request SHOULD be applied to the resource created or modified by the PUT.

9.7 DELETE
The DELETE method requests that the origin server delete the resource identified by the Request-URI. This method MAY be overridden by human intervention (or other means) on the origin server. The client cannot be guaranteed that the operation has been carried out, even if the status code returned from the origin server indicates that the action has been completed successfully. However, the server SHOULD NOT indicate success unless, at the time the response is given, it intends to delete the resource or move it to an inaccessible location.

A successful response SHOULD be 200 (OK) if the response includes an entity describing the status, 202 (Accepted) if the action has not yet been enacted, or 204 (No Content) if the action has been enacted but the response does not include an entity.

If the request passes through a cache and the Request-URI identifies one or more currently cached entities, those entries SHOULD be treated as stale. Responses to this method are not cacheable.

9.8 TRACE
The TRACE method is used to invoke a remote, application-layer loop- back of the request message. The final recipient of the request SHOULD reflect the message received back to the client as the entity-body of a 200 (OK) response. The final recipient is either the

origin server or the first proxy or gateway to receive a Max-Forwards value of zero (0) in the request (see section 14.31). A TRACE request MUST NOT include an entity.

TRACE allows the client to see what is being received at the other end of the request chain and use that data for testing or diagnostic information. The value of the Via header field (section 14.45) is of particular interest, since it acts as a trace of the request chain. Use of the Max-Forwards header field allows the client to limit the length of the request chain, which is useful for testing a chain of proxies forwarding messages in an infinite loop.

If the request is valid, the response SHOULD contain the entire request message in the entity-body, with a Content-Type of "message/http". Responses to this method MUST NOT be cached.

9.9 CONNECT
This specification reserves the method name CONNECT for use with a proxy that can dynamically switch to being a tunnel (e.g. SSL tunneling [44]).

Q No-5:- What is the difference between POST AND put? Explain with an example.

What is PUT?
PUT method is used to update resource available on the server. Typically, it replaces whatever exists at the target URL with something else. You can use it to make a new resource or overwrite an existing one. PUT requests that the enclosed entity must be stored under the supplied requested URI (Uniform Resource Identifier).

What is POST?
POST is a method that is supported by HTTP and

depicts that a web server accepts the data included in the body of the message, which is requested. POST is often used by World Wide Web to send user generated data to the web server or when you upload file.,

KEY DIFFERENCES:
a)PUT method is called when you have to modify a single resource while POST method is called when you have to add a child resource.
b)PUT method response can be cached but you cannot cache POST method responses.
c)You can use UPDATE query in PUT whereas you can use create query in POST.
d)In PUT method, the client decides which URI resource should have, and in POST method, the server decides which URI resource should have.
e)PUT works as specific while POST work as abstract.
f)If you send the same PUT request multiple times, the result will remain the same but if you send the same POST request multiple times, you will receive different results.
g)PUT method is idempotent whereas POST method is not idempotent.

Example of PUT
Here is the webserver example of a PUT method:

HTTP PUT http://www.google.com/users/234

HTTP PUT http://www.google.com/users/234/accounts/567

Request

PUT /new.html HTTP/1.1
Host: example.com
Content-type: text/html
Content-length: 20

<p>New File</p>
Responses

If the target resource having current representation and is modified with the state of the enclosed representation, then the server should send two responses. The first response code is 200 (OK), and the second response code is 204 (No Content).

If the target resource does not have any representation, then the server should inform the user by sending a 201 code (Created) response.

 HTTP/1.1 201 Created
Content-Location: /new.html
Example of POST
Here is an example of POST method:

HTTP POST http://www.google.com/users

HTTP POST http://www.google.com/users/234/accounts

A form using the default application/x-www-form-urlencoded content type:

POST /test HTTP/1.1
Host: abc.example
Content-Type: application/x-www-form-urlencoded
Content-Length: 40

field1=value1&field2=value2

Q No-6:- Name 5 main categories of HTTP status codes? Explain 5 status codes from each category(You have to tell the status code and description of each status code with an example).

What are HTTP status codes?
HTTP status codes are three-digit responses from the server to the browser-side request. Everyone has probably gotten the classic 404 page-not-found error. That is an HTTP client error status code and there are a lot more of them.

These status codes (also called response status codes) serve as a means of communication between the server and the internet browser and there are multiple code classes based on the type of information they are communicating. The differences in classes are indicated through the first digit of the error code, for example: just like a 404, any other 4xx will mean that in some way the page or website could not be reached, while a 2xx means that your request was successfully completed.

How are HTTP status codes categorized?
HTTP status codes are split into 5 different categories. Each category will give you hints as to what the response was, even if you don't know the specific response code.

For an explanation of each category - and each individual status code - click on the corresponding link below or go to our complete list of HTTP status codes.

1xx - Informational: The server has received the request and is continuing the process 
2xx - Successful: The request was successful and the browser has received the expected information 
3xx (Redirection): You have been redirected and the completion of the request requires further action
4xx (Client Error): The website or the page could not be reached, either the page is unavailable or the request contains bad syntax 
5xx (Server Error): While the request appears to be valid, the server could not complete the request

Complete list of HTTP Status Codes:

Status code	Meaning
1xx Informational	 
100	Continue
101	Switching protocols
102	Processing
103	Early Hints
 	 
2xx Succesful	 
200	OK
201	Created
202	Accepted
203 	Non-Authoritative Information
204	No Content
205	Reset Content
206	Partial Content
207	Multi-Status
208	Already Reported
226	IM Used
 	 
3xx Redirection	 
300	Multiple Choices
301	Moved Permanently
302	Found (Previously "Moved Temporarily")
303	See Other
304	Not Modified
305	Use Proxy
306	Switch Proxy
307	Temporary Redirect
308	Permanent Redirect
 	 
4xx Client Error	 
400	Bad Request
401	Unauthorized
402	Payment Required
403	Forbidden
404	Not Found
405	Method Not Allowed
406	Not Acceptable
407	Proxy Authentication Required
408	Request Timeout
409	Conflict
410	Gone
411	Length Required
412	Precondition Failed
413	Payload Too Large
414	URI Too Long
415	Unsupported Media Type
416	Range Not Satisfiable
417	Expectation Failed
418	I'm a Teapot
421	Misdirected Request
422	Unprocessable Entity
423	Locked
424	Failed Dependency
425	Too Early
426	Upgrade Required
428	Precondition Required
429	Too Many Requests
431	Request Header Fields Too Large
451	Unavailable For Legal Reasons
 	 
5xx Server Error	 
500	Internal Server Error
501	Not Implemented
502	Bad Gateway
503	Service Unavailable
504	Gateway Timeout
505	HTTP Version Not Supported
506	Variant Also Negotiates
507	Insufficient Storage
508	Loop Detected
510	Not Extended
511	Network Authentication Required

HTTP Status Codes explained individually
In some cases a HTTP response code might be descriptive enough to understand its meaning. 200 OK probably means that everything went okay. But what about a 103 Early Hints, 205 Reset Content and 305 Use Proxy?

Below is an explanation for all 63 status codes, sorted in the 5 overall categories.

 

What does a 1xx Informational status code mean?
A 1xx Informational status code means that the server has received the request and is continuing the process. A 1xx status code is purely temporary and is given while the request processing continues. For most tasks you won't encounter these much, as it's not the final response to the request.

100 Continue
101 Switching protocols
102 Processing
103 Early Hints
 

What does 100 Continue mean?
The 100 Continue status code means that the initial part of the request has been received by the server and that the client should proceed with the request or ignore the response if the request has already finished.

 

What does 101 Switching protocols mean?
The 101 Switching protocols status code means that the server understands the Upgrade header field request and indicates which protocol it is switching to.

 

What does 102 Processing mean?
The 102 Processing status code means that the server has accepted the full request but has not yet completed it and no response is available as of yet.

 

What does 103 Early Hints mean?
The 103 Early hints status code is intended to be used to allow the user agent to preload resources, while the server prepares a response. It is intended to be primarily used with the Link Header.

What does a 2xx Succesful status code mean?
A 2xx Succesful status code means that the request was successful and the browser has received the expected information. This is generally the one you want to see, as it means that the request was a success and has been received, understood and accepted it. As a website owner you should make sure that all pages and resources (images, videos, etc.) all return a 2xx status code. This means that browsers can reach it successfully and that your website visitors can see and use your website.

200 OK
201 Created
202 Accepted
203 Non-Authoritative Information
204 No Content
205 Reset Content
206 Partial Content
207 Multi-Status
208 Already Reported
226 IM Used
 

What does 200 OK mean?
The 200 OK status code means that the request was successful, but the meaning of success depends on the request method used:

GET: The requested resource has been fetched and transmitted to the message body.
HEAD: The header fields from the requested resource are sent in without the message body. 
POST or PUT: A description of the result of the action is transmitted to the message body.
TRACE: The request messages, as received by the server, will be included in the message body
When looking at things SEO-wise the 200 OK response code is the perfect status code for a functioning page, all the linked pages are working as they should. A 200 will mean that search engine crawlers can successfully crawl the page and it will be put into their search index.

 

What does 201 Created mean?
The 201 Created status code means that the request was successfully fulfilled and resulted in one or possibly multiple new resources being created.

 

What does 202 Accepted mean?
The 202 Accepted status code means that the request has been accepted for processing, but the processing has not been finished yet. The request may or may not be completed when the processing eventually takes place.

 

What does 203 Non-Authoritative Information mean?
The 203 Non-Authoritative Information status code means that the request was successful. However, the meta-information that has been received is different from the one on the origin server and has instead been collected from a 3rd party or local copy. When not used for backups or mirrors of another resource a 200 OK response is preferable.

 

What does 204 No Content mean?
The 204 No Content status code means that while the server has successfully fulfilled the request, there is no available content for this request. But the user agent might want to update its currently cached headers for this resource, for the new one. 

 

What does 205 Reset Content mean?
The 205 Reset Content status code means that the user should reset the document that sent this request.

 

What does 206 Partial Content mean?
The 206 Partial Content response code is a response to a Range header sent from the client when requesting only a part of the resource.

 

What does 207 Multi-Status mean?
The 207 Multi-Status status code conveys information about multiple resources, in situation when multiple status codes are appropriate.

 

What does 208 Already Reported mean?
The 208 Already Reported status code is used inside the response element DAV: propstat, in order to avoid enumerating the internal members of multiple bindings to the same collection repeatedly.

 

What does 226 IM Used mean?
The 226 IM response code means that the server has successfully fulfilled a GET request for the resource, and the response is a representation of the result of one or multiple instance-manipulations applied to the current instance.

What does a 3xx Redirection code mean?
A 3xx Redirection status code means that you have been redirected and the completion of the request requires further action. Redirects are a natural part of the internet and you shouldn't be scared to have 3xx redirect status codes on your website. A redirect means that the request was received successfully, but that the resource was found elsewhere. If a webpage has changed path and you try to access it through the old path, your CMS will often redirect the user to the new path. Ultimately the request will end in a 2xx success, but first it must go through the 3xx redirection.

300 Multiple Choices
301 Moved Permanently
302 Found (Previously "Moved temporarily")
303 See Other
304 Not Modified
305 Use Proxy
306 Switch Proxy
307 Temporary Redirect
308 Permanent Redirect
 

What does 300 Multiple Choices mean?
The 300 Multiple Choices status code means that the request has multiple possible responses and the user/user agent should choose one.

 

What does 301 Moved Permanently mean?
The 301 Moved Permanently response code means that the target resource has been assigned a new permanent URL and any references to this resources in the future should use one of the URLs included in the response.

When looking at things SEO-wise the 301 Permanent Redirect should be used every time a URL is moved permanently. This redirect passes your current link equity from your content to the new URL. Links that result in a status code 301 does give slightly less link equity than 200. So if you have a lot of links going through a 301 Permanent Redirect it is advised to fix these, if possible.

 

What does 302 Found (Previously “Moved temporarily”) mean?
The 302 Found status code, previously known as “Moved temporarily”, means that the URI of the request has been changed temporarily, and since changes can be made to the URI in the future, the effective request URI should be used for future requests.

When looking at things SEO-wise the 302 Found should only be used when making temporary changes as it does not pass the link equity the same way as a 301. If the page is not going to come back you should always use 301.

 

What does 303 See Other mean?
The 303 See Other response code is sent by the server in order to direct the client to get the requested resource at another URI with a GET request.

 

What does 304 Not Modified mean?
The 304 Not Modified response code informs the client that the response has not been modified. This means that the client can continue to use the already present, cached version of the response.

 

What does 305 Use Proxy mean?
The 305 Use Proxy status code instructs a client that it should connect to a proxy and then repeat the same request there. This response code is deprecated due to security concerns.

 

What does 306 Switch Proxy mean?
The 306 Switch proxy status code is no longer in use. It was used to inform the client that the subsequent requests should use the specified proxy.

 

What does 307 Temporary Redirect mean?
The 307 Temporary Redirect status code gets sent by the server in order to direct the client to the requested resource at another URI. The request method, however, must not be changed.

 

What does 308 Permanent Redirect mean?
The 308 Permanent Redirect status code means that the requested resource has been permanently assigned a new URI and future references to the resource should be made by using one of the enclosed URIs.

What does a 4xx Client Error mean?
A 4xx Client Error status code means that the website or the page could not be reached and either the page is unavailable or the request contains bad syntax. As a website owner you should do your best to avoid these, as it means your users will not find what they're looking for. This can be either pages that are no longer found and are either temporarily or permanently gone. Besides giving a bad user experience, it can also hurt your SEO efforts.

400 Bad Request
401 Unauthorized
402 Payment Required
403 Forbidden
404 Not Found
405 Method Not Allowed
406 Not Acceptable
407 Proxy Authentication Required
408 Request Timeout
409 Conflict
410 Gone
411 Length Required
412 Precondition Failed
413 Payload Too Large
414 URI Too Long
415 Unsupported Media Type
416 Range Not Satisfiable
417 Expectation Failed
418 I'm a Teapot
421 Misdirected Request
422 Unprocessable Entity
423 Locked
424 Failed Dependency
425 Too Early
426 Upgrade Required
428 Precondition Required
429 Too Many Requests
431 Request Header Fields Too Large
451 Unavailable For Legal Reasons
 

What does 400 Bad Request mean?
The 400 Bad Request status code means that the server could not understand the request because of invalid syntax.

 

What does 401 Unauthorized mean?
The 401 Unauthorized status code means that the request has not been applied because the server requires user authentication.

 

What does 402 Payment Required mean?
The 402 Payment Required status code is a response reserved for future use. It was originally created to be implemented in digital payment systems, however, it is rarely used and a standard convention of using it does not exist.

 

What does 403 Forbidden mean?
The 403 Forbidden status code means that the client request has been rejected because the client does not have rights to access the content. Unlike a 401 error, the client's identity is known to the server, but since they are not authorized to view the content, giving the proper response is rejected by the server.

 

What does error 404 mean?
The 404 Not Found status code means that the server either did not find a current representation for the requested resource or is trying to hide its existence from an unauthorized client.

When looking at things SEO-wise the 404 Not Found status code pages with a high volume of traffic should be redirected using a 301 to the most relevant page possible. For some pages, however, a 404 might be necessary, for example, if the product is out of stock for an extended period of time. If you have external links pointing to a page that returns 404, you will lose the link equity those links would otherwise give.

If you need to fix 404 errors, jump to this section.

 

What does 405 Method Not Allowed mean?
The 405 Method Not Allowed status code means that while the server knows the request method, the method has been disabled and can not be used.

 

What does 406 Not Acceptable mean?
The 406 Not Acceptable status code is sent by the server when it does not find any content following the criteria given by the user agent.

 

What does 407 Proxy Authentication Required mean?
The 407 Proxy Authentication Required status code means that the client must first be authenticated by a proxy (similar to a 401).

 

What does 408 Request Timeout mean?
The 408 Request Timeout status code means that the server did not receive a complete request in the time that it prepared to wait.

 

What does 409 Conflict mean?
The 409 Conflict status code means that the request could not be fulfilled due to a conflict with the current state of the target resource and is used in situations where the user might be able to resubmit the request after resolving the conflict.

 

What does 410 Gone mean?
The 410 Gone status code means that the target resource has been deleted and the condition seems to be permanent. 

When looking at things SEO-wise the 410 Gone status code is a more permanent version a 404. The page will no longer be available from the server and has no forwarding address available. If you want to completely remove a page from Googles search index, then using 410 on a page is the proper way of doing it (instead of simply 404). 

 

What does 411 Length Required mean?
The 411 Length Required status code means that the server has rejected the request because it requires the Content-Length header field to be defined.

 

What does 412 Precondition Failed mean?
The 412 Precondition Failed status code means the server does not meet one or multiple preconditions that were indicated in the request header fields.

 

What does 413 Payload Too Large mean?
The 413 Payload Too Large status code means the server refuses to process the request because the request payload is larger than the server is able or willing to process. While the server may close the connection to prevent the client from continuing the request, it should generate a Retry-After header field and after how long can the client retry.

 

What does 414 URI Too Long mean?
The 414 URI Too Long status code means that the server is refusing to service the request because the request-target was longer than the server was willing to interpret.

 

What does 415 Unsupported Media Type mean?
The 415 Unsupported Media Type status code means that the server is rejecting the request because it does not support the media format of the requested data.

 

What does 416 Range Not Satisfiable mean?
The 416 Range Not Satisfiable status code means that the range specified in the Range header field of the request can't be fulfilled. The reason might be that the given range is outside the size of the target URI's data.

 

What does 417 Expectation Failed mean?
The 417 Expectation Failed status code means that the Expectation indicated by the Expect request-header field could not be met by the server.

 

What does 418 I’m a Teapot mean?
The 418 I'm a Teapot status code means that the server refuses to brew coffee because it is, in fact, a teapot. (It is a reference to a 1998 April Fools' joke called ''Hyper Text Coffee Pot Control Protocol'').

 

What does 421 Misdirected Request mean?
The 421 Misdirected Request status code means that the client request was directed at a server that is not configured to produce a response.

 

What does 422 Unprocessable Entity mean?
The 422 Unprocessable Entity status code means that while the request was well-formed, the server was unable to follow it, due to semantic errors.

 

What does 423 Locked mean?
The 423 Locked status code means that the resource that is being accessed is locked.

 

What does 424 Failed Dependency mean?
The 424 Failed Dependency status code means that the request failed due to the failure of a previous request.

 

What does 425 Too Early mean?
The 425 Too Early status code means that the server is not willing to risk processing a request that might be replayed.

 

What does 426 Upgrade Required mean?
The 426 Upgrade Required status code means that while the server refuses to perform the given request using the current protocol, it might be willing to do so after the client has been upgraded to a different protocol.

 

What does 428 Precondition Required mean?
The 428 Precondition Required status code means that the origin server requires the request to be conditional.

 

What does 429 Too Many Requests mean?
The 429 Too Many Requests response code means that in the given time, the user has sent too many requests.

 

What does 431 Request Header Fields Too Large mean?
The 431 Request Header Fields Too Large means that the server is not willing to process the request because its header fields are indeed too large, however, the request may be submitted again once the size of the request header fields is reduced.

 

What does 451 Unavailable For Legal Reasons mean?
The 451 Unavailable For Legal Reasons response code means that the user has requested an illegal resource (such as pages and sites blocked by the government).

What does a 5xx Server error mean?
A 5xx Server error status code means that while the request appears to be valid, the server could not complete the request. If you're experiencing 5xx server errors for your website, you should immediately look at your server. If you're hosting your own server you'll need to start debugging to figure out why it is not responding properly. If you're using an external hosting provider you'll need to reach out to them, so they can look at it.

500 Internal Server Error
501 Not Implemented
502 Bad Gateway
503 Service Unavailable
504 Gateway Timeout
505 HTTP Version Not Supported
506 Variant Also Negotiates
507 Insufficient Storage
508 Loop Detected
510 Not Extended
511 Network Authentication Required
 

What does 500 Internal Server Error mean?
The 500 Internal Server Error status code means that the server has encountered a situation that it does not know how to handle.

When looking at things SEO-wise the 500 Internal Server Error indicates a problem with the server, not the actual availability of the content. Since bots and users will both be lost, the link equity will go down fast.

 

What does 501 Not Implemented mean?
The 501 Not Implemented response code means that the request can not be handled because it is not supported by the server.

 

What does 502 Bad Gateway mean?
The 502 Bad Gateway response code means that the server received an invalid response while working as a gateway to handle the response.

 

What does 503 Service Unavailable mean?
The 503 Service Unavailable response code means that the server is currently not ready to handle the request. This is a common occurrence when the server is down for maintenance or is overloaded.

When looking at things SEO-wise the 503 Service Unavailable status code means that the server is unavailable and the visitor, bot or human, is asked to return again at a later time. This could be because of either server maintenance or server overload and search engines know to come back and check the availability later.

If you want to fix 503 errors, jump to this section.

 

What does 504 Gateway Timeout mean?
The 504 Gateway Timeout response code means that the server acting as a gateway could not get a response time.

 

What does 505 HTTP Version Not Supported mean?
The 505 HTTP Version Not Supported response code means that the version of HTTP used in the request is not supported by the server.

 

What does 506 Variant Also Negotiates mean?
The 506 Variant Also Negotiates response code means that the server has the following internal configuration error: The chosen variant resource is configured to engage in transparent negotiation itself, therefore it cannot be a proper endpoint in the negotiation process.

 

What does 507 Insufficient Storage mean?
The 507 Insufficient Storage status code means that the method could not be performed on the resource because the server is not able to store the representation that would be needed to complete the request successfully.

 

What does 508 Loop Detected mean?
The 508 Loop Detected response code means that the server has detected an infinite loop while processing the request.

 

What does 510 Not Extended mean?
The 510 Not Extended response code means that further extensions are required for the server to be able to fulfil the request.

 

What does 511 Network Authentication Required mean?
The 511 Network Authentication Required response code indicates that the client needs to authenticate to gain network access. 

Q No-7:-What are the main components of HTTP requests and HTTP responses?
 
 HTTP requests:-

An HTTP request is made by a client, to a named host, which is located on a server. The aim of the request is to access a resource on the server.

To make the request, the client uses components of a URL (Uniform Resource Locator), which includes the information needed to access the resource. The components of a URL explains URLs.

A correctly composed HTTP request contains the following elements:
A request line.
A series of HTTP headers, or header fields.
A message body, if needed.
Each HTTP header is followed by a carriage return line feed (CRLF). After the last of the HTTP headers, an additional CRLF is used (to give an empty line), and then any message body begins.
Request line
The request line is the first line in the request message. It consists of at least three items:
A method. The method is a one-word command that tells the server what it should do with the resource. For example, the server could be asked to send the resource to the client.
The path component of the URL for the request. The path identifies the resource on the server.
The HTTP version number, showing the HTTP specification to which the client has tried to make the message comply.
An example of a request line is:
GET /software/htp/cics/index.html HTTP/1.1

In this example:
the method is GET
the path is /software/htp/cics/index.html
the HTTP version is HTTP/1.1
A request line might contain some additional items:
A query string. This provides a string of information that the resource can use for some purpose. It follows the path, and is preceded by a question mark.
The scheme and host components of the URL, in addition to the path. When the resource location is specified in this way, it is known as the absolute URI form. For HTTP/1.1, this form is used when a request will go through a proxy server. Also for HTTP/1.1, if the host component of the URL is not included in the request line, it must be included in the message in a Host header.
HTTP headers
HTTP headers are written on a message to provide the recipient with information about the message, the sender, and the way in which the sender wants to communicate with the recipient. Each HTTP header is made up of a name and a value. The HTTP protocol specifications define the standard set of HTTP headers, and describe how to use them correctly. HTTP messages can also include extension headers, which are not part of the HTTP/1.1 or HTTP/1.0 specifications.

The HTTP headers for a client's request contain information that a server can use to decide how to respond to the request. For example, the following series of headers can be used to specify that the user only wants to read the requested document in French or German, and that the document should only be sent if it has changed since the date and time when the client last obtained it:
Accept-Language: fr, de
If-Modified-Since: Fri, 10 Dec 2004 11:22:13 GMT

An empty line (that is, a CRLF alone) is placed in the request message after the series of HTTP headers, to divide the headers from the message body.

Message body
The body content of any HTTP message can be referred to as a message body or entity body. Technically, the entity body is the actual content of the message. The message body contains the entity body, which can be in its original state, or can be encoded in some way for transport, such as by being broken into chunks (chunked transfer-coding). The message body of a request may be referred to for convenience as a request body.

Message bodies are appropriate for some request methods and inappropriate for others. For example, a request with the POST method, which sends input data to the server, has a message body containing the data. A request with the GET method, which asks the server to send a resource, does not have a message body.

Parent topic:
The HTTP protocol

HTTP responses:-


An HTTP response is made by a server to a client. The aim of the response is to provide the client with the resource it requested, or inform the client that the action it requested has been carried out; or else to inform the client that an error occurred in processing its request.

An HTTP response contains:
A status line.
A series of HTTP headers, or header fields.
A message body, which is usually needed.
As in a request message, each HTTP header is followed by a carriage return line feed (CRLF). After the last of the HTTP headers, an additional CRLF is used (to give an empty line), and then the message body begins.
Status line
The status line is the first line in the response message. It consists of three items:
The HTTP version number, showing the HTTP specification to which the server has tried to make the message comply.
A status code, which is a three-digit number indicating the result of the request.
A reason phrase, also known as status text, which is human-readable text that summarizes the meaning of the status code.
An example of a response line is:
HTTP/1.1 200 OK

In this example:
the HTTP version is HTTP/1.1
the status code is 200
the reason phrase is OK
Status codes and reason phrases explains more about these elements of the status line.

HTTP headers
The HTTP headers for a server's response contain information that a client can use to find out more about the response, and about the server that sent it. This information can assist the client with displaying the response to a user, with storing (or caching) the response for future use, and with making further requests to the server now or in the future. For example, the following series of headers tell the client when the response was sent, that it was sent by CICS®, and that it is a JPEG image:
Date: Thu, 09 Dec 2004 12:07:48 GMT
Server: IBM_CICS_Transaction_Server/3.1.0(zOS)
Content-type: image/jpg

In the case of an unsuccessful request, headers can be used to tell the client what it must do to complete its request successfully.
An empty line (that is, a CRLF alone) is placed in the response message after the series of HTTP headers, to divide the headers from the message body.

Message body
The message body of a response may be referred to for convenience as a response body.

Message bodies are used for most responses. The exceptions are where a server is responding to a client request that used the HEAD method (which asks for the headers but not the body of the response), and where a server is using certain status codes.

For a response to a successful request, the message body contains either the resource requested by the client, or some information about the status of the action requested by the client. For a response to an unsuccessful request, the message body might provide further information about the reasons for the error, or about some action the client needs to take to complete the request successfully.

Parent topic:
The HTTP protocol


Q No-8:- What are the main components of the HTTP request header and response header?

HTTP Request
When we work with Web API’s, the communication between our clients and our API will be done using HTTP requests. An HTTP request is a message that one computer sends to another using the HTTP protocol. The HTTP request is made by the clients of our API to our API. When our API receives this request, it processes it, and then returns a response, called an HTTP response. The clients and our API will communicate using HTTP requests and responses. These messages have a structure, and in this section we will study that structure.

In general, an HTTP request is divided into 3 parts:

A request line
A set of header fields
A body, which is optional
Let’s see these parts.

Request Line
In the request line we place the HTTP method to be used, the URI of the request and the HTTP protocol to be used. That is, they have the following structure:

HTTP-METHOD URI HTTP-PROTOCOL

We will talk about HTTP methods in the next post, but basically HTTP methods indicate what kind of action our client wants to perform, whether he wants to read a resource, or if he wants to send information to the API, etc. The URI refers to the address where the resource is located. And the HTTP protocol refers to which HTTP protocol will be used, this is because there are several versions of the HTTP protocol, at the time of writing this post, the most common protocol is HTTP/1.1, however, there are other more recent revisions , like the HTTP/2.0 revision.

Let’s see an example of a request line:

GET /api/authors HTTP/1.1
We see that the HTTP method is GET, which means that we want to read a resource, which resource? Well the one indicated afterward, in /api/authors. Finally, it is indicated the HTTP protocol to be used. Then, this request line tells our API that a user or client wants to read the resource found in the URI /api /authors.

Let’s see another example:

POST /test.html HTTP/1.1
Here the HTTP Method is POST, which means that the user wants to send us something. That something the user wants to send us will be found in the body of the request, we will see this in a few minutes. We see that the URI is /test.html, and the procolo is HTTP/1.1.

The second part of an HTTP request is the header.

Request Header
The header of the request is where the headers of the request are located. Headers are metadata that are sent in the request to provide information about the request. Each header is specified with a name, then two points, and then followed by the value of that header.

Let’s see an example of a header:

Host: en.wikipedia.org
In this case, the name of the header is Host, and its value is en.wikipedia.org. The Host header indicates the domain of the server.

Another header example could be:

Cache-Control: no-cache
The name of this header is Cache-Control, and its value is no-cache.

There may be multiple headers in the header of the request. Let’s see an example of a petition with its request line and header:

GET /api/autores HTTP/1.1
Host: en.wikipedia.org
Cache-Control: no-cache
Here we see that the first line is the request line, below this is the header of the request, which is composed of several individual headers, host and cache-control in our case.

The Host and Cache-Control headers are standard headers, which already have a well-defined purpose. However, we are free to use our own custom headers. When we need to express our metadata of our request, we can use custom headers. All you need to do is send them in the header of the HTTP request.

Let’s now look at the third and final part of an HTTP request, the body.

Request Body
The Request Body is where we put additional information that we are going to send to the server. In the body of the request we are free to place virtually whatever we want. From the username and password of a person trying to login to our system, to the answers of a complex form of a survey. The body is quite important, because it represents, in many cases, the content per se that one wants to transmit.

We note that GET requests do not use a body, because one does not tend to send many complex data when reading information. In the case of the POST method, we usually use the body of the request to place what we want to send.

Let’s see an example of a request body:

Hello
Here we have a simple “Hello”. The body of the request is to send virtually anything we want, from a simple greeting, to a little more structured information, such as the following:

{
    "Name": "Felipe Gavilán",
    "Age": 999
}
Here we have data in JSON format that represents the body of our request.

Let’s see then an HTTP request with its three parts:

POST /api/authors HTTP/1.1
Host: myWebApi.com
Content-Type: application/json
Cache-Control: no-cache

{
     "Name": "Felipe Gavilán",
     "Age": 999
}
The request we are looking at is a POST towards the resource /api /authors. We have a header composed of 3 headers: Host, Content-Type and Cache-Control. And finally, at the bottom we have the body of the petition. Notice that a blank line is the separation between the HTTP header and the body.

HTTP Response
As we said at the beginning of this entry, when the client sends us an HTTP request, our server must respond with an HTTP response. The HTTP response also has its own structure, which is quite similar to the structure of the request. These parts are:

Status line
Header
Body, optional
The request status is indicated in the status line, that is, if it was successful, if there was an error, or if it is required that we take some type of action. The HTTP status codes is something we will see in a future entry. The header is a set of headers, just like the request header. The server can send us as many headers as it wants. And, finally, the server has the option to send a body with the data that it wants to transmit to us. Although the body is also optional, it is quite fundamental when it comes to using web pages, since it is through the body that we receive the HTML of a web page that we want to have displayed in our web browser.

Example of an HTTP response:

HTTP/1.1 200 OK
Date: Thu, 03 Jan 2019 23:26:07 GMT
Server: gws
Accept-Ranges: bytes
Content-Length: 68894
Content-Type: text/html; charset=UTF-8

<!doctype html><html …
In the first line we have the status line, the answer was a 200 OK. Then we have the headers of the answer. Finally, separated by a blank line from the headers, we have the body of the response, which in this case is an HTML document.

Summary
An HTTP request is divided into three parts: Request line, header and body. An HTTP response is also divided into three parts: Status line, header and body.

HTTP Response
Have you ever thought about how the front-end of an application communicates with the backend to get data or perform certain operations? It is done through API Requests. API stands for Application Programming Interface. The communication between our client and the API is achieved using HTTP Request which is followed by a Response to the client. Both the Requests and Response follows a certain syntax and structure to ease the communication process.

Whenever our client application wants to communicate to the server, it sends out a message to the server using HTTP Protocols, which is also termed as the HTTP Request. Based on that message, the server performs certain operations as demanded by the message and then replies to the client through a message, also knows as HTTP Response.

Below is an image depicting the Request-Response Cycle:


Image of HTTP Request-Response Cycle

Structure of HTTP Response: As discussed above, the HTTP Response has a special structure that is followed so that the client can easily understand it. There exists a Universal Language that everybody follows so that there is no communication gap between people. HTTP Response broadly has 3 main components: 

Status Line
Headers
Body (Optional)
 

An HTTP Response as a whole looks like the below picture:


Anatomy of HTTP Response

Let us go through each of them one by one:

Status Line: An example of a Status-Line is given below:

HTTP/1.1 200 OK
The Status Line contains three important components – HTTP Version, HTTP Response Code, and a Reason-Phrase. 

HTTP Version: The HTTP version number shows the HTTP specification to which the server has tried to make the response message comply. In the above example, 1.1 is the HTTP Version.
HTTP Response Code: It is a 3 digit number that shows the conclusion of the Request. In the above example, the response code 200 denotes that the content requested was OK. A very popular Status Code that we frequently encounter is 404 which represents the requested resource was not found.
Reason-Phrase: Also known as Status Text as it summarizes the Status Code in human-readable form.
Response Header: The Response Header contains the information about the content that is being returned in response together with data about the Server that sent it. This information helps the Client/Browser in deciding in what way the response data would be used. In other words, headers can be said as metadata that is sent together with a response to provide more info about it.

The Server can send as many headers as needed. The headers are sent as a key-value pair separated by a colon ( : ). Although the server can send as many headers as required, the most popular response headers are Content-Length, Content-Type, Date, Server, Set-Cookie, etc.

Date: Thu, 16 Jan 2016 08:16:18 GMT
Server: IBM_CICS_Transaction_Server/3.1.0(zOS)
Content-type: image/jpg
In the above example, the response header shows the date and time when the response was sent, the server that sent the response, and the type of content that was sent, which here is a jpg image file.

Body: In case of a successful response, the body of the Response Message is used to serve the Client/User with the resource asked for in the request. Although the body is optional, it is one of the most fundamental parts of the communication between the Client and Server and is sent most of the time. The body carries the data and can be in one of the many formats such as json, html, image, etc. which is accordingly specified in the headers. 

In case of some errors, the body might provide the reason for the errors or the actions needed to complete the request successfully. Sometimes, it may have a link to guide the user to some other page.

Q No-9:- What is the difference between authentication and authorization?

What Is Authentication?
Authentication is the act of validating that users are whom they claim to be. This is the first step in any security process. 

Complete an authentication process with:

Passwords. Usernames and passwords are the most common authentication factors. If a user enters the correct data, the system assumes the identity is valid and grants access.
One-time pins. Grant access for only one session or transaction.
Authentication apps. Generate security codes via an outside party that grants access.
Biometrics. A user presents a fingerprint or eye scan to gain access to the system. 
In some instances, systems require the successful verification of more than one factor before granting access. This multi-factor authentication (MFA) requirement is often deployed to increase security beyond what passwords alone can provide.

What Is Authorization?
Authorization in system security is the process of giving the user permission to access a specific resource or function. This term is often used interchangeably with access control or client privilege.

Giving someone permission to download a particular file on a server or providing individual users with administrative access to an application are good examples of authorization.

In secure environments, authorization must always follow authentication. Users should first prove that their identities are genuine before an organization’s administrators grant them access to the requested resources.

Authentication vs Authorization

 

Authentication vs. Authorization
Despite the similar-sounding terms, authentication and authorization are separate steps in the login process. Understanding the difference between the two is key to successfully implementing an IAM solution.

Let's use an analogy to outline the differences.

Consider a person walking up to a locked door to provide care to a pet while the family is away on vacation. That person needs:

Authentication, in the form of a key. The lock on the door only grants access to someone with the correct key in much the same way that a system only grants access to users who have the correct credentials.
Authorization, in the form of permissions. Once inside, the person has the authorization to access the kitchen and open the cupboard that holds the pet food. The person may not have permission to go into the bedroom for a quick nap. 
Authentication and authorization work together in this example. A pet sitter has the right to enter the house (authentication), and once there, they have access to certain areas (authorization).

 	
Authentication

Authorization

What does it do?

Verifies credentials 

Grants or denies permissions

How does it work?

Through passwords, biometrics, one-time pins, or apps

Through settings maintained by security teams

Is it visible to the user?

Yes

No

It is changeable by the user?

Partially

No 

How does data move?

Through ID tokens

Through access tokens 

 

Systems implement these concepts in the same way, so it’s crucial that IAM administrators understand how to utilize both:

Authentication. Let every staff member access your workplace systems if they provide the right credentials in response to your chosen authentication requirements.
Authorization. Grant permission to department-specific files, and reserve access to confidential data, such as financial information, as needed. Ensure that employees have access to the files they need to do their jobs. 
Understand the difference between authentication and authorization, and implement IAM solutions that have strong support for both. You will protect your organization against data breaches and enable your workforce to be more productive.

Q No-10:- Briefly explain common API Authentication Methods.

Unless your API is a public feed of read-only data, you likely need authentication. There are many options you could choose, which may vary depending on your use case. However, it’s unlikely you’ll need to go out and create your own authentication method. Whenever possible, use a standard that is widely implemented. Otherwise, developers will spend more time than necessary figuring out how to get started. Plus, “creative” authentication can often lead to security issues.

We won’t mention every authentication option in this article, but we’ll cover three common approaches: OAuth, API Keys (and other tokens), and OpenID Connect.

OAuth for Accessing User Data
Gone are the days of users sharing passwords with API developers. This insecure practice has been replaced by an OAuth standard that is widely adopted. You can use OAuth for both authentication and authorization, terms that are easily confused.

A simple hotel analogy can help explain the difference. You give your driver license to the concierge, she reads your name and looks at your smiling face and photo. This is to determine your authenticity. Congratulations! You are now authenticated. The attendant then checks some records, returns you the smile and gives you a key card. In OAuth terms, she defined if you are authorized to stay in a hotel room, and gave you an access token for the resource.

OAuth can be used for authentication, but it was designed for authorization. You can use the keycard to access your room and amenities without confirming who you are again, the same as accessing resources with your OAuth token without copy-pasting keys or retyping passwords. Imagine the concierge writing your name and ID number on your card. Similarly,  OAuth allows you to include your identity information as a claim in your token. You then prove your identity everywhere with the key. 

OAuth makes your life easier and helps protect your passwords by using access tokens instead. But tokens themselves have to be protected.

API Keys and Other Tokens Must Be Secured
Microservices are now everywhere and so are API keys. You can use them with well-known callers when you don’t need granular permissions. Expanding on the hotel example, caretakers often have master keys opening every door. That practice itself is not insecure.

“Hey, what if such a super-key is stolen,” you might argue. Yes, we have a problem here. This is why API keys must be secured. Sniffed OAuth tokens are usually not as big of a risk, because they are often time-bound and can be scoped to specific areas of an API. Still, even if set to expire shortly, it can be used to perform a call or two on your behalf.

Sending keys or tokens unencrypted is like keeping those hotel key cards stacked on the counter. How you send your secrets also might be important. Headers or POST requests over an encrypted channel are proven ways to do it. The querystring, on the other hands, is subject to problems like bookmarking, screenshotting, or logging. OAuth2 access tokens, for instance, are sent inside a header. And always with SSL/TLS.

OpenID Connect Provides Identity Atop OAuth
As we’ve mentioned, OAuth is made for authorization. However. you can also send your identity information as a part of an OAuth token. There are advantages to letting OAuth focus on authorization and separating out the identity flow.

Again, let’s return to our hotel example. Remember the card the concierge gave you? It included your name and driver license number on it. If you lost that card bad things could happen. If your personal information was not on your card, it couldn’t be compromised. The same is true of your token. 

Another standard can help us here. In this case, OpenID Connect. It employs battle-tested OAuth2 for authorization and adds a separate id_token for identity information. This way you avoid leaking user-specific information in access tokens. In addition, OpenID Connect is a standard, so all the implementations have to be compliant. You only need to know that a provider implements it to plug both authorization and authentication into your application.

When it comes to API authentication and authorization, choose standards and the best practices used across the industry. Don’t get creative, or you’ll make it difficult for developers to get started and easier for them to do the wrong thing.
