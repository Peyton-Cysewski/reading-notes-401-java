# Spring and Sockets

## Tutorial Summary
- Add Dependencies: This is only necessary to do manually if you are doing the setup manually and not using the Spring Initializr. Here are the dependenies that otherwise should be implemented: `'org.webjars:webjars-locator-core'`, `'org.webjars:sockjs-client:1.0.2'`, `'org.webjars:stomp-websocket:2.3.3'`, `'org.webjars:bootstrap:3.3.7'`, `'org.webjars:jquery:3.1.1-1'`
- Setup Resource Representation Classes: These are described as POJOs, or Plian Old Java Objects. They are very simplistic in their format and exist as classes that only hold potentially a single field. This is used to store data that is sent in the form of JSON. The conversion library that Spring uses to convert JSON to Java is "Jackson JSON".
- Create a Messaging Controller: Inside this controller, the `@MessageMapping` and `@SendTo` annotations let Spring know that this endpoint is used for message sending and where to send the message objects.
- Congfigure STOMP: The STOMP messaging service has a configuration class denoted by `@Configuration`. This allows STOMP to work some of its magic behind the scenes.
- Client JavaScript: Since a page can only be updated using JavaScript, the live feed of messages has to be dealt with using the `SockJS` and `STOMP` JavaScript libraries.


[Table of Contents](../README.md)


### External Links
- [Real time messaging with websockets](https://spring.io/guides/gs/messaging-stomp-websocket/)