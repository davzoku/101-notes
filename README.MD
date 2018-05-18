# 101 Notes - ABCs of Programming

This article provides a comprehensive list of layman explanations of programming terms. Most of these terms (and its applications) appeared in the coding interviews that I have attended.

Hope it helps anyone having a coding interview or for self-learning. The programming terms are broadly categorized in alphabetical order.

*This is a WIP*

## A

### Agile + Scrum + Kanban

[The Ultimate Agile Dictionary](https://www.smartsheet.com/ultimate-agile-dictionary)

#### Agile

Agile Software Development refers to the project management approach of developing increments of software in *frequent iterations* based on *evolving requirements*.

**Methodology**
- Scrum
- Kanban
- Extreme Programming (XP)
- Crystal
- Dynamic Systems Development Method (DSDM)
- Lean
- Feature-Driven Development (FDD)

 
**Scrum**

Scrum is agile in a specfic shaping; it is an agile process framework.

*How it’s Used*: Scrum methodology designates three specific roles for each Scrum project: the Product Owner, Scrum Master, and Scrum Team. A Scrum project is characterized by product backlog, sprint planning, backlog refinement, daily Scrum meetings, sprint review meeting, and sprint retrospective meeting. 

*Sprint/ Iteration*: about 2 weeks
- Content of the sprint is determined by a *product owner*
- *product owner* is also in charge of the *backlog*; which is an ordered list of user stories 
- Planning phase: the team decides what user stories that can be delivered by the end of the sprint
- Each day, the team meets to track progress, re-plan in 15-mins meetings called *daily scrums*
- Retrospect/ review what can be done/improve on the next sprint

**Kanban**

Kanban is also a specfic shapings of an agile software methodology.

*How it’s Used*: Rather than being assigned tasks, team members pull work from the product backlog. The only constraint in Kanban are limits (WIP limits) placed on the amount of work that exists in the pipeline at any given time. Kanban helps teams reduce cycle time, optimize workflow, and increase productivity, leading to continuous improvement.

Kanban is a *pull system* versus a push system, instead of, “You start left with the Backlog, and push your work items along through the in progress”, it should read, “You start on the right hand side of the board and pull work items through based on the allocated capacity”.

**Roles in Agile**

- *Scrum Master/Team Lead*: Increases team efficiency, motivate his team, spins, argues for changes that will ensure quality and timeliness.
Ensure observance of DoD.

- *Product Owner*: PO need to understand the clear vision of a product from the customer, end user or stakeholders point of view. The product Owner is responsible for managing the *product backlog* and product backlog visibility. He ensures the business value of the product.

- *Stakeholder*: A stakeholder is anyone who is a direct user, indirect user, manager of users, senior manager, operations staff member, the "gold owner" who funds the project, support (help desk) staff member, auditors, your program/portfolio manager, developers working on other systems that integrate or interact with the one under development, or maintenance professionals potentially affected by the development and/or deployment of a software project.

- *Product Manager*

- *Release Train Engineer (RTE)*: aka Train Scrum Master, also the Program Manager. 

#### Scaled Agile Framework (SAFe)

[Youtube Explanation](https://www.youtube.com/watch?v=RXzurBazN-I)

There are 3 levels (Read from bottom-to-top)

1. 	__**Portfolio Level**__
- Dictate all underlying trains by allocating budget and investment themes
- Create backlog of *portfolio level epics* (big user stories) that needs to be addressed by the train's product managers in upcoming PSI
- *Kanban System*: to ensure cohesiveness by limiting the amount of portfolio level initiatives and make sure all trains are focused on finishing the initiatives.

2. 	__**Program Level**__ 
- Scaled-up version of the Team level
- Made up of multiple teams working together (50-125 ppl)
- **Product Shippable Increment (PSI)**: 5 sprints by default, to deliver a bigger working software
- **Agile Release Train (ART)**: It is constant, relatively short like train timing intervals. *Business Features* that didn't make it in this train, can be done on the next one
- **Product Manager**: handles the *program backlog* which provide most of the content for the team backlog
- The teams also capture dependencies between themselves
- System Demo to ensure that the the whole train is sprinting at the same speed, (same speed among the diff teams)
- 4 sprints are planned. The last sprint is the *HIP sprint*
*Hardening*: Final verification that the PSI objectives are met + load testing
*Innovation*: hackation, explore creative ideas
*Planning*: PSI Demo, maintenance & retrospection, Plan the next PSI
- **Architectual Runway**: 


3. __**Team**__ 
- Works like standard scrum (3-9 ppl)
- Cross-functional; Includes developers and testers

#### Other Agile Terms

- **Backlog**:
A backlog is a changing list of product requirements based on the customer’s needs. The backlog is not a to-do list; rather, it is a list of all the desired features for the product. The Agile team uses the backlog to prioritize features and understand which features to implement first. 

*How It’s Used*: The development team pulls work from the backlog to complete during each iteration. The backlog may change throughout the development process as the team learns more about the customer’s requirements.

- **Definition of Done**:
refers to a set of predetermined criteria that a product needs to meet in order to be considered as being done. 

*How it’s Used*: The team agrees upon a list of criteria which must be met before a product increment is considered to be ‘done’—that is, all design, coding, testing, and documentation have been completed, and the code has been fully integrated into the system. If a task does not meet the Definition of Done criteria, it does not count toward team velocity.

### Asynchronous vs Synchronous

### Assessment

** Risk Assessment **

** Vulnerability Assessment **

## B

### Big Data

## C

### Collection (Java)

#### 


## D 

## E 

### Exception

## F

## G

## H 

## I 

### Interface (C++)
- C++ has no built-in concepts of interfaces. 
- To implement it, use abstract classes which only pure virtual functions
- *Interfaces defines a contract of methods you have to implement*, they can't hold states
- Methods declared in interface are *public and abstract*. All fields are *public, static and final*.
- An interface can extend more than one interface
- A class can implement more than 1 interface, and it must implement all methods in interface,
- Interfaces specify what a class must do and not how. It is the blueprint of the class.
- We cannot create an instance of an interface

### [Implements vs Extends](https://stackoverflow.com/questions/10839131/implements-vs-extends-when-to-use-whats-the-difference)
- extends is for extending a class.
- implements is for implementing an interface
- The difference between an interface and a regular class is that in an interface you can not implement any of the declared methods. Only the class that "implements" the interface can implement the methods. The C++ equivalent of an interface would be an abstract class (not EXACTLY the same but pretty much).
- Also java doesn't support multiple inheritance for classes. This is solved by using multiple interfaces.

## J

## K

## L

### [Lambda Calculus](https://www.youtube.com/watch?v=eis11j_iGMs)

- 3 things in Lambda functions; 1. variables (eg. x, y, z) , 2. lambda notation(way of building functions), 3. way of applying function
- see [Church-Turing Thesis](https://en.wikipedia.org/wiki/Church%E2%80%93Turing_thesis)
- Turing machine program can be translated into an equivalent Lambda Calculus program and vice versa. They are formally equivalent.
- present in most languages today
- see Y combinator / Y Operator; encoding recursion

## M

### MVC (Model, View, Controller)

## N

## O

### Object-Oriented Analysis and Design (OOAD)

## P

### Programming Paradigms

Imperative programming – defines computation as statements that change a program state.
Procedural programming, structured programming – specifies the steps a program must take to reach a desired state.
Declarative programming – defines program logic, but not detailed control flow.
Functional programming – treats programs as evaluating mathematical functions and avoids state and mutable data
Object-oriented programming (OOP) – organizes programs as objects: data structures consisting of datafields and methods together with their interactions.
Event-driven programming – program control flow is determined by events, such as sensor inputs or user actions (mouse clicks, key presses) or messages from other programs or threads.
Automata-based programming – a program, or part, is treated as a model of a finite state machine or any other formal automaton.

## R

## S

### Software Requirements Specification (SRS)

## T

### TensorFlow vs PyTorch

- TensorFlow: Developed by Google Brain

- PyTorch: Cousin of lua-based Torch framework used at Facebook

**Tensor**

### Types of Programming Languages

#### Compiled vs Interpreted Languages
Compiled languages use compilers to generate machine code from source code. Low-level programming languages tends to be compiled for **efficiency** rather than **cross-platform support**. Compiled codes tend to be faster than those translated at run time.
Eg. C++, D, Go, Rust

Interpreted languages use interpreter to execute the instruction directly. They provides additional flexibility and include [platform independence, reflection, dynamic typing, dynamic scoping.](https://en.wikipedia.org/wiki/Interpreted_language)
Eg. PHP, Powershell

Some languages use an *intermediate representation*, which combines compiling and interpreting.
Eg. Javascript, Python, Ruby

#### Functional Programming vs OOP

Object-Oriented Programming 

### Types of Testing

#### Black Box vs White Box Testing

#### Unit Testing, Integration Testing, System Testing

### SIT = System Integration Testing


## U

### UML

## V

## W

## X

## Y

## Z