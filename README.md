# Object-Oriented-Analysis-Design-Review-M3

## Business Value of SDLC

Business value is important to both the company and its customers

- A project's success is measured based on its ability to:
  - deliver quality
  - deliver on time
  - deliver within budget
- A project can only be considered successful if it delivers the predetermined business value

## Systems Analysis & Design Method (SADM)

- A recommended collection of:
  - Phases
  - Procedures
  - Rules
  - Techniques
  - Tools
  - Documentation
  - Management
  - Training
- To understand the problem and provide solutions
- Business Analysts / Systems Analysts are responsible for SADM's implementation
  - by collaborating with other members of the team

**Systems analysis**
- Analyzing the stakeholder needs in order to understand their requirements
**System Design**
- Guidelines on how the proposed system will solve problem

### SADM - User stories

A 1 sentence description of a work-related goal of user
- As a &lt;role&gt; I want to &lt;goal&gt; so that &lt;benefit&gt;
- As a shipping clerk, I want to ship an order as accurately as possible

### SADM - Use Cases

An activity that the system performs, usually in response to a request or trigger
- Define functional requirements
- Business analysts & system analysts decompose the system into a set of use cases 
- Name each use case using Verb-Noun
  - Ship items
  - Read message
  - Transfer forms

### SADM - User goal technique

1. Identify all the potential users
2. Classify users by functional roles
  - e.g., shipping, marketing, sales
3. Further classify users by organizational level
  - e.g., operational, management, executive
4. For each type of user, interview them to find specific goals they want
  - current goals and innovative functions to add value
5. Build a list of preliminary use cases
6. Redundant duplicates and resolve inconsistencies
7. Merge different types of user needing same use cases
8. Review use case list with each type of user (and stakeholders)

### SADM - Event decomposition technique

- Allows to capture temporal and state events aside from user events
  - More comprehensive and complete than user goal technique

**Event**
- Something that occurs in a specific temporal-spacial place
- We care about only a small set of event in real world
**External Event**
- Usually initiated by an external agent or actor, not inside the system
  - Customer buys a product
  - User updates profile
  - Sales manager updates production plans
**Temporal Event**
- datetime or counter defined event
  - Monthly billing
  - Cron jobs
  - Weekly summary report
**State Event**
- Internal states the system is at that triggers the event

1. Identify external events that require a response from the system with name & use case (verb-noun)
2. Identify temporal events that require a response from the system with name & use case (verb-noun)
3. Identify state events that the system might respond to with name & use case (verb-noun)
  - Then, define the state change
5. When events and use cases are defined, redundancy with perfect technology assumption

- Help decompose at an elementary business process (EBP)

#### Elementary business process (EBP)

A fundamental business process performed by one person, in one place, in response to a business event
- Make sure functions that support the users work are identified
- Make sure no additional functions (e.g., security, system controls)

#### Perfect technology assumption

Do not include events that involve such system controls as:
- Login
- Logout
- Change password
- Backup
- Restore database

## Use Case Diagrams

**Use Case Diagrams**
- UML model used to graphically show uses cases and their relationships to actors
**UML**
- Unified Modelling Language, the standard for diagrams and terminology
**Actor**
- All types of end users, including malicious users
**Automation boundary**
- A box that separates actors on the outside, system components at inside
- The box represents the system itself

1. Identify all the stakeholders who need to see a use case diagram.
2. Determine what is important for each stakeholder.
3. Organize the use cases for each communication need. Draw the use case diagrams.
4. Carefully name each diagram as it pertains to each stakeholder and user.

## Quizzes

### Event Decomposition Technique

The technique used to identify use cases based on external, temporal, and state events is the _______.
- Event Decomposition Technique

List three types of events and provide descriptions for each.
1. External event - triggered by actor or something outside of the system
2. Temporal event - triggered by change of time.
3. State event - triggered by state change.

"Customer decides to buy a shirt" is an example of what?
- Activity prior to an event

When a customer buys an item of merchandise using his store credit account, a separate event is required to pay the store.
- True

One way to determine whether an occurrence is an event or part of the interaction before or after an event is by asking if any long pauses or intervals occur
- True

The event decomposition technique begins by identifying all of the _______.
- Business events

In using the event decomposition technique, which of the following is NOT a type of event that is considered?
- Event initiated by a user login

The way to determine whether an occurrence is an event or part of the interaction is to ask the following question: _______?
- Is the system at rest

The event decomposition technique begins by identifying use cases.​
- False, identify external events

One benefit of the event decomposition technique is that it helps to identify use cases at the right level of detail
- True

The end product of the event decomposition technique is a list of use cases at the right level of analysis.
- True

-----

### State event

A(n) _______ event occurs when something happens inside the system that triggers the need for processing.
- State

A state event is a political or governmental activity.​
- False

A state event is an event that occurs when something happens outside the system that triggers the need for processing
- False (a state event happens internally)

The end of an event or a user case is when the system is at rest in a consistent state.​
- True

Which of the following is an example of a state event?
- Inventory reorder point is reached

State events are also sometimes called _______ events.
- internal

A(n) _______ event occurs when something happens inside the system that triggers the need for processing.
- state

The end of an event of a user case is when the system is at rest in a consistent state.
- True

A state event is a political or governmental activity.
- False

Another name for a state event is an internal event.
- True

The analyst begin identifying state events by asking about the specific deadlines that the system must accommodate.
- False

Which of the following is an example of a state event?
- inventory reorder point is reached.

-----

### Temporal Event

Which of the following is an example of a temporal event?​
- Month end billing is started

An event that occurs by reaching a point in time is called a _______ event.​
- temporal

Temporal events always occur on a fixed date or at a fixed time.
- False

Something that occurs at a specific time and place and should be remember by the system is called a(n) _______
- Temporal Event

Which of the following is an example of a temporal event?
- month end billing is started

-----

### External Event

When describing an external event, there is no need to worry about the person or thing causing the event.​
- False

The focus on external events is inappropriate when working with end users because discussing events tends to confuse the issues.​
- False

"The type of event that occurs outside of the system is called a(n) _______.
- external event

When describing an external event, were is no need to worry about the person or thing that caused the event.
- False

The focus of external events is inappropriate when working with end users because discussing events tend to confuse users
- False

alse - begins with gathering information
An actor is a person that plays a particular role within a business process.
- False (an actor is a person, group or external system that interacts with the system by supplying or receiving data)

A customer wants to buy a new shirt can be considered an external event
- False

"Customer decides to buy a shirt" is an example of what:
- An external event (activity prior to event)

-----

### Use cases

The system's reaction to an event is called a(n) _______ .​
- use case

Each use case is used by only one actor.​
- False, multiple actors may have common use cases

A one sentence description of a use case is called a(n) _______.
- brief use case description

The system's reaction to an event is called
- Use case

An activity that the system performs in response to a user request is called a(n):
- Use case

A one sentence description of a use case is called a(n) _______.
- brief use case description

Checks and safety procedures that are put in place to protect the integrity of the system are called _______ .
- System controls

-----

### User Story

User story are different than use cases in:
- Amount of detail

Highly Agile development methodologies favor detailed use case documentation over sketchy user story.
- False, agile favors user story

The beginning step in defining use cases is always to obtain a user story.
- False, identify the actors / stakeholders

User story are different than use cases in what way?
- Differ in the amount of detail captured

Acceptance criteria are usually associated with:
- User story

"As a student, I want to register for a class in order to fulfill education requirements" is an example of a(n):
- User story

The standard template for a user story is "As a ______, I want to &lt;goal&gt; so that &lt;reason&gt;"
- Role

The acceptance criteria can be used to generate test data.
- True

The acceptance criteria for a user story can be considered a contract between the developers and users.
- True

-----

## UMLs & Use Case Diagram

A diagram that illustrates actors and their relationships to the functions provided by the system is called a(n):
- use case diagram

In a use case diagram, and actor must always be a person.
- False, actors can also be other systems, time triggers or event triggers

A UML model that is used to show use cases and their relationships to actors is called a(n):
- Use case diagram

The use case that is “included” use case is the one which is connected to :
​- the head of an arrow

Another name for the «includes» relationship is the «uses» relationship.
- True

The UML notation for the «includes» relationship is a(n):
- Dashed arrow

The UML notation for the «extend» relationship is a(n):
- Dashed arrow

In UML notation, the guillemets character « » is used to show what kind of notation?​
- Stereotypes

In UML notation, the guillemets character is used to show what kind of notation?
- Subordinates

-----

## Boundary

The boundary between the automated portion of the system and the users of the system is called the _______.
- Automation boundary

The automation boundary is the same thing as the system boundary
- False, system boundary is inside automation boundary, representing individual systems

-----

## User Goal Technique

One technique to identify use cases is to ask users what they want to achieve with a particular business procedure. This technique is called ______.
- User goal technique

During the interviews in the user goal technique, the analyst should not try to influence the users in discussing work methods.
- False

Before using the user goal technique the analyst must first identify and classify all the types of system users.
- True

-----

### System Components

Checks or safety procedures are put in place to protect the integrity of the system is referred to as _______.
- system controls

The user goal technique normally begins by identifying, listing, and classifying _______ .
- System users

-----

### Real Time systems

Real time systems require the system to react immediately to things that are going on in the environment.
- True

The source of using the concept of events to define functional requirements was first emphasized with _______ systems.
- Real Time

-----

### Perfect technology assumption

The _______ indicates that events should be included during analysis only if the system would be required to respond under ideal conditions.
- Perfect technology assumption

-----

### Elementary Business Process

A(n) _______ is a task that is performed by one person in response to a business event, adds value, and leaves the system in a stable condition.
- Elementary Business Process

The level of analysis to use when identifying user goals is the _______.
- Elementary business process level

During analysis the analyst should be sure to identify system control events such as the user logging in or out.
- False, user logging is in design phase (core process 4)
