loading...

#### Programming language

- OOP

  OOP is a programming paradigm based on "objects". Objects can bse considered as real-world instances of entities like class, that have some characteristics and behaviors.

  - `Encapsulation`

    Encapsulation is used to bind together both data and methods which manipulate those data, to make sure that certain data can only be used in a proper way and keep them safe from outside. 

    - Data hiding 

      Hiding some informaiton, such as restricting access to any fields or methods of an object.

    - Data binding 

      Binding fields and methods together as a class.

    - Flexsibility and Reusability 

      Can make the variables of a class to be read-only or write-only, by only providing the get methods or the set methods.  Can always reuse part of code or modify with new requirements. 

  - `Inheritence`

    Inheritance not only helps to keep the implementation simpler but also helps to facilitate code reuse. Subclass will inherit the fields and methods from superclass, and not inherit constructors. If the an instance of subclass is created, the constructor of superclass will be called before the constructor of subclass.

    - `Overriding`

      Methods overriding allows subclass provide different implementation of method that already provided by superclass. So the implementation in the subclass will rewrite the method in superclass.

      If an object of a superclass is used to invoke the method, then the method in the superclass will be executed; if an object of the subclass is used to invoke it, then the method in the subclass will be executed. Notice it's the type of the object being instantiated (not the type of the reference variable) that determines which version of the method should be executed.  

  - `Polymorphism`

    Polymorphism is the ability of an object to take on multiple forms. So with polymorphism, same reference, but different implementations. 

    - `static` 

      static polymorphism allows a class to have multiple methods that use the same name, but different signatures (method signature may indicate the number, types or sequences of parameters) with 

      different implementations. The compiler will determine which method to be invoked at the compiling time. 

    - `dynamic`

      In Java, dynamic polymorphism can't be achieved by the compiler. Instead, the JVM will do that at runtime. It occurs mostly in inheritance with method overriding. When you declare a superclass variable and assign it with a subclass object, in this way, the method in the subclass should be invoked, and this is called `upcasting`.

  - Override vs Overload

    - Methods overload is about same method name with different signatures (types, number, order) in same class, Methods override is about same method name with same signatures but in different class connected with inheritence.
    - Override represents dynamic polymorphism, Overload represents static polymorphism.

  - `Interface`

    It is blueprint of class, which enforces some behaviors a class has to do without telling how to do that. In Java, all methods in interface should be public and abstract, and all fields should be public static and final. Interface can not be instantiated. A class can implement more than one interface, and interface can extends multiple interfaces.  

    - `Default` 

      Default allow us to add new methods to an interface that are automatically available in the implementations. But it will cause the code simply won't compile, as there's a conflict caused by multiple interface inheritance. (a.k.a the Diamond Problem).

    - `static` 

      Static allows us to increase the degree of [cohesion](https://en.wikipedia.org/wiki/Cohesion_(computer_science)) of a design by putting together related methods in one single place without having to create an object.

      > ​	https://www.baeldung.com/java-static-default-methods

  - `Abstract`

    - `Abstract method`

      A method that is declared, but contains no implementation. 

    - `Abstract class`

      A class contains one or more abstract methods. Abstract class cannot be instantiate and requires subclasses to provide implementations for its abstract methods. So abstract class provides a way where classes can only be inherited but not instantiated.

  - `Abstract class` vs `Interface`

    -  Interfaces contain only abstract methods (before Java8) and therefore methods are by default abstract without being declared with keyword. Abstract class can have both abstract and non-abstract methods, and so abstract methods must be declared with keyword "abstract". 
    - Variables in interfaces are by default static and final while in abstract classes they can be static or non-static, final or non-final.
    - Abstract class can implement one or multiple interface using keyword "implements", abstract class can extend only one class (either abstract or non-abstract, considering the Object class). An interface can extend multiple interfaces. 
    - Fields and methods in an interface are public by default, while members in an abstract class can also be protected or private. 

  - `Garbage Collection`

    - xxx

      > https://www.geeksforgeeks.org/island-of-isolation-in-java/#:~:text=Basically%2C%20an%20island%20of%20isolation,an%20island%20of%20isolation%20too.

- Java SE

  - Exception
  - Generic
  - CommonClass
    - String 
    - Date API
    - Comparator
    - System
    - Math
    - BigInteger + BigDecimal
  - Thread

#### JavaEE

- JDBC

  JDBC(Java Database Connectivity) is a group of public interfaces provide by Sun. It has two parts. One called `Java Driver API` is for Database factory who want to provide connection service. Another called `Java API` is for developer, which can help developer unite development logic and develop base on interface-oriented.

  - Statement

    - problems
      - Complex
      - SQL Injection
      - can not manipulate blob type data

  - PreparedStatement

    DBserver will cache prepared statement compiled. When same prepared statement invoked again, DBServer will directly execute prepared statement compiled.

  - ORM

    ORM refers to Object Relationship mapping

    - One table represents one class
    - One row represents one object
    - One columnlabel represents one field

  - Transaction

    Either all manipulations complete and commit or all manipulate rollback.

    - features

      - Atomicity 

        Either success or fail

      - Consistence 

        State before execution equals state after execution

      - Isolation 

        - read uncomited -> dirty read -> read commited
        - read commited -> non-repeatable read -> repeatable read
        - repeatable read -> phantom /ˈfan(t)əm/ read -> serialize

      - Durability 

        Once commit, the change are permanent

  - Connection Pool

    Create a "buffer pool" for database connections. Put a certain number of connections in the buffer pool in advance. When you need to establish a database connection, you only need to take one out of the "buffer pool" and put it back after use, which simplify database management and improve efficiency.

- JavaWeb

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

#### MiddleWare

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
      
      - Form data
      - Payload
  
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
