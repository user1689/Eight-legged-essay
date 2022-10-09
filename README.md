loading...

#### Programming language

- OOP

  OOP is a programming paradigm based on "objects". Objects can bse considered as real-world instances of entities like class, that have some characteristics and behaviors.

  - 
  - 

- Java SE

- Java Thread

FrameWork
- Spring
- SpringMVC
- SpringBoot
- SpringSecurity
- SpringCloud
  - Gateway
  - OpenFeign
  - 

#### DB

- MySql

MiddleWare
- Redis
- ElasticSearch 

#### OS

- Turing machine
- Semaphore

#### NetWork

- `Tcp` 

- `Http` 
  
  - `Https`  
    Https secures the connection between server and client ensuring data is encrypted and preventing data from intermediary actions.
  - `Http/2`  
    Http/2 allows for multiplexing (requesting multiple data files at the same time), which significantly imporves both site performance and server efficiency. 
  
- Communication way of server and client  
  Polling is a request way based on AJAX.
  
  - `short polling`  
    Lots of requests that are processed as they come on the server, so it will create a lot of traffic. 
  - `long pollling`  
    long polling is a technique which server will hold connection until data is ready or timeout. After client get response, it will send the next request immediately. So the traffic is smaller, but it will eat up resources fast.
  - `server send event`  
    sse base on Http/1.1 or Htpp/2, it will create a one-way communication channel where events flow from server to client only over an HTTP without polling per connection. 
  - `WebSockt`  
  
- `REST API`

  - `REST`

    REST stands for Representational State Transfer, it is a architectural style based on the Hypertext Transfer Protocol(HTTP) for developing web-based applications. REST outlines the guidelines that web service must follow to be considered RESTful. These guidelines ensure that requests and resources are sent easily and efficiently between client and server using standardized HTTP methods.

  - `REST API`

    API stands for application programming interface, it allows seperate application to interact and share data. REST API, also called RESTful API, is api that follows REST principles. In REST API, all data are treated as resources,  and can be represented by a unique uniform resource identifier(URI).

  - `REST Principles`

    - `client-server decoupling`

      The client and server can only interact in a series of requests and responses. Only client can make requests and only server can send responses. This simple principle allows both parties to operate independently of each other.

    - `uniform interface`

      The server and client must follow same protocol. For REST, this protocol is HTTP. 

    - `stateless`

      The server does not store any information about past request/ responses. Each  request and reponse contains all information needed to complete the interaction. Stateless communication reduces server load, saves memory, and improves performance.

    - `layered system`

      Layers are servers that sit between client and server for identifying spam or improving performace. In REST, layers are modular and can be added and removed without affecting the messages between the client and the API server.

    - `cacheable`

      Server response indicate whether or not the resources is cacheable, so that clients can cache any resources to improve performance.

  - `Makeup Languages `
  
    - `XML` (extensible markup language)
    - `JSON `(JavaScript Object Notation)
  
  - Supported HTTP methods
  
    - `POST` creates a new resource on server
    - `GET` requests a resource from the server
    - `PUT`  updates a resource from the server
    - `DELETE`  delete a resource from the server
    - `HEAD` requests meta-information about a resource. This request is similar to GET, but the response does not include a response body
    - `OPTIONS` retrieves a list of possible methods for a resources
  
  - Difference between `POST` and `PUT`
  
    
  
  - `CRUD`
  
    These are the four basic actions that can be performed on databases through a REST API. Each action corresponds to an HTTP request method:
  
    - `C` -> POST
    - `R` -> GET
    - `U` -> PUT
    - `D` -> DELETE
  
  - `HTTP `request
  
    - `StartLine`
  
      - Request method
      - URI
      - HTTP version
  
    - `HTTP request Header`
  
      It includes request meta-data, such as, the user agent, file formats the client will accept, format of request body, caching preference
  
    - `HTTP request Body`
  
      Contains any data associated with the request
  
  - `HTTP`response
  
    - `HTTP version`
    - `Status line`
    - `HTTP` response Header
    - `HTTP` respnose Body
  
  - `HTTP` response status codes
  
    - `1xx` represents informational responses eg: 102 Processing
    - `2xx` represents successful responses
    - `3xx` represents redirects
    - `4xx` represents client errors
    - `5xx` represents server errors
    - `200`
    - `201`
    - `301`
    - `302`
    - `400`
    - `401`
    - `403`
    - `404`
    - `500`
    - `502`
    - `503`
  
  - `Resource`
  
    In REST, every accessible piece of content on the server is labeled as a resource.
  
  - `URI`
  
    `URI` stands for uniform resource identifier. In REST, a URI is a string that identifies a resource on a web server. Each resource has its own unique URI, allows clients to target that resource and perform actions on it. 
  
    eg: `protocol://service-name/resource-type/resource-id`
  
  - `Caching`
  
    
  
  - `Payload`
  
    Payload refers to the data in the request body of POST methods. It is not same as request paramters. 
  
    Hence, it is not possible to send payload data in GET or DELETE methods.
  
  - `AJAX`
  
    Asynchronous JavaScript, or AJAX, is a set of web development techniques used in web applications. At its core, AJAX allows a web page to make requests to a server and update the page interface without needing to refresh.
  
  - Benefits of REST
  
    - 
  
  - DrawBacks of REST
  
    - While statelessness is a benefit of REST, it can sometimes be a disadvantage too. In other words, the server does not keep records of past interactions.
  
    - REST is less strict with its security 
  
    - How to improve? 
      - Authentication and authorization
        - Simply put, authentication is the process of verifying who someone is, whereas authorization is the process of verifying what specific applications, files, and data a user has access to.
        - 
      - Validation
      - Encryption
      - Rate-limiting
      - No sensitive information in URIs
