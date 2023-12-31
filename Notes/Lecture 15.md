### Software Design and Architecture

#### Architectural Design in Software Engineering
Architectural design is a key process in software engineering, focusing on the division of a system into subsystems or components. These components are designed to function independently, providing specific services while maintaining the ability to integrate with other parts of the system. The goal is to create interoperable and reusable components that can be utilized in various systems without significant code changes.

#### Subsystems and Modules
- **Subsystems** are defined as system components that operate independently from others, offering distinct functionalities. For example, a payment handling subsystem can operate on a separate physical unit and scale across multiple systems to handle increasing transaction volumes.
- **Modules** are smaller parts of a subsystem and in object-oriented (OO) programming, they correspond to classes. Modules contribute to a subsystem's functionality but cannot provide complete services independently.

#### Communication Between Subsystems
Modern subsystems often communicate through web services, allowing for loose coupling and scalability. This method facilitates the interaction between different subsystems, such as payment processing and messaging services, each capable of performing its tasks autonomously.

#### Examples of Subsystems
- In Java, subsystems can be organized as packages, like a `payment handler` package containing all related code.
- Pre-existing subsystems like Hibernate offer database abstraction, enabling object loading and saving without extensive SQL knowledge.
- Subsystems for security, logging, financial transactions, marketing, and order processing exemplify services that can be reused across different applications.

#### Client-Server Architecture
The client-server model is prevalent in distributed systems, where the server provides services to the client. This architecture facilitates data distribution across numerous clients and allows for system scaling by adding servers or enhancing network capacity.

#### Control Models in Software Systems
Control models dictate the flow of control between subsystems:
- **Centralized Control**: A core subsystem manages other subsystems.
- **Event-Based Control**: Subsystems react to external events, such as incoming network packets or hardware interrupts.

#### Concurrent Systems and Hardware Events
Systems may run concurrent processes managed by a central system, ensuring safe and autonomous operation even during network failures. Hardware events, like mouse clicks or network card signals, trigger immediate responses through hardware interrupts, ensuring swift data processing.

#### Modular Decomposition
Systems can be decomposed into modules using two main approaches:
- **Object Model**: The system is divided into loosely coupled modules communicating through messaging. Objects consist of a class, attributes, and methods.
- **Data Flow Model**: The system is segmented into processes with incoming and outgoing data flows. This model is less focused on reusability and not the primary approach in this context.

#### Invoice Processing Example
An invoice processing system can include classes for customers, payments, invoices, and receipts, each with specific attributes and linked to one another to facilitate the transaction process.
