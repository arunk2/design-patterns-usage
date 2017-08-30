Design Patterns - Structural Patterns
====================================

## Adapter:
It is very normal you have multiple components being developed by different team. We need to these components to collaborate to give results. We typically go by contracts or specification of how we communicate. Different team works in different speed and some might be migrated to newer version and they may discontinue older specifications and come-up with new specification. Hence to make the other system work we need to change it to use the new specification. Adapter pattern is used in such scenarios. It is used to convert the programming interface of one class into that of another. We write a class that has the desired interface and then make it communicate with the class that has a different interface. It is kind of a Wrapper around other class that adjusts interface to suit needs. Contains other object and delegates requests to it.

**Example:** Arrays to List transalation by Arrays.asList(...)

## Proxy:
Sometimes the creation of an object is expensive, you might want to postpone this creation until you need the actual object. Proxy pattern allows you to achieve this.Proxy object usually has the same methods as the object it represents. After the object is loaded in memory, it passes on the method calls from the Proxy to the actual object.

**Example:** RMI Stub

## Facade:
As your programs evolve over time, they grow in complexity and there may be a number of complicated subsystems, each of which has its own complexities. The Facade pattern allows you to simplify this complexity by providing a simplified interface to these subsystems. It provides a simplified interface to a complex set of inter-related classes. It mainly reduces coupling between software components. 

**Example:** Session bean provides access to several entity beans.

## Bridge:
You might come across situations where you might want to replace some kind of implementation with other kind. Especially with the agile way of developing. Bridge pattern should be used for communication between components which might change very frequently. It is designed by always separating a class’s interface from its implementation. Hence, at any point of time we can have different implementation. It separates abstract and concrete inheritance trees and is normally used along with Abstract Factory pattern.

**Example:** Java AWT peer classes

## Flyweight:
Sometimes you need to have a very large number of class instances to represent data. You can greatly reduce the number instances, if you can recognize that the instances are fundamentally the same except for a few parameters. You can separate these variables outside the class instance and refer to a single common instance, the memory usage can be reduced a lot.
Some other times you might use multiple instances of same and immutable data. It is wise to share the same instance rather than creating separate instances.

**Example:** String literal pool in JVMs are implemented as Flyweight

## Composite:
You can use the Composite pattern to build part-whole hierarchies. A composite is nothing but a collection of objects, where the any object may be either a composite, or a primitive object. 

**Example:** Java AWT Components

## Decorator:
Sometimes you might need to modify the behavior of individual objects without having to create a new derived class. You may want to attach additional responsibilities to an object dynamically. It is an alternative to subclassing for extending functionality.

**Example:** Java BufferedReader, IO StreamReader
