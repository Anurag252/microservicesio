# microservicesio
Apigateway:-
can provide consolidated results for each call , in a single round trip
can switch protocols
The API gateway must use either the Client-side Discovery pattern or Server-side Discovery pattern to route requests to available service instances.
The API Gateway may authenticate the user and pass an Access Token containing information about the user to the services
An API Gateway will use a Circuit Breaker to invoke services


API Composition
to implemenet a query use application code
Implement a query by defining an API Composer, which invoking the services that own the data and performs an in-memory join of the results.

![image](https://user-images.githubusercontent.com/4143476/135197680-dd6537c8-14db-4575-a184-d3811e5d0c33.png)

CQRS
How to implement a query that retrieves data from multiple services in a microservice architecture?
Define a view database, which is a read-only replica that is designed to support that query. The application keeps the replica up to data by subscribing to Domain events published by the service that own the data.

![image](https://user-images.githubusercontent.com/4143476/135197944-965c1eec-be3e-4280-898b-9c725fb5e0ae.png)

alternative is API composition
