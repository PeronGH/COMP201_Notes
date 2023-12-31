### Essentials of Class Models

#### Class Naming Conventions
- Use singular nouns for class names, avoiding plurals and verbs.
- For actions, use the noun form (e.g., "Encryptor" instead of "Encryption" or "Encrypting").

#### Understanding Class Models
- Class models are part of the Unified Modeling Language (UML).
- They are static models that define the structure of a system, its elements, and their relationships.
- Unlike dynamic models, class models do not describe system behavior over time.

#### Building Class Models
- Aim to build models quickly and cost-effectively, ensuring they meet all requirements.
- Ensure future maintainability by designing encapsulated modules with low coupling and high cohesion.

#### Class Representation
- Classes should represent permanent entities within the domain.
- Use a data dictionary to maintain consistent naming conventions.

#### Class Identification Techniques
- **Data-Driven Design**: Identify classes based on required knowledge, then assign responsibilities.
- **Responsibility-Driven Design**: Identify classes based on required actions, then assign attributes.

#### Associations in Class Models
- Associations between classes are derived from verbs and express relationships.
- An association exists if an instance of one class needs to know about an instance of another.

#### Multiplicity in Associations
- Multiplicity defines the number of instances in an association.
- Notations:
    - **1**: Exactly one
    - **1..***: One or more
    - **2**: Exactly two
    - **1..10**: A range from one to ten
    - **\***: Zero or more (unspecified number)

#### Attributes and Operations
- Attributes describe the data contained within a class.
- Operations define the actions a class can perform.
- Operation signatures include the function name, parameters, and return type.

#### Dynamic Binding
- Dynamic binding determines the method to execute at runtime, allowing for method overriding in subclasses.

#### Generalization and Inheritance
- Generalization implies that a subclass supports all attributes and operations of its superclass.
- Inheritance is the implementation aspect of this conceptual relationship.

#### CRC Cards
- CRC (Class-Responsibility-Collaboration) cards are a design tool to define high-level responsibilities and collaborations.
- Aim for high cohesion (few responsibilities) and low coupling (few collaborators).

#### UML's Expressiveness
- UML allows for a detailed and expressive design language to describe class relationships and system structure.
