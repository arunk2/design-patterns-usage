Design Patterns in OS Kernel
============================
Most of us know about design patterns. But let me give the crux of what a design pattern is before getting into the topic. 
Design Patterns are the set of solution to typical and most commonly occurring problems in designing software program. They are mostly related to object orient design but not restricted to OOD. We can see many of these patterns being used in non-OO paradigms like OS Kernel.

In this post lets try to list some popular design patterns in OS Kernel.

## Singleton Pattern:
All the global variables available in the kernel are singleton equivalent. We even have thread safe access to some of them via 'Reference Count' type global variables.

## Factory Pattern:
Template based abstract data structures like List, Queue, Heap, etc... creation can be done with some kind of factory methods.

## Iterator Pattern:
All the template based abstract data structures like List, Queue, Heap, etc... navigation/access are done through iterator patterns.

## Facade Pattern:
All System calls like open, read, write, etc... simply abstracts the complex file system underlying it.

## Observer Pattern:
The entire Linux monolithic kernel and plug-gable Kernel modules works majorly on this observer/observable pattern. This pattern is popularly known as publisher-subscriber model.
The recent RCU based APIs Implementations is another example of this pattern.
