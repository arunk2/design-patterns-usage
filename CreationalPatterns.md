Design Patterns - Creational Patterns
=====================================

## Factory Method:
If you need to abstract the actual object creation based on data it holds - you might want to go for Factory method. Typically a Factory pattern returns an instance of one of several possible classes depending on the data provided to it (like choosing from predefined set on some condition). Usually all of the classes it returns have a common parent class and common methods, but their implementation are different for different data.

**Example:** You normally use it when a class can’t anticipate kind of objects it must create. Consider the use of multiple database servers like MySQL, Oracle, SQL Server, DB2, etc... If you have DB instance created through a Factory method, you can easily switch between DB engines based on some configuration @ run time per customer needs.

## Abstract Factory:
You might be in situations where you want to Group together a number of factory methods and Provide an interface for the generation of a whole group of related objects. Typically we need different factories to create objects for different frameworks or platforms. This is closely related to another popularly known pattern DI (Dependency Injection) where you need a run-time value to construct a particular dependency.

**Example:** Data access to two different data sources (e.g. a SQL Database and a XML file).

## Builder:
Often we use complex data structures/objects in our system. The objects are so complex that you need to abstract the construction part into a separate class. They are typically classes dedicated to creating object type and can be used to build complex composite objects.

**Example:** Building objects from files based on some structure defined (some thing like unmarshaling a serialized object from file).

## Prototype:
Sometime you might observe creation of objects are highly computational and needs lots of system resources apart from memory and the new objects are slight modification of an existing object. Prototype pattern is ideal for such situations. It Provides a clone method on objects, so that new, similar objects can be cloned instead of newly created. Thus, a pool of ready-made objects could be used without knowing about their details.

**Example:** Java's base class 'Object' provides clone method for this purpose.

## Singleton:
There are any number of places in programming where you need to make sure that there can be one and only one instance of a class. Singleton pattern ensure there is exactly one instance of a class and access to it. 

**Example:** Print spooler, or a Single access to database engine.
