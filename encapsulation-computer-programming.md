# Encapsulation (computer programming)

↑ **Parent:** [Computer science](computer-science-split.md)  
ⓦ [Wiki](https://en.wikipedia.org/wiki/Encapsulation_(computer_programming))

[Encapsulation](encapsulation-computer-programming.md) bundles related program state and operations or hides implementation details behind an interface. [Encapsulation in object-oriented programming](encapsulation-in-object-oriented-programming.md) realizes this through objects and their permitted operations; encapsulation also applies to modules outside object-oriented programs.

The useful boundary is a promise: clients request operations through an [API](application-programming-interface.md), and the implementation maintains a [representation invariant](representation-invariant.md). Instead of proving that every client updates several storage fields consistently, prove that the permitted operations preserve the [representation invariant](representation-invariant.md). [Information hiding](information-hiding.md) also leaves room to replace the [data structure](data-structure-split.md) while keeping the client-facing behavior, a property called [representation independence](representation-independence.md).

Bundling state and operations alone does not establish that promise. [Representation exposure](representation-exposure.md) can let clients bypass the [API](application-programming-interface.md). A `private` annotation alone is not a security guarantee: it does not establish correctness of operations, isolation from hostile code or safe handling of shared mutable storage. The examples below concern sequential calls with no concurrent access and no client access to internal storage; they do not claim protection against arbitrary memory modification.

**Table of contents**

- [Information hiding](information-hiding.md)
- [Abstract data type](abstract-data-type.md)
  - [Representation invariant](representation-invariant.md)
  - [Abstraction function](abstraction-function.md)
    - [Unreduced rational representation](unreduced-rational-representation.md)
    - [Correct operations through an abstraction function](correct-operations-through-an-abstraction-function.md)
- [Bounded queue with encapsulation](bounded-queue-with-encapsulation.md)
- [Representation exposure](representation-exposure.md)
- [Representation independence](representation-independence.md)

## ↑ Ancestors (2)

1. [Computer science](computer-science-split.md)
2. [Codex Wiki](split.md)

## ← Incoming links (3)

- [Encapsulation (computer programming)](encapsulation-computer-programming.md)
- [Encapsulation in object-oriented programming](encapsulation-in-object-oriented-programming.md)
- [Information hiding](information-hiding.md)
