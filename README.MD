# 101 Notes - ABCs of Programming

This article provides a comprehensive list of layman explanations of programming terms. Most of these terms (and its applications) appeared in the coding interviews that I have attended.

Hope it helps anyone having a coding interview or for self-learning. The programming terms are broadly categorized in alphabetical order.

*This is a WIP*

## .

### .NET + ASP.NET
.Net framework is a software layer between the OS and .Net compliant software languages like ** C++, C#, F#, or Visual Basic**

It is a **runtime environment** or platform providing services and extensive set of libraries to application and developers.

It allows 1 editor, 1 common set of libraries and 1 runtime environment for .net compliant languages; allows re-usability of resources


ASP.Net is a web app framework developed by microsoft

- subset of .NET framework
- a framework is a collection of classes

**Common Language Infrastructure (CLI)** provides a language-neutral platform for application development and execution, including functions for exception handling, garbage collection, security, and interoperability.

Microsoft's implementation of CLI is Common Language Runtime (CLR).
The **Common Language Runtime (CLR)**, the virtual machine component of Microsoft's .NET framework, manages the execution of .NET programs. A process known as just-in-time compilation converts compiled code into machine instructions which the computer's CPU then executes. The CLR provides additional services including *memory management, type safety, exception handling, garbage collection, security and thread management*. All programs written for the .NET framework, regardless of programming language, are executed by the CLR.

### .NET vs Node.js
___

## A

### Access Modifiers

Access Level:
+ **private**: accessible only in this class


+ **protected**: accessible only in this package and in all subclasses of this class

+ **public**: accessible everywhere this class is available

+ **static**: A method should be made static when it does not access any of the non-static fields of the class, and does not call any non-static methods. If a field is static, there is only one copy for the entire class, rather than one copy for each instance of the class.

+ **final**:  A final method cannot be overridden in a subclass. A final field is like a constant: once it has been given a value, it cannot be assigned to again.

**[Static Methods vs Non-Static Methods](https://stackoverflow.com/questions/3903537/what-is-the-difference-between-a-static-method-and-a-non-static-method)**
A static method belongs to the class itself and a non-static (aka instance) method belongs to each object that is generated from that class. If your method does something that doesn't depend on the individual characteristics of its class, make it static (it will make the program's footprint smaller). Otherwise, it should be non-static.

Example: Static methods are useful if you have only one instance (situation, circumstance) where you're going to use the method, and you don't need multiple copies (objects). For example, if you're writing a method that logs onto one and only one web site, downloads the weather data, and then returns the values, you could write it as static because you can hard code all the necessary data within the method and you're not going to have multiple instances or copies.

Non-static methods are used if you're going to use your method to create multiple copies. For example, if you want to download the weather data from Boston, Miami, and Los Angeles, and if you can do so from within your method without having to individually customize the code for each separate location, you then access the method non-statically

___


### Agile + Scrum + Kanban + SAFe

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

1. 	**_Portfolio Level_**
- Dictate all underlying trains by allocating budget and investment themes
- Create backlog of *portfolio level epics* (big user stories) that needs to be addressed by the train's product managers in upcoming PSI
- *Kanban System*: to ensure cohesiveness by limiting the amount of portfolio level initiatives and make sure all trains are focused on finishing the initiatives.

2. 	**_Program Level_** 
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


3. **_Team Level_**
- Works like standard scrum (3-9 ppl)
- Cross-functional; Includes developers and testers

#### Other Agile Terms

**_Backlog_**:
A backlog is a changing list of product requirements based on the customer’s needs. The backlog is not a to-do list; rather, it is a list of all the desired features for the product. The Agile team uses the backlog to prioritize features and understand which features to implement first. 

*How It’s Used*: The development team pulls work from the backlog to complete during each iteration. The backlog may change throughout the development process as the team learns more about the customer’s requirements.

**_Definition of Done (DoD)_**:
refers to a set of predetermined criteria that a product needs to meet in order to be considered as being done. 

*How it’s Used*: The team agrees upon a list of criteria which must be met before a product increment is considered to be ‘done’—that is, all design, coding, testing, and documentation have been completed, and the code has been fully integrated into the system. If a task does not meet the Definition of Done criteria, it does not count toward team velocity.

___


### Asynchronous vs Synchronous

___


### Assessment

**Risk Assessment**

**Vulnerability Assessment**

___


## B

### Big Data
___


## C

### Collection (Java)

Hashes, also called associative arrays, are dictionary-like data structures which are similar to arrays. Instead of using integers to index an object, however, hashes use any object as its index.
___


