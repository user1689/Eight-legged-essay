loading...

Programming language
- Java SE
- Java Thread

FrameWork
- SpringMVC
- SpringBoot
- SpringSecurity

DB
- MySql

MiddleWare
- Redis
- ElasticSearch 

NetWork
- Tcp
- Http
  - Https  
    Https secures the connection between server and client ensuring data is encrypted and preventing data from intermediary actions.
  - Http/2  
    Http/2 allows for multiplexing (requesting multiple data files at the same time), which significantly imporves both site performance and server efficiency. 

- Communication way of server and client
  - short polling  
    short polling a request way based on AJAX, client send request to server and server will response it immediately. So it will cause traffic.
  - long pollling  
    long polling is different from short polling, server will hold connection until data is ready or exception happen. After client get response, it will send the next request immediately. So it will run out the resource of server.
  - server send event  
    sse base on Http/1.1 or Htpp/2, it will create a one-directional channel between client and server, server can continously send data to client through channel.
  - WebSockt  
