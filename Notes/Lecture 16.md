### Distributed Systems: Architecture and Design

#### Introduction to Distributed Systems
- **Definition**: Distributed systems are collections of independent computers that appear to the users as a single coherent system.
- **Execution**: They execute on more than one processor or core, which can be within a single CPU, across multiple CPUs, or even over a network of interconnected computers.
- **Reasons for Distribution**: The primary reasons for using distributed systems are **scalability** and **redundancy**. Scalability allows for handling increased loads by adding more resources, and redundancy ensures there is no single point of failure.

#### Types of Distributed Systems
- **Simple Personal Systems**: Typically have one processor but may contain multi-core CPUs, allowing for some degree of parallel processing.
- **Embedded Systems**: Can have single or multiple processors on a single motherboard.
- **Distributed Systems**: Comprise separate processors that do not share memory space and can operate on different operating systems, connected via a network.

#### Characteristics of Distributed Systems
- **Resource Sharing**: CPUs may share resources such as memory or processing power.
- **Openness**: Systems are open to external requests, making them adaptable to new requirements.
- **Concurrency**: Multiple operations can occur simultaneously.
- **Scalability**: Additional hardware can be integrated to enhance processing power.
- **Fault Tolerance**: The failure of one server does not halt the entire system.
- **Transparency**: Users interact with the system as a single entity without awareness of the underlying complexity.

#### Challenges in Distributed Systems
- **Complexity**: More intricate than single-processor systems.
- **Security**: Open systems are more susceptible to attacks, especially in applications like online banking.
- **Management**: Requires handling scalability and unpredictable network traffic.
- **Unpredictability**: Traffic can fluctuate, necessitating dynamic response strategies.

#### Distributed Systems Architectures
- **Client-Server Architecture**: Distinguishes between client processes (requesting data) and server processes (providing services).
- **Distributed Object Architecture**: Treats entities as both clients and servers, allowing objects to request services from each other across different machines.

#### Middleware
- Sits between clients and servers, facilitating communication and data transmission.
- Examples include Java Remote Methods and object brokers.

#### Multiprocessor Architecture
- Involves multiple processes that may not execute on separate physical processors.
- Managed by an operating system dispatcher that allocates processes to available processors using scheduling algorithms like round-robin.

#### Client-Server Process Mapping
- Processes are mapped onto hardware, where a single server can support multiple server processes, and clients can run multiple client processes simultaneously.
- Traffic routing uses port numbers to direct requests and responses appropriately.

#### Layered Architecture of Networked Applications
- **Presentation Layer**: Handles user interface and output presentation.
- **Application Layer**: Manages business logic and application functionality.
- **Data Management Layer**: Stores and manages data persistently.

#### Thin vs. Fat Client Models
- **Thin Client Model**: Processing and data management occur on the server, with the client handling presentation.
- **Fat Client Model**: The client performs some processing and application tasks in addition to presentation.

#### Three-Tier Architecture
- Consists of three physical layers: the client, the application processing server, and the database server.
- Allows for scalability by adding more servers to each layer as needed.

#### Distributed Object Architecture
- No strict distinction between clients and servers; objects can request services from each other.
- Uses middleware like object request brokers for communication across the network.

#### Summary
- Modern systems often use a hybrid of thin and fat client models, with a three-tier architecture being common for scalability and flexibility.
- Distributed object architecture is suitable for highly scalable applications requiring extensive data processing across many machines. It is dynamic, allowing for the addition of new services and the distribution of complex problems.