#### 


## D 

## E 

### Enum

Enum / enumeration is a data type consisting of a set of named values called element, members enumeral or enumerators.

You should always use enums when *a variable (especially a method parameter) can only take one out of a small set of possible values*. Examples would be things like type constants (contract status: "permanent", "temp", "apprentice"), or flags ("execute now", "defer execution").

___

### Exception
___


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

___

## J


## K

## L

### [Lambda Calculus](https://www.youtube.com/watch?v=eis11j_iGMs)

- 3 things in Lambda functions; 1. variables (eg. x, y, z) , 2. lambda notation(way of building functions), 3. way of applying function

- see [Church-Turing Thesis](https://en.wikipedia.org/wiki/Church%E2%80%93Turing_thesis)

- Turing machine program can be translated into an equivalent Lambda Calculus program and vice versa. They are formally equivalent.

- present in most languages today

- see Y combinator / Y Operator; encoding recursion

___


## M

### MVC (Model, View, Controller)
___


## N

## O

### Object-Oriented Analysis and Design (OOAD)
___


## P

### Programming Paradigms

**Imperative programming** – defines computation as statements that change a program state.

**Procedural programming, structured programming** – specifies the steps a program must take to reach a desired state.

**Declarative programming** – defines program logic, but not detailed control flow.

**Functional programming** – treats programs as evaluating mathematical functions and avoids state and mutable data

**Object-oriented programming (OOP)** – organizes programs as objects: data structures consisting of datafields and methods together with their interactions.

**Event-driven programming** – program control flow is determined by events, such as sensor inputs or user actions (mouse clicks, key presses) or messages from other programs or threads.

**Automata-based programming** – a program, or part, is treated as a model of a finite state machine or any other formal automaton.
___


## R

### RAID (Redundant Array of Independent Disks)

1. Disk Striping (RAID 0)

- divides data into blocks and spread the data blocks across multiple storage devices

2. Mirroring (RAID 1)
- replicate data to 2 or more disks for high performance and high availability

3. Parity (RAID 5)
- for fault tolerance
- Parity computations are used in RAID drive arrays for fault tolerance by calculating the data in two drives and storing the results on a third. The parity is computed by XOR'ing a bit from drive 1 with a bit from drive 2 and storing the result on drive 3

#### RAID 0 - Performance (Disk Striping) *
*RAID 0 mode provides disk striping across all drives in the RAID drive group, but no mirroring or parity*. RAID 0 does not provide data redundancy but does provide the best performance of any RAID levels. RAID 0 breaks up data into smaller segments and stripes the data segments across each drive in the drive group.

#### RAID 1 - Data Protection (Mirroring) *
Set the system to data protection mode (also known as mirrored mode or RAID 1) and the capacity is divided in half. Half of the capacity is used to store your data and half is used for a duplicate copy. If one drive goes down your data is protected because it's duplicated.

#### RAID 2
- bit-level striping with dedicated Hamming-Code parity.
- All disk spindle rotation is synchronized and data is striped such that each sequential bit is on a different drive. Hamming-code parity is calculated across corresponding bits and stored on at least one parity drive.
- NOT commerically available anymore

#### RAID 3
- byte-level striping with dedicated parity
- All disk spindle rotation is synchronized and data is striped such that each sequential byte is on a different drive. Parity is calculated across corresponding bytes and stored on a dedicated parity drive.
- NOT common


#### RAID 4
- block-level striping with dedicated parity

#### RAID 5 - Data Protection and Speed (Striping with Parity)*
- block-level striping with distributed parity

In systems with three or more drives we recommend that you set the system to RAID 5. This gives you the best of both worlds: fast performance by striping data across all drives; data protection by dedicating a quarter of each drive to fault tolerance leaving three quarters of the system capacity available for data storage.


#### RAID 6
- block-level striping with double distributed parity. Double parity provides fault tolerance up to two failed drives. This makes larger RAID groups more practical, especially for high-availability systems

#### RAID 10 (1+0) - High Reliablity and Performance *
RAID 10 or RAID 1+0 delivers very high I/O rates by striping RAID 1 (mirrored) segments. This RAID mode is good for **business critical** database management solutions that require maximum performance and high fault tolerance. A system set to RAID 10 yields half the total capacity of all the drives in the array.

#### JBOD & Spanning
JBOD (Just a Bunch of Disks) is the use of one or more drives not in a RAID configuration but managed as separate logical volumes. 

Spanning is the combination of drives in a linear fashion to create one large logical volume. The advantage of using this mode is that you can add more drive without having to reformat the system.

#### [Which RAID Should You Use With SQL Server?](https://www.datavail.com/blog/which-raid-should-you-use-with-sql-server/)
1. Consider the number of write and read options

**Data striping (RAID 0) is the RAID configuration with the highest performance, but if one disk fails, all the data on the stripe set becomes inaccessible.** A common installation technique for relational database management systems is to configure the database on a RAID 0 drive and then place the transaction log on a mirrored drive (RAID 1). You can get the best disk I/O performance for the database and maintain data recoverability (assuming you perform regular database backups) through a mirrored transaction log.

**For any data that has to be rapidly recoverable, RAID 5 is the better option. This level of RAID gives users full redundancy of all the data on the array. **This is useful if a single disk happens to fail. The disk can be easily replaced, most often, without any system downtime. Although it does not have the same performance as RAID 0 or RAID 1, using RAID 5 does provide users with higher reliability and faster recovery.
___


### [Random Forest](https://medium.com/@Synced/how-random-forest-algorithm-works-in-machine-learning-3c0fe15b6674)

- works as a large collection of decorrelated decision trees
- based on the bagging technique
- **can be used for both classification and regression**
- create a forest of random decision trees, the larger the number of trees, the more accurate the result
-  Overfitting is one critical problem that may make the results worse, but for Random Forest algorithm, if there are enough trees in the forest, the classifier won’t overfit the model.
- can handle missing values
- can be modelled for categorical values

#### Bagging
- To average noisy and unbiased models to create a model with low variance

___



## S

### Software Requirements Specification (SRS)
– A complete description of the *software’s purpose and functionality*

– Details as to how the software will perform in terms of *speed, response time, availability, portability, maintainability, recovery speed and more*

– *Use cases* of how users will use the software
– The definition of how the application with *interact with other hardware and program*

– *Non-functional requirements* (e.g: performance engineering requirements, quality standards, or design constraints)

**Simple SRS Outline**
1. Purpose
2. Scope
3. System Overview
4. References
5. Definitions
6. Use Cases
7. Functional requirements
8. Non-functional requirements


___

### SQL

#### What is Active-Active and Active-Passive cluster?
The main purpose of an active-active cluster is to achieve **load balancing**. Both nodes are actively running the same service simultaneously. Load balancing distributes workloads across all nodes in order to prevent any single node from getting overloaded. Because there are more nodes available to serve, there will also be a **marked improvement in throughput and response times.**

In the case of active-passive cluster, for example, if the first node is already active, the second node must be passive or on standby.

The passive (a.k.a. failover) server serves as a **backup** that's ready to take over as soon as the active (a.k.a. primary) server gets disconnected or is unable to serve. 

___


## T

### TensorFlow vs PyTorch

- TensorFlow: Developed by Google Brain

- PyTorch: Cousin of lua-based Torch framework used at Facebook

**Tensor**

___


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

___


### Types of Testing

#### Black Box vs White Box Testing

#### Unit Testing, Integration Testing, System Testing

### SIT = System Integration Testing

#### Testing Frameworks: Selenium
- Open source testing framework for web applications

- Selenium Webdriver *supports most of all browsers* to run your test cases and *many programming languages like C#, Java, Python, Ruby, .Net, Perl, PHP, etc..* to create and modify your test scripts.

___



## U

### Unified Modelling Language (UML)
- graphical language for visualizing, specifying, constructing, and documenting information about software-intensive systems.

- Common visualization tools: *Microsoft Visio, Lucid Chart, UMLet, PlantUML*

**_Structural UML diagrams_**
describes the static features of the system

+ **Class diagram**
+ Component diagram
+ Composite structure diagram
+ Deployment diagram
+ Object diagram
+ Package diagram
+ Profile diagram

**_Behavioral UML diagrams_**
describes the interaction in the system;
shows dynamic behavior

+ **Activity diagram**
+ Communication diagram
+ Interaction overview diagram
+ **Sequence diagram**
+ State diagram
+ Timing diagram
+ **Use case diagram**

**TLDR: When to Use**
+ Use **class diagram** to describe classes and show relationships between class
+ Use **activity diagram** to show flow of __actions__, esp good at conditional structures, loops, concurrency
+ Use **sequence diagram** to show __interactions__ and sequence of messages flowing from object to another and the time-order
+ use **use case diagram** during analysis phase to identify system functionality

- For more details: See [dazoku/UML-Study](https://github.com/davzoku/UML-study)
___


## V

## W

## X

## Y

## Z