# APIs

## Index

[Home](../README.md)  
[API Design Best Practices](#api-design-best-practices)

[API Design Best Practices](https://docs.microsoft.com/en-us/azure/architecture/best-practices/api-design)

1. What does REST stand for?
   -Representational State Transfer
2. REST APIs are designed around a ____.
   - Resources, which are any kind of object, data, or service that can be accessed by the client.
3. What is an identifier of a resource? Give an example.
   - for example domain.com/projects  Projects is the identifier here and it gives implied meaning to what you will find on said page.
4. What are the most common HTTP verbs?
   - GET
   - POST
   - PUT
   - PATCH
   - DELETE
5. What should the URIs be based on?
   - URIs should be based on nouns (the resource) and not verbs (the operations on the resource).
6. Give an example of a good URI.
   - domain.com/collection
7. What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?
   - Avoid "chatty" web APIs that expose a large number of small resources. Such an API may require a client application to send multiple requests to find all of the data that it requires. Instead, you might want to denormalize the data and combine related information into bigger resources that can be retrieved with a single request.
8. What status code does a successful `GET` request return?
   - HTTP status code 200 (OK).
9. What status code does an unsuccessful `GET` request return?
   - 404 (Not Found).
10. What status code does a successful `POST` request return?
    - HTTP status code 201 (Created).
11. What status code does a successful `DELETE` request return?
    - HTTP status code 204 (No Content)

[Back To Top](#index)
