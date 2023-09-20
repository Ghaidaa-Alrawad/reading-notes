# Class 18 Reading

## Many to many relationships

### Name a few examples of real world ManyToMany relationships.

- Authors and Books: Authors can write multiple books, and a single book can have multiple authors. This is another common ManyToMany relationship.
- Students and Courses: In a university system, students can enroll in multiple courses, and each course can have multiple students. This forms a ManyToMany relationship between students and courses.

### Explain the significance of a join table for ManyToMany relationships.

In a ManyToMany relationship, a join table is significant because it serves as an intermediary table that connects the two entities involved in the relationship. This join table is responsible for managing the associations between records of the two entities. It allows you to store and represent the many-to-many relationship by linking the primary keys of the entities involved.

For example, in the Hibernate tutorial, the join table employee_project connects the Employee and Project entities. It contains foreign key columns employee_id and project_id, which establish the relationships between employees and projects. The presence of this join table enables you to efficiently query and manage the associations between employees and projects without having to modify the primary tables themselves.

### What are the values held within a join table?

- The employee_project join table contains two columns: employee_id and project_id. These columns hold foreign key references to the primary keys of the Employee and Project tables, respectively.
- The values in the employee_id column represent the employees associated with specific projects.
- The values in the project_id column represent the projects associated with specific employees.

---

## Security: a humorous overview

### According to the author of the article, will you ever be truly secure from ALL possible security threats?

No we can never achieve complete security from all possible threats.

The article highlights that security research often delves into complex and unlikely scenarios, while practical security concerns are more common, the author suggests that in the real world, absolute security is hard to attain, and it's important to balance addressing real risks without becoming overly paranoid about improbable ones.

---

## Things I want to know more about

- How to Join tables are vital intermediaries, connecting entities and managing associations.
- Absolute security against all threats is impossible.