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
