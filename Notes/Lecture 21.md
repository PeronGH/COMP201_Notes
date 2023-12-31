### Class Diagrams and Associations

#### Aggregation and Composition
- **Aggregation** is a type of association that indicates a "part-whole" relationship. It is represented by a hollow diamond symbol. For example, a module is part of an honors course, meaning that the honors course class will have an attribute listing its modules.
- **Composition** is a stronger form of aggregation denoted by a filled diamond symbol. It implies ownership, where the composed object cannot exist independently of the composite. For instance, if a tic-tac-toe board is deleted, its squares (the composed objects) are also deleted.

#### Association Types
- The relationship between an employee and a team is an **aggregation** because the employee can exist independently of the team.
- The relationship between a wheel and a car is a **composition** because the wheel is an integral part of the car.
- The relationship between an account and a customer is also a **composition** since an account cannot exist without a customer.

#### Roles in Associations
- Associations can be read in both directions, such as "is taking" or "is taken by." It is sometimes clearer to have separate names for the roles that objects play in the association.
- For example, a student is directed by a director of studies, and this relationship is clear from the context of how students and modules operate.

#### Navigability
- Navigability indicates the direction in which messages are sent between classes. For example, a module knows about the student, but the student may not know all details about the module.

#### Qualified Associations
- Qualified associations provide finer detail, such as identifying squares on a tic-tac-toe board by their row and column, rather than just as a collection of nine squares.

#### Derived Associations
- Derived associations are used to imply relationships that are not explicitly modeled. For example, if a lecturer teaches a module and a student takes a module, it is derived that the lecturer teaches the student.

#### Constraints
- Constraints ensure the correctness of a design. They are formally written in the Object Constraint Language (OCL).
- An **XOR constraint** ensures that an object can only be associated with one of two other objects, not both or neither.

#### Association Classes
- An association class combines the properties of an association and a class. It is used when an attribute belongs to the association itself, such as a grade belonging to the association between a student and a module.

#### Interfaces
- Interfaces specify operations that are visible outside of a class. All elements of an interface are public, and they define operations without implementation, similar to an abstract class.
