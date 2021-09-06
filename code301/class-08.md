# APIs

## API Design Best Practices

### - What does REST stand for?

#### Roy Fielding proposed Representational State Transfer (REST) as an architectural approach to designing web services. REST is an architectural style for building distributed systems based on hypermedia. REST is independent of any underlying protocol and is not necessarily tied to HTTP.

### - REST APIs are designed around a ?

#### A RESTful API is an architectural style for an application program interface that uses HTTP requests to access.

### - What is an identifer of a resource? Give an example.

#### The target of an HTTP request is called a “resource”, whose nature isn’t defined further; it can be a document, a photo, or anything else. Each resource is identified by a Uniform Resource Identifier (URI) used throughout HTTP for identifying resources.

### - What are the most common HTTP verbs?

#### REST APIs use a uniform interface, which helps to decouple the client and service implementations. For REST APIs built on HTTP, the uniform interface includes using standard HTTP verbs to perform operations on resources. The most common operations are GET, POST, PUT, PATCH, and DELETE.

### - What should the URIs be based on?

#### nouns (the resource) and not verbs (the operations on the resource).

### - Give an example of a good URI.

#### URIs should follow a predictable, hierarchical structure to enhance understandability and, therefore, usability: predictable in the sense that they’re consistent, hierarchical in the sense that data has structure—relationships. RESTful APIs are written for consumers

### - What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?

#### Chatty API is one that requires consumer to make tremendous - subjective matter - amount of distinct API calls to get needed information about a resource. George Reese has defined chatty API as any API that requires consumer to do more than a single call to perform a single, common operation.

### - What status code does a successful GET request return?

#### 200 or 201- the server successfully returned the page

### - What status code does an unsuccessful GET request return?

#### If not valid, 400 Bad Request is returned. Order is processed. If the order is successful, a 201 Created is returned for the order. If an unexpected error is encountered, a 500 Server Error is returned.

### - What status code does a successful POST request return?

#### If a POST method creates a new resource, it returns HTTP status code 201 (Created).

### - What status code does a successful DELETE request return?

#### It's be HTTP response code 200 (OK) if the response includes an entity describing the status, 202 (Accepted) if the action has been queued, or 204 (No Content) if the action has been performed but the response does not include an entity.
