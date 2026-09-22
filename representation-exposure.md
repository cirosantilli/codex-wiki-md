# Representation exposure

↑ **Parent:** [Encapsulation (computer programming)](encapsulation-computer-programming.md)

[Representation exposure](representation-exposure.md) gives outside code access that can modify storage on which the [representation invariant](representation-invariant.md) or promised behavior depends. Returning the internal [array](array-data-structure.md) exposes a route around the [API](application-programming-interface.md); merely hiding the field name does not close it. Incoming shared mutable storage can create the same problem. Copies or immutable values can prevent such modification, but their costs and sharing rules belong in the design.[Reading 13, Invariants, Immutability: mutable aliases through both returned values and constructor arguments](6-005-software-construction-spring-2016/reading-13-abstraction-functions-and-rep-invariants.md)

The [bounded queue with encapsulation](bounded-queue-with-encapsulation.md) deliberately stores immutable labels. A [FIFO queue](fifo-queue.md) of mutable objects needs a separate promise about whether changing a returned object changes stored content; protecting the queue's ordering and size does not automatically make every stored object immutable.

## ↑ Ancestors (3)

1. [Encapsulation (computer programming)](encapsulation-computer-programming.md)
2. [Computer science](computer-science-split.md)
3. [Codex Wiki](split.md)

## ← Incoming links (2)

- [Encapsulation (computer programming)](encapsulation-computer-programming.md)
- [Representation exposure](representation-exposure.md)
