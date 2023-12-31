### Object-Oriented Design and Analysis: Hotel Booking System Case Study

#### Introduction to Object-Oriented Design
- Object-oriented design (OOD) involves identifying the necessary **classes**, **attributes**, and **methods** needed to solve a problem.
- The goal is to determine:
  - The classes required for the system.
  - The attributes each class must have to function properly.
  - The methods needed to make the classes work.

#### Identifying Classes and Attributes
- Start by creating a list of class candidates that may be needed for persistence throughout the codebase.
- Use **noun analysis** to identify potential classes and attributes from a given problem description.
- Not all nouns will become classes; some may serve as attributes, and others may not be needed at all.
- Infer additional classes and attributes that are not explicitly mentioned but are necessary for the system's functionality.

#### Case Study: Hotel Booking System
- The hotel booking system requires a database to capture various details.
- Essential classes identified include:
  - `Hotel`: Represents the hotel entity.
  - `Room`: Stores attributes of individual rooms.
  - `Guest`: Contains details about the guests.
  - `Booking`: Manages booking details.
  - `RoomBooking`: Represents a booking of a specific room.
- Additional inferred classes:
  - `RoomDescription`: Describes types of rooms available.
  - `Person`: A superclass for `Guest`, storing personal details.
  - `Address`: Stores address details, linked to `Person`.

#### Object-Oriented Analysis
- For each class, define:
  - Attributes: Data members that store the state of an object.
  - Relationships: Associations between classes (one-to-one, one-to-many, many-to-many).
  - Methods: Functions that define the behavior of the class.
- Include a unique identifier (ID) for each object to maintain persistence in a database.

#### Database and Class Relationships
- Establish relationships between classes to reflect real-world associations.
- Example relationships:
  - A `Hotel` has multiple `Rooms`.
  - A `Room` has one `RoomDescription`.
  - A `Guest` can have multiple `Bookings`.
- Consider transactional attributes such as rates and currency codes for financial calculations.

#### Method Implementation
- Methods should be derived from use cases and associated with the correct class.
- Common methods include:
  - Checking room availability.
  - Creating a booking.
  - Canceling a booking.
- Design methods to update the database accordingly.

#### Design Flexibility
- The design should support multiple implementation approaches without being overly rigid.
- Allow for changes during the implementation phase without necessitating a complete redesign.

#### Class Diagram
- A class diagram provides a high-level overview of the system's structure.
- It visually represents classes, their attributes, methods, and the relationships between them.

#### Summary
- Use noun analysis to create initial class and attribute lists.
- Add extra classes as needed to ensure the system's functionality.
- Carefully consider class relationships and method requirements.
- Aim for a flexible design that accommodates various implementation strategies.
