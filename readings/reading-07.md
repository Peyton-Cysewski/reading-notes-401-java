# WRRC and Java

## HTTP In Java
HTTP data transfer will be done using the `HttpUrlConnection` or the `HttpClient` package. The first step is to create a `URL` object with the appropriate URL. Next is to form a connection by running `.openConnection()` on the URL object. Then the request type can be added by passing in the type as a string in all caps to `.setRequestMethod()` on the opened connection. Headers can be set using the `setRequestProperty` method and be read using `.getHeaderField()`. Timeouts for connecting and reading data can also be set. There is a lot more that this class can do, but note that it is a very verbose library. Other external libraries can do the same things in a more tidy manner.



[Table of Contents](../README.md)



### External Links
- [HTTP Review](https://dev.to/dangolant/things-i-brushed-up-on-this-week-the-http-request-lifecycle-)
- [Java HTTP](https://www.baeldung.com/java-http-request)