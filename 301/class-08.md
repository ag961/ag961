# APIs

Source:

> https://docs.microsoft.com/en-us/azure/architecture/best-practices/api-design

1. What does REST stand for?
    
    - Representational State Transfer

1. REST APIs are designed around a resource.
      
1. What is an identifer of a resource? Give an example.
    
    - URI, a unique sequence of characters.

    > https://adventure-works.com/orders/1
      
1. What are the most common HTTP verbs?

    - GET, POST, PUT, PATCH, and DELETE

1. What should the URIs be based on?
    
    - on nouns
      
1. Give an example of a good URI.
    
    - https://adventure-works.com/orders
      
1. What does it mean to have a ‘chatty’ web API? Is this a good or a bad thing?
    
    - APIs that expose a large number of small resources. It is a bad thing as it may require a client application to send multiple requests to find all of the data that it requires.
      
1. What status code does a successful GET request return?
    
    - 200 (OK)
      
1. What status code does an unsuccessful GET request return?
    
    - 404 (Not Found)
      
1. What status code does a successful POST request return?
    
    -  201 (Created)
      
1. What status code does a successful DELETE request return?
    
    -  204 (No Content)
      
---------

[**<== BACK**](301-toc.md)