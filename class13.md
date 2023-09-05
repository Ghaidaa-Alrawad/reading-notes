# Class 13 Reading

## Related data in Spring (only read section “3. One-to-Many Relationship”)

### Name a few real life examples of “One To Many” relatioships.

- Customer and Orders: A customer can place multiple orders, but each order is associated with only one customer.
- Teacher and Students: A teacher can have many students in a class, but each student belongs to a single teacher.
- Author and Books: An author can write many books, but each book is authored by one author.

### Given two entities, one named Player and one named Team, if you wanted to create a one to many relationship with those entities which would be the one and which would be the many?

- The "Team" entity would be the "one" side of the one-to-many relationship because a team can have multiple players.
- The "Player" entity would be the "many" side of the relationship because each player belongs to one team.

### Explain one to many relationships to a non-technical friend.

Imagine you have a library, and you want to organize books. In a "one to many" relationship, think of it as a librarian (the "one") managing many books (the "many"). Each librarian takes care of a collection of books. So, you have Librarian A responsible for Fiction books, Librarian B for Non-fiction books, and so on. Each librarian (the "one") is connected to multiple books (the "many") in their respective sections. This way, each librarian handles a specific category of books, and the books are organized efficiently.

---

## Baeldung: Spring Integration Testing

### Describe the difference between a unit test and an integration test.

- Unit Test: A unit test focuses on testing a small, isolated piece of code, typically a single function, method, or class. It doesn't involve external dependencies or interactions with other components of the system. Unit tests are designed to ensure that individual units of code work correctly in isolation. Mocks and stubs are often used to isolate the unit being tested from its dependencies.
- Integration Test: An integration test, on the other hand, focuses on testing the interactions and integration points between different components or modules of a system. It tests whether these components work correctly when connected together. Integration tests can involve multiple units, external dependencies, databases, or network interactions. They verify that the system's various parts work together as expected.

### What is the object that provides support for Sprin MVC Testing?

The object that provides support for Spring MVC Testing is `MockMvc`. `MockMvc` is a part of the Spring Test framework and allows you to perform requests and interact with your application's controllers as if you were making real HTTP requests. It provides a way to simulate HTTP requests and responses, making it useful for testing Spring MVC controllers and their behavior without the need to deploy your application to a real server.

### What does the “perform()” method do in a Spring integration test?

In a Spring integration test using `MockMvc`, the `perform()` method is used to send an HTTP request to a specific endpoint of your application and simulate the interaction with that endpoint. It allows you to perform various actions like making GET, POST, PUT, DELETE requests, and more. The `perform()` method returns a `ResultActions` object, which can be used to set expectations on the response received from the server, such as verifying the HTTP status code, response content, headers, and more. It is a key method for executing the actual test and asserting the behavior of your Spring MVC controllers.

---

## Things I want to know more about

- How Spring Data REST handles cascading operations and more complex relationships between entities, such as bidirectional relationships and advanced customizations.
- Exploring more advanced testing scenarios and techniques for Spring MVC applications, such as testing exception handling, authentication, and complex request/response scenarios.