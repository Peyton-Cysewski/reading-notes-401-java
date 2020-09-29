# Spring RESTful Routing & Static Files

## Request Mapping
Spring allows endpoints to be mapped to various different types of request shapes. This is most useful for differentiating between GET and POST request. The `@RequestMapping` attribute will usually hold just the value for the url endpoint as a string and the method as `GET`, `POST` or another type of request. Headers can also be added as a single key-value pair, or with groupings inside of curely braces. Parts of the URL itself can be mapped as well using `@PathVariable` before the parameter that is mapped. The endpoint variable in the url also needs to be wrapped in curley braces. Other extensions for this can be used as well, such as with Regex to filter out different endpoint paths.

## Spring Data JPA
The JPA acts as a relational entity database that is stored in memory and can also be queried. Objects that can be stored need the `@Entity` attribute a protected constructor, and any additional tags to help with database storage, such sa `@Id`. The entities are stored in database objects. However, you only need to make an interface that extends `CrudRepository` and JPA with instantiate it on its own. Internally, the interface can have query methods defined that similarly will be filled in by the application itself. Lastly, the application needs the `@SpringBootApplication` annotation. Inside the main method it is also common to create a logger inside to log transactions and entities.

## Repositories
- `CrudRepository`: Provides all the basic/common CRUD functionality that is expected in a database.
- `PagingAndSortingRepository`: Provides a pageable object that is useful for pagination and also sorting.
- `JpaRepository`: Adds more customizable and therefore more powerful CRUD functionality.



[Table of Contents](../README.md)



### External Links
- [Baeldung: Spring Request Mapping](https://www.baeldung.com/spring-requestmapping)
- [Spring guide: Accessing Data with JPA](https://spring.io/guides/gs/accessing-data-jpa/)
- [Baeldung: Comparing repositories](https://www.baeldung.com/spring-data-repositories)