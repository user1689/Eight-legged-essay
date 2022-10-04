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
    long polling is a technique which server will hold connection until data is ready or timeout. After client get response, it will send the next request immediately. So the traffic is smaller, but you eat up your resources fast.
  - `server send event`  
    sse base on Http/1.1 or Htpp/2, it will create a one-way communication channel where events flow from server to client only, which means it allows clients to receive a stream of events from a server over an HTTP connection without polling per connection. 
  - `WebSockt`  
