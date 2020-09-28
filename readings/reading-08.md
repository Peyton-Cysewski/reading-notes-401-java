# Spring

## Getting Started
Spring recommends getting started with their Spring Initializr. It is an online application that generates a file that will hold all the project dependencies that you select. Once you attain the appropriate file for your project you can begin setting things up. The most common application uses a form of MVC. The `@Controller` annotation denotes that the class is a controller (that should also have "controller" as part of its naming convention). The `@Getmapping` annotation means that all GET requests from `/greeting` are sent to that method. The `@RequestParam` annotation binds the input from the query string to the method parameter it references.

## Thymeleaf
In Spring, the data that can be accessed in the view is held in a `Model` object. This data can be added with the `addAttribute()` function, returning a `ModelAndView` object, or by using a method with the `@ModelAttribute` annotation attached to it. To access the data on the view side use `${param.<parameter>}` where parameter is the name of the parameter. Note that parameters may be multivalued and use of bracket notation is required to access the specific values. 




[Table of Contents](../README.md)



### External Links
- [Spring App Basics](https://spring.io/guides/gs/serving-web-content/)
- [Spring MVC and Thymeleaf](https://www.thymeleaf.org/doc/articles/springmvcaccessdata.html)