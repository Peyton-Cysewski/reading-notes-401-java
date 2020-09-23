# Solid Principles

## Single Responsibility Principle
Each method should be responsible for exactly one task. One a large scale this makes everything easier. Code is easier to maintain and tests are easier to write. With tests in mind, it is also a good idea to make tests test for only one use case. All the same reasons apply.

## Open/Close Principle
Any class or method should be considered a closed box once it has been written. If a use case comes up where the behavior needs to be adjusted, instead of changing the base class or method, it should be extended and then this new derived class or method can adjust for the new needed behavior.

## Liskov Substitution Principle
Any object in your application should be able to be replaced with an object that is derived from it without breaking the application.

## Interface Segregation Principle
Clients should not be required to rely interfaces that they do not use. Functionality should not be joined at the hip to some massive interface, instead it should allow for smaller segments within to be used on a per need basis.

## Dependency Inversion Principle
Code should depend on abstractions, not concrete implementations. Moreover, the details of those abstractions need to also depend on the abstractions.



[Table of Contents](../README.md)



### External Links
- [SOLID Principles](https://www.digitalocean.com/community/conceptual_articles/s-o-l-i-d-the-first-five-principles-of-object-oriented-design)
- [SOLID in Real Life](https://dzone.com/articles/the-solid-principles-in-real-life)