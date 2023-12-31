### System Models in Detail

#### State Charts and Finite State Machines

- State charts are diagrams that show the **states** and **transitions** of a system or a component.
- They can be used to model the **behaviour** and **control** of a system, such as an automatic braking system.
- State charts have the following elements:
    - **States**: represented by rounded rectangles, they show the conditions or situations of the system.
    - **Transitions**: represented by arrows, they show the changes of states triggered by **events** or **conditions**.
    - **Actions**: represented by labels on the transitions, they show the activities or operations that are performed when the transition occurs.
    - **Initial state**: represented by a black dot, it shows the starting point of the system.
    - **Final state**: represented by a black dot inside a circle, it shows the end point of the system.
- The advantage of putting an action after an event in terms of moving into a change of state is that it allows for more **flexibility** and **relevance**. For example, if the system enters the same state from different locations, it can have different actions depending on the event that triggered the transition.
- Finite state machines (FSMs) are similar to state charts, but they have some extra notation. They are also known as **automata**.
- FSMs are often used to model things where the system **recognises** a pattern of incoming data, such as spell checking, grammar analysis, predictive text, etc.
- FSMs are **context-relevant**, meaning that the output or the next state depends on the input and the current state.
- FSMs have the following elements:
    - **States**: same as state charts, but they can also have **accepting states**, which are represented by double circles. They show the states where the system recognises a valid pattern or input.
    - **Transitions**: same as state charts, but they also have **input symbols** on the labels, which show the characters or data that trigger the transition.
    - **Initial state**: same as state charts.
    - **Input alphabet**: a set of symbols that the system can accept as input.
    - **Transition function**: a rule that defines how the system moves from one state to another given an input symbol.
- There are two variants of FSMs: **Mealy machines** and **Moore machines**. They differ in how they produce **output**.
- Mealy machines have **output symbols** on the transitions, which show the characters or data that are produced when the transition occurs. The output depends on the input and the current state.
- Moore machines have **output symbols** on the states, which show the characters or data that are produced when the system enters that state. The output depends only on the current state.
- Mealy machines and Moore machines are **computationally equivalent**, meaning that they can perform the same tasks. However, Mealy machines may need less states to represent the same system, as they are more **adaptive** and **flexible**.

#### Petri Nets

- Petri nets are another type of diagram that can model the **behaviour** and **control** of a system, especially when the system is **non-deterministic**, meaning that the next state or event is not predictable or random.
- Petri nets were originally developed by Carl Adam Petri when he was 12 years old to model chemical reactions, where molecules can react spontaneously without any external trigger.
- Petri nets have the following elements:
    - **Places**: represented by circles, they show the conditions or situations of the system.
    - **Transitions**: represented by bars, they show the changes of states or events that occur in the system.
    - **Tokens**: represented by dots inside the places, they show the resources or data that are available or consumed in the system.
    - **Arcs**: represented by arrows, they show the connections between places and transitions. They also have **capacities**, which show the number of tokens that are required or produced by the transition.
- The **marking** of a Petri net is the assignment of tokens to places, which shows the **state** of the system. It can be represented by a tuple of numbers, where each number corresponds to the number of tokens in each place.
- A transition is **enabled** when there are enough tokens in each place connected to it by an incoming arc, according to the capacity of the arc. For example, if an arc has a capacity of 2, there must be 2 tokens in the place connected to it for the transition to be enabled.
- A transition can **fire** when it is enabled, which means that it consumes the tokens from the places connected to it by incoming arcs, and produces tokens in the places connected to it by outgoing arcs, according to the capacities of the arcs. For example, if an arc has a capacity of 3, the transition will produce 3 tokens in the place connected to it when it fires.
- The firing of a transition changes the marking of the Petri net, which means that it changes the state of the system. The firing of a transition is **non-deterministic**, meaning that it can happen at any time, or not at all, and it does not depend on any external trigger or input.
- Petri nets can be used to model different computational structures, such as:
    - **Sequence**: when one transition must fire before another, creating a sense of order.
    - **Choice**: when one of several transitions can fire, creating a sense of alternative.
    - **Concurrency**: when several transitions can fire at the same time, creating a sense of parallelism.
    - **Synchronization**: when several transitions must fire together, creating a sense of coordination.
    - **Merging**: when one transition can fire after any of several transitions, creating a sense of aggregation.
    - **Priority**: when one transition can prevent another from firing, creating a sense of preference.
    - **Inhibit**: when the presence of a token can prevent a transition from firing, creating a sense of negation. This is represented by a small circle on the arc.
- Petri nets have a proper mathematical notation, which can be used to analyse their properties, such as **reachability**, **liveness**, **boundedness**, etc. We will look at this in more detail in the next lecture.

#### Semantic Data Models

- Semantic data models are diagrams that show the **structure** and **meaning** of data in a system or a domain.
- They can be used to model the **information** and **relationships** of a system, such as a database or a software design.
- Semantic data models have the following elements:
    - **Entities**: represented by rectangles, they show the objects or concepts that are relevant to the system or the domain.
    - **Attributes**: represented by labels or ovals, they show the properties or characteristics of the entities.
    - **Relationships**: represented by diamonds or lines, they show the connections or associations between the entities.
    - **Cardinalities**: represented by numbers or symbols, they show the number or type of entities that can participate in a relationship.
- There are different types of semantic data models, such as:
    - **Entity-relationship models**: used in database design, they show the entities, attributes, and relationships of a database schema, using symbols such as crow's feet, bars, circles, etc. to indicate the cardinalities of the relationships.
    - **Object models**: used in software design, they show the classes, attributes, and operations of a software system, using symbols such as rectangles, ovals, lines, etc. to indicate the inheritance, aggregation, association, etc. of the classes.
- Semantic data models can be accompanied by **data dictionaries**, which are tables that show the definitions, types, and constraints of the entities, attributes, and relationships in the model.