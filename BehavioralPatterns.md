Design Patterns - Behavioral Patterns
=====================================
Behavioral patterns are mainly concerned with communication between objects.

## Observer/Observable:
When you need a way a number of classes to be notified of a change or occurrence of an event, Observer pattern can be used. This pattern defines a standard interface for notification of object changes by decoupling the observable from the observers. It is important to note that we have One-to-many relationship from observable to observers

**Example:** Multiple views on one set of data

## Iterator:
The Iterator pattern formalizes the way we move through a list of data within a class.

**Example:** Java Iterator on all Collection of objects, C++ Standard Template Library

## Chain of Responsibility:
If you want requests or exceptions to be handled by classes responsible for it, it can be done by passing request between classes until it is recognized. This way of communications is called as Chain of Responsibility pattern. It is the default method for event handling in hierarchical systems. Events get passed on from most specifically affected class to container classes and eventually the root default handler.

**Example:** Displaying GUI help, Properly implemented Exception handling 

## State:
The State pattern provides a memory for a class’s instance variables. It is very much useful, when the action/behavior is state-dependent and the number of states is likely to change.

**Example:** TCP Connection class with states ‘closed’, ‘established’, and ‘listen’

## Command:
In places where you want to separate an action (or request) from its invocation (or trigger), you want to implement it as Command pattern.

**Example:** Menu systems

## Strategy:
In places where you might want to choose some algorithm over other based on runtime value, Strategy pattern can be used. It encapsulates an algorithm used to perform a task, enabling dynamically switching the algorithm.

**Example:** Pluggable caching strategy

## Template:
There are places where you might want know the skeletal flow of system or a high level algorithm, but the actual implementation has to be decided based on run-time data. Template pattern provides an abstract definition of an algorithm and can be used in such scenarios.

**Example:** InputStream defines read(buf) and read(buf,off, len) in terms of the template method read().


There are other patterns like **Visitor, Interpreter, Mediator** which are less popular in general software application design.
