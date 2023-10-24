# Class 29

## What database engine is Room wrapped around? Do you think this is a good choice? Why or why not?

Room is wrapped around SQLite, which is a lightweight, embedded relational database engine. It's a good choice for local database persistence in Android apps due to its simplicity, efficiency, and widespread usage. SQLite is a serverless database that operates directly on the device, making it suitable for mobile applications. However, for larger-scale or server-side applications, a more robust database engine might be preferable.

---

## Do Rooms have any similarities to JPA?

Yes, Room has similarities to JPA (Java Persistence API). Both Room and JPA are object-relational mapping frameworks that provide a higher-level abstraction over traditional relational databases. They use annotations to define entities and relationships, and they generate the necessary database operations based on these annotations. Both aim to simplify database access and reduce boilerplate code in the application.

---

## Describe a DAO in your own words

DAO (Data Access Object) is an interface or abstract class in the Room persistence library that defines methods for accessing and manipulating data in a database. These methods include operations like inserting, updating, deleting, and querying data. DAOs act as a bridge between the application code and the underlying database, providing a clean and abstract way to interact with the data. They encapsulate the database operations, promoting separation of concerns and facilitating testability of database access logic.

---

## Things I want to know more about

- Room and Dependency Injection
- Advanced Room Features