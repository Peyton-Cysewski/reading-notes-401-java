# Related Resources and Integration Testing

## Data Entity Relationships
- 1 to 1: With this type of relationship, use the `@OneToOne` annotation. The association needs to be "owned" by one side of the relationship. The other side then needs to also have an `@JoinColumn` annotation.
- 1 to many: Because one side owns the relationship, `@OneToMany` and `@ManyToOne` need to be used in the appropriate spots. The many to 1 side also needs the `@JoinColumn` annotation.
- many to many: Use the `@ManyToMany` annotation

## Integration Testing
Writing integration tests in Spring is very useful. The is the option to verify that the correct view was returned, the response body was correct, GET requests work with path variables, GET requests work with query parameters, and POST requests work. This allows for fairly widespread testing of the application's functionality. The specifics of each test vary, so it is worth looking at the links below for more detail.

[Table of Contents](../README.md)



### External Links
- [Related data in Spring](https://www.baeldung.com/spring-data-rest-relationships)
- [Baeldung: Spring Integration Testing](https://www.baeldung.com/integration-testing-in-spring)