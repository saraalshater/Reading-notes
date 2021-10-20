# [Using WebSocket to build an interactive web application](https://spring.io/guides/gs/messaging-stomp-websocket/)

### What is websocket ? 
The WebSocket API is an advanced technology that makes it possible to open a two-way interactive communication session between the user's browser and a server. With this API, you can send messages to a server and receive event-driven responses without having to poll the server for a reply.




### This guid will build a server that accepts a message that carries a user’s name. In response, the server will push a greeting into a queue to which the client is subscribed.

1. Starting with Spring Initializr 

2. Adding Dependencies

3. Create a Resource Representation Class

4. Create a Message-handling Controller

5. Configure Spring for STOMP messaging

6. Create a Browser Client

7. Make the Application Executable
 - Build an executable JAR

8. Test the service
