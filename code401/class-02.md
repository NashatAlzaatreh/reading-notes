# Express

## Review, Research, and Discussion

1. What’s the difference between PUT and PATCH?

- PUT HTTP Request: PUT is a method of modifying resources where the client sends data that updates the entire resource. PUT is similar to POST in that it can create resources, but it does so when there is a defined URL wherein PUT replaces the entire resource if it exists or creates new if it does not exist.

- PATCH HTTP Request: Unlike PUT Request, PATCH does partial update e.g. Fields that need to be updated by the client, only that field is updated without modifying the other field.

2. Provide links to 3 services or tools that allow you to “mock” an API for development like json-server

- [Nock](https://github.com/nock/nock)
- [MockServer](https://www.mock-server.com/)
- [Postman Mock Server](https://learning.postman.com/docs/designing-and-developing-your-api/mocking-data/setting-up-mock/)

3. Compare and contrast Swagger and APIDoc.js 1 Which HTTP status codes should be sent with each type of (un)successful API call?

| aspect                    | Swagger                                                                                                                                                                           | APIDoc.js                                                                                                                                   |
| ------------------------- | --------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------------------------------------------------------------------------- |
| Popularity                | more popular                                                                                                                                                                      | less popular                                                                                                                                |
| Consistency               | more consistent                                                                                                                                                                   | less consistent                                                                                                                             |
| Implementation complexity | required documentation content on implemented method                                                                                                                              | required documentation content on implemented method                                                                                        |
| Maintenance               | you can limit changes                                                                                                                                                             | have to modify documentation for each affected method/endpoints if service changed, but by implementing apidocjs you can isolate the layer. |
| Other benefits            | Because swagger use plain .json that could be parsed through programing language, thus we can get advantage of various other 3rd parties in order to create http client and more. | XXX                                                                                                                                         |
| Future                    | XXX                                                                                                                                                                               | Due to popularity of swagger, apidocjs provide information about apidoc-swagger converter so we can switch apidoc to swagger anytime.       |

- When a successful API call is made a statues code `200` is sent.
- When an unsuccessful API call is made , many status code can be sent in relation to the cause. like:
  1
  - 308
  - 204
  - 404
  - 403
  - or 500

4. Compare and contrast SOAP and ReST

- **SOAP** is a protocol which was designed before REST and came into the picture. The main idea behind designing SOAP was to ensure that programs built on different platforms and programming languages could exchange data in an easy manner. SOAP stands for Simple Object Access Protocol.
- **REST** was designed specifically for working with components such as media components, files, or even objects on a particular hardware device. Any web service that is defined on the principles of REST can be called a RestFul web service. A Restful service would use the normal HTTP verbs of GET, POST, PUT and DELETE for working with the required components. REST stands for Representational State Transfer.

| SOAP                                                                       | REST                                                                             |
| -------------------------------------------------------------------------- | -------------------------------------------------------------------------------- |
| Simple Object Access Protocol                                              | Representational State Transfer                                                  |
| a protocol                                                                 | an architectural pattern                                                         |
| uses service interfaces to expose its functionality to client applications | uses Uniform Service locators to access to the components on the hardware device |
| needs more bandwidth for its usage                                         | doesn’t need much bandwidth                                                      |
| only works with XML formats                                                | work with plain text, XML, HTML and JSON.                                        |
| cannot make use of REST                                                    | can make use of SOAP                                                             |

### Vocabulary

- Web Server: A web server is a computer that runs websites. It's a computer program that distributes web pages as they are requisitioned.
- Express: A minimal and flexible Node.js web application framework, is used to build backend applications (server side web services) such as APIs
- Routing: The process of selecting a path for traffic in a network or between or across multiple networks.
- WRRC: Web Request Response Cycle

### Preview

1- Which 3 things had you heard about previously and now have better clarity on?

- Node js and express framework
- middleware
- CI/CD
