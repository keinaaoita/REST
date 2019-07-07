# Build a RESTful API with Node.js and Express

## What is REST?

### Representational State Transfer

Series of rules in place for the server to understand what it does and how it works.

Constraints
1. Client server constraint.

    + The Client sends a request, then the server handles the request and sends back a response.

2. Stateless Server

    + One server should have all the information necessary to process a request to send back a response. The server should not store ANY information about the request or the server.

3. Caching

    + The server should let the client know how long this data is for, for any information that the client wants that may be requested for multiple times.

## The Uniform Interface

When dealing with interface for a RESTful service, behave in a very specific way that's uniform with one service to the next.

1. Resources

    + Built around things, not actions. (nouns)
    Examples: Books and authors are what RESTful will be dealing with. Only through nouns.

    + HTTP verbs.
    Examples: GET (request data, service will return data), POST (add data), DELETE (remove data), PUT/PATCH. PUT used for replacing objects. PATCH will only update specific parts of an object and is mostly used for changing larges amounts of data.

2. HATEOAS (Hypermedia as the Engine of Application State)

    + In each request, there will be a set of links that can used to navigate through the API. Shows what other actions you can take on a specific resource.

## Tools Used

### ES Lint

Formats code based on strict syntax to maintain order and cleanliness.

Installs eslint as a dependency 

    npm i eslint -D

    npm run lint

To customize certain rules of eslint, include properties based on name and values.

    rules: {
        "linebreak-style": 0
    }

### Nodemon

Any changes made will automatically reflect onto the designated node environment. Settings was configured in package.json.

