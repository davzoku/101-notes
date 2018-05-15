# 101 Notes - ABCs of Programming

This article provides a comprehensive list of layman explanations of programming terms. Most of these terms (and its applications) appeared in the coding interviews that I have attended.

Hope it helps anyone having a coding interview or for self-learning. The programming terms are broadly categorized in alphabetical order.

*This is a WIP*

## A

### Agile + Scrum

### Asynchronous vs Synchronous

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

## P

## R

## S

### Software Requirements Specification (SRS)

## T

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


## U

### UML

## V

## W

## X

## Y

## Z