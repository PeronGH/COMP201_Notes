### Software Design: Coupling and Coherence

#### Introduction to Software Design Principles
- **Coupling** and **coherence** are fundamental concepts in software design.
- **Loose coupling** and **strong coherence** are characteristics of good software.
- **SOLID principles** in object-oriented (OO) development emphasize these concepts, with the "S" standing for **Single Responsibility**.

#### Importance of Design Principles
- Software should not only meet the requirements but also be stable, error-free, modifiable, and reusable.
- **Useful and usable**: Software must fulfill user requirements and provide an accessible interface.
- **Reliability**: Software should function correctly under various conditions and environments.
- **Flexibility**: Software should be easy to modify and maintain, with clear documentation for future changes.
- **Affordability**: Development costs should be reasonable.
- **Availability**: Software must be accessible when needed.

#### Modular Design and Interfaces
- **Interfaces** define how to interact with code modules, specifying method names, parameters, and return types.
- **Abstraction** allows for the separation of interface and implementation.
- **Documentation** is crucial for understanding how to use interfaces, with tools like Javadoc automating the creation of code documentation.

#### Example of an Interface in C++
```cpp
class Vector {
public:
    Vector(float x, float y, float z); // Constructor
    ~Vector(); // Destructor
    float dotProduct(const Vector& other); // Returns scalar value
    Vector crossProduct(const Vector& other); // Returns a new vector

    void setVector(float x, float y, float z); // Sets vector values

private:
    void normalize(); // Normalizes the vector
};
```

#### Principles of Good Design
- **Linguistic Module Unit**: A class or method that encapsulates a single unit of functionality.
- **Fewer Interfaces**: Minimize the number of interconnections between classes to reduce complexity and improve stability.
- **Loose Coupling**: Changes in one module should have minimal impact on others.
- **Reusability**: Design with the intention to reuse code in future projects.
- **Step-wise Refinement**: Start with a high-level view and progressively break down into smaller, manageable problems.

#### Traceability and Information Hiding
- **Traceability Matrix**: A tool to track which classes interact with each other.
- **Information Hiding**: Internal details of a module should be private unless explicitly declared public.

#### Cohesion and Encapsulation
- **Cohesion**: The degree to which a component is a singular logical entity.
- **Encapsulation**: Protecting the internal state and behavior of a module, promoting strong cohesion.

#### Final Thoughts
- Consider the principles of design when creating software to ensure it is robust, maintainable, and adaptable for future needs.
- Reflect on the importance of these principles and how they can be applied to real-world projects. 