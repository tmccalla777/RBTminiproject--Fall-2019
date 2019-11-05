# Mini Project 2 Definitions of Terms

#### How Python Uses Indentation to Control Flow
Tabs are used in Python in order to order the execution of code, where this enhances the usability and usefulness of the 
code being written (as well as organization).

A good example of flow control can be explained with the organization of a nested if-then statement within a for-loop, 
where we can see how the order of when the loops are executed is impacted by indentation.
Say we have the following loop...

for x in range(1,5):

&nbsp;&nbsp;&nbsp;if x %% 2 == 0:

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;print("Even Number!")

&nbsp;&nbsp;&nbsp;else:

&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;print("Odd Number!")

Here we can see how the tabs are used to order the execution of the loops, where we would like the nested if-then loop 
to run AFTER the for loop.
#### Don't Repeat Yourself
The _Don't Repeat Yourself_ concept is used in software development to reduce repetition of code in order to ensure that
code is organized and as efficient as possible. Removing duplicate code will make the code easier to read and much easier
to maintain for future use.

*More code = More processing*
#### Design Patterns from Gang of Four
The Design Patterns from the Gang of Four are broken up as show below...

##### Creational Design Patterns
- Abstract Factory: Allows the creation of objects without specifying their type
- Builder: Objects contain methods used to build/configure an object, where an object can be build and returned in
various ways. This allows for the creation of complex objects, easily.
- Prototype: Creates a new object from copying a pre-existing object.
- Singleton: Ensures that only one object is created, eliminating the option of instantiating more than one object.

##### Structural Design Patterns
- Adapter: Allows for two incompatible classes that share a similar purpose to work together transparently (using 
abstraction).
- Bridge: Defines two layers of abstraction, one for the target that can be extended for different types of receivers
and one for the controls which can be extended to different types of controls that will be able to communicate with the
targets.
- Composite: Allows us to attach individual objects and a composition of objects uniformly. Imagine a folder tree
structure starting at the root. This can be the root composite object (folder) where it accepts types of files and types
of folders. File types have no child components attached to them but a folder can have many more files and even more
groupings contained within.
- Facade: Separates the client from the subcomponents, where the main purpose is to simplify interfaces so you don't
have to worry about what is going on under the hood.
- FlyWeight: Used when creating a lot of similar objects, where objects will be created fro a factory that doesn't share
the same definition or configuration.
- Proxy: Provides a class with limited access to another class to increase security controls.

##### Behavioral Design Patterns
- Chain of Responsibility: Sends problem to an object and if that object can't use it, then it sends it to an object
chained to it that might. The object will have additional objects chained to it until it finds the corresponding object
that can solve the problem.
- Command: An object encapsulates everything needed to execute a method in another object.
- Interpreter: The pattern solves a problem by using a context object to interpret an issue and find a class using
reflection to return the answer.
- Iterator: Implements a special language, and one object can transverse the elements of another object.
- Mediator: Handles communication between related objects without having to know anything about each other, where the
mediator will regulate interactions.
- Momento: Provides the ability to restore an object to it's previous state
- Observer: Contains an object referred to as the subject that maintains a list of dependent classes called observers.
The subject object notifies all observers automatically of any state changes by calling their methods.
- State: Allows an object to change it's behavior when its state changes. Each state implements a behavior associated
with it's state of context.
- Strategy: An object controls which of a family of methods is called. Each method is in its own class that extends a
common base class.
- Template: Contains a final method that defines the steps of an algorithm, it allows subclasses to configure the
template by overwriting methods.
- Visitor: Allows you to perform the same action on many objects of different types without much alteration to their
respective classes.

#### Class

#### Object

#### Static

#### Property/Attribute

#### Method

#### Exception

#### Unit Test

#### Constructor

#### Factory
Standard way to create objects and daa structures that are following a pre-defined pattern. If we think about it, we are
using a template in that the factory is producing the same object.
#### Decorator
This allows all of the options/functionalities that an object can have, where we use decorators to assign these options.

We can think about video games for example, where a character can be equipped with different objects and functions
throughout the game, this can be done through the Decorator.
#### Extend Class

#### CSV Files

#### Reading Files