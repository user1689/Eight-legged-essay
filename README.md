loading...

#### Programming language

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

      Layers are servers that sit between client and server for identifying spam or improving performace. 

    - `cacheable`

      Server response indicate whether or not the resources is cacheable, so that clients are cache any resources to improve performance.

  - 
