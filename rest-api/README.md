# REST API Cheat Sheet

## HTTP Methods

- **GET**: Retrieve data from the server.
- **POST**: Create new data on the server.
- **PUT**: Update existing data on the server.
- **DELETE**: Remove data from the server.
- **PATCH**: Update a part of existing data on the server.
- **HEAD**: Retrieve metadata from the server.
- **OPTIONS**: Get information about the communication options available for the target resource.

## HTTP Status Codes

- **2xx Success**: Indicates that the request was successful.
  - 200 OK: Successful request.
  - 201 Created: Resource successfully created.
  - 204 No Content: Successful request with no response body.

- **3xx Redirection**: Indicates further action is needed to complete the request.
  - 301 Moved Permanently: Resource has been permanently moved.
  - 302 Found: Resource temporarily resides at a different URI.
  - 304 Not Modified: Resource has not been modified since the last request.

- **4xx Client Error**: Indicates a problem with the client's request.
  - 400 Bad Request: Invalid request from the client.
  - 401 Unauthorized: Authentication is required to access the resource.
  - 403 Forbidden: The server refuses to authorize the request.
  - 404 Not Found: The requested resource could not be found.

- **5xx Server Error**: Indicates a problem with the server.
  - 500 Internal Server Error: Server encountered an unexpected condition.
  - 502 Bad Gateway: Server received an invalid response from an upstream server.
  - 503 Service Unavailable: Server is currently unable to handle the request.

## RESTful Principles

- **Uniform Interface**: Use standard HTTP methods and URIs for interacting with resources.
- **Stateless**: Each request from the client must contain all the necessary information to be understood by the server.
- **Client-Server Architecture**: Separation of concerns between the client and the server.
- **Cacheability**: Responses must define whether they are cacheable or not.
- **Layered System**: The architecture should support the use of intermediary servers (proxies, gateways, etc.).
- **Code on Demand (Optional)**: Server can provide executable code to the client.

## RESTful API Design Best Practices

- **Use Nouns for Resource URIs**: Represent resources with nouns instead of verbs.
- **Use Plural Nouns for Collection Resources**: Use plural nouns for resources representing collections.
- **Use HTTP Methods Correctly**: Use HTTP methods as per their intended semantics.
- **Use HTTP Headers for Metadata**: Utilize HTTP headers for providing metadata.
- **Use Query Parameters for Filtering**: Use query parameters to filter collection resources.
- **Version Your APIs**: Include versioning in your API URIs to ensure backward compatibility.
- **Handle Errors Gracefully**: Provide meaningful error messages and appropriate HTTP status codes.
- **Document Your APIs**: Document your APIs comprehensively to help developers understand usage.

## Tools

- **Postman**: A popular API development environment for building, testing, and documenting APIs.
- **Swagger (OpenAPI)**: A framework for API design, documentation, and testing.
- **Insomnia**: Another API testing tool similar to Postman.
- **curl**: Command-line tool for transferring data with URLs.

## Security

- **OAuth 2.0**: Authorization framework that allows third-party services to exchange authentication credentials securely.
- **JWT (JSON Web Tokens)**: Compact, URL-safe means of representing claims to be transferred between two parties.
- **HTTPS**: Secure communication protocol that encrypts data sent between the client and server.

## References

- [HTTP/1.1 Status Code Definitions](https://www.w3.org/Protocols/rfc2616/rfc2616-sec10.html)
- [Roy Fielding's REST Dissertation](https://www.ics.uci.edu/~fielding/pubs/dissertation/rest_arch_style.htm)
- [RESTful API Design Best Practices](https://docs.microsoft.com/en-us/azure/architecture/best-practices/api-design)
