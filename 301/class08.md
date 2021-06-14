# API Design Best Practices

1. What does REST stand for?

 Representational State Transfer (REST)

2. REST APIs are designed around a ____.

REST APIs are designed around resources, which are any kind of object, data, or service that can be accessed by the client.

3. What is an identifer of a resource? Give an example.

A resource has an identifier, which is a URI that uniquely identifies that resource. For example, the URI for a particular customer order might be:

https://adventure-works.com/orders/1

4. What are the most common HTTP verbs?

GET, POST, PUT, PATCH, and DELETE.

5. What should the URIs be based on?

resource URIs should be based on nouns (the resource) and not verbs (the operations on the resource).

6. Give an example of a good URI.

https://adventure-works.com/orders

7. What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?

APIs that expose a large number of small resources. and it's a bad thing because it's impose a load on the web server.

8. What status code does a successful GET request return?

returns HTTP status code 200 (OK).

9. What status code does an unsuccessful GET request return?

return 404 (Not Found).

10. What status code does a successful POST request return?

HTTP status code 201 (Created).

11. What status code does a successful DELETE request return?

the web server should respond with HTTP status code 204, indicating that the process has been successfully handled.

