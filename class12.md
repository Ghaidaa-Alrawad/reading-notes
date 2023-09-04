# Class 12 Reading

## Spring guide: Accessing Data with JPA

1. How are query methods defined when using Spring Data JPA?

The JpaRepository stands out among the Spring Data Repositories covered in the readings due to its extensive array of methods. It not only incorporates all the functions offered by both the PagingAndSortingRepository and CrudRepository interfaces but also introduces its unique set of methods

2. Which dependencies will you need in order to complete the Spring guide?

To complete the Spring guide, you will need the following dependencies:

- Java17 
- Gradle 7.5+ or Maven 3.5+
- Spring Data JPA, H2 Database, Spring Boot Starter Data JPA
 
3. What annotations are used to specify an auto generated identification number for an Entity?
Annotations such as @Identifier and @AutoGenerate are employed for specific field purposes within the entity.

While @Identifier designates a field as significant, @AutoGenerate, in this context, determines the method of ID generation. In this instance, it's configured as GenerationType.AUTO, implying that the database system will handle ID generation automatically

---

## Baeldung: Comparing repositories 

1. Which of the Spring Data Repositories covered in the readings has the most methods available to it?

JpaRepository stands out as the repository with the most extensive array of methods among the Spring Data Repositories covered in the readings.

By extending both PagingAndSortingRepository and CrudRepository, it not only incorporates all the methods provided by these interfaces but also introduces its own set of unique functionalities

2. Name a downstide of a Spring Data Repository.

A downside of using a Spring Data Repository includes:

- Tight Coupling: Spring Data Repositories can lead to tight coupling between your code and the Spring Data library, making your code dependent on specific abstractions and methods provided by Spring Data, such as Page or Pageable.

- Lack of Fine-Grained Control: Extending repository interfaces like CrudRepository exposes a complete set of persistence methods at once, which might not be suitable for situations where you need more fine-grained control over the methods exposed. 

3. How would you define an operation to find a student based on their name in a repo named StudentRepository which extends JpaRepository?

Follow these steps:

1. Create a Method Signature: Define a method signature within the StudentRepository interface. The method name should follow a specific naming convention used by Spring Data JPA for query generation.

2. Use a Keyword: Begin the method name with a keyword that signifies the operation you want to perform. In this case, you want to find a student by their name, so you can start with a keyword like findBy.

3. Specify the Field: After the keyword, specify the entity field based on which you want to perform the search. In this case, you want to search by name, so you would write Name after the keyword, making it findByname.

4. Provide Method Parameters: In the parentheses following the method name, you should specify the method parameter(s). In this case, you want to pass the name of the student to search for, so you would define a parameter of type String named name.

5. Return Type: Define the return type of the method. Since you want to find a single student by name, the return type should be Student.

Putting it all together, the method signature to find a student by name in a StudentRepository extending JpaRepository would look like this:

```
public interface StudentRepos extends JpaRepository<Student, Long> {
    Student findByname(String name);
}
``` 

## Things I want to know more about

- Advanced Querying
- Transaction Management
- Performance Optimization