# design-patterns

Design patterns, as name suggest, are solutions for most commonly (and frequently) occurred problems while designing a software. These patterns are mostly “evolved” rather than “discovered”. A lot of learning, by lots of professional, have been summarized into these design patterns. None of these patterns force you anything in regard to implementation; they are just guidelines to solve a particular problem – in a particular way – in particular contexts. Code implementation is your responsibility.

## Creational Design Patterns ##
Creational patterns often used in place of direct instantiation with constructors. They make the creation process more adaptable and dynamic. In particular, they can provide a great deal of flexibility about which objects are created, how those objects are created, and how they are initialized.

In software engineering, creational design patterns are design patterns that deal with object creation mechanisms, trying to create objects in a manner suitable to the situation. The basic form of object creation could result in design problems or added complexity to the design. Creational design patterns solve this problem by somehow controlling this object creation.

### Abstract Factory ###  
Creates an instance of several families of classes

### Builder ###
Separates object construction from its representation

### Factory Method ###
Creates an instance of several derived classes

### Object Pool ### 
Avoid expensive acquisition and release of resources by recycling objects that are no longer in use

### Prototype ###
A fully initialized instance to be copied or cloned

### Singleton ###
A class of which only a single instance can exist

## Structural patterns ##
In Software Engineering, Structural Design Patterns are Design Patterns that ease the design by identifying a simple way to realize relationships between entities.

### Adapter ###
Match interfaces of different classes

### Bridge ###
Separates an object's interface from its implementation

### Composite ###
A tree structure of simple and composite objects

### Decorator ###
Add responsibilities to objects dynamically

### Facade ###
A single class that represents an entire subsystem

### Flyweight ###
A fine-grained instance used for efficient sharing

### Private Class Data ###
Restricts accessor/mutator access

### Proxy ###
An object representing another object

## Behavioral patterns ##
In software engineering, behavioral design patterns are design patterns that identify common communication patterns between objects and realize these patterns. By doing so, these patterns increase flexibility in carrying out this communication.

A behavioral pattern abstracts an action you want to take from the object or class that takes the action. By changing the object or class, you can change the algorithm used, the objects affected, or the behavior, while still retaining the same basic interface for client classes.

## Chain of responsibility ###
A way of passing a request between a chain of objects

## Command ###
Encapsulate a command request as an object

## Interpreter ###
A way to include language elements in a program

## Iterator ###
Sequentially access the elements of a collection

## Mediator ###
Defines simplified communication between classes

## Memento ###
Capture and restore an object's internal state

## Null Object ###
Designed to act as a default value of an object

## Observer ###
A way of notifying change to a number of classes

## State ###
Alter an object's behavior when its state changes

## Strategy ###
Encapsulates an algorithm inside a class

## Template method ###
Defer the exact steps of an algorithm to a subclass

## Visitor ###
Defines a new operation to a class without change

## Rules of thumb ##
1. Adapter makes things work after they're designed; Bridge makes them work before they are.
2. Bridge is designed up-front to let the abstraction and the implementation vary independently. Adapter is retrofitted to make unrelated classes work together.
3. Adapter provides a different interface to its subject. Proxy provides the same interface. Decorator provides an enhanced interface.
4. Adapter changes an object's interface, Decorator enhances an object's responsibilities. Decorator is thus more transparent to the client. As a consequence, Decorator supports recursive composition, which isn't possible with pure Adapters.
5. Composite and Decorator have similar structure diagrams, reflecting the fact that both rely on recursive composition to organize an open-ended number of objects.
6. Composite can be traversed with Iterator. Visitor can apply an operation over a Composite. Composite could use Chain of responsibility to let components access global properties through their parent. It could also use Decorator to override these properties on parts of the composition. It could use Observer to tie one object structure to another and State to let a component change its behavior as its state changes.
7. Composite can let you compose a Mediator out of smaller pieces through recursive composition.
8. Decorator lets you change the skin of an object. Strategy lets you change the guts.
9. Decorator is designed to let you add responsibilities to objects without subclassing. Composite's focus is not on embellishment but on representation. These intents are distinct but complementary. Consequently, Composite and Decorator are often used in concert.
10. Decorator and Proxy have different purposes but similar structures. Both describe how to provide a level of indirection to another object, and the implementations keep a reference to the object to which they forward requests.
11. Facade defines a new interface, whereas Adapter reuses an old interface. Remember that Adapter makes two existing interfaces work together as opposed to defining an entirely new one.
12. Facade objects are often Singleton because only one Facade object is required.
13. Mediator is similar to Facade in that it abstracts functionality of existing classes. Mediator abstracts/centralizes arbitrary communication between colleague objects, it routinely "adds value", and it is known/referenced by the colleague objects. In contrast, Facade defines a simpler interface to a subsystem, it doesn't add new functionality, and it is not known by the subsystem classes.
14. Abstract Factory can be used as an alternative to Facade to hide platform-specific classes.
15. Whereas Flyweight shows how to make lots of little objects, Facade shows how to make a single object represent an entire subsystem.
16. Flyweight is often combined with Composite to implement shared leaf nodes.
17. Flyweight explains when and how State objects can be shared.
