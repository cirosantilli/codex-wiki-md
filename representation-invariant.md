# Representation invariant

↑ **Parent:** [Abstract data type](abstract-data-type.md)

A [representation invariant](representation-invariant.md) $I(r)$ specifies which concrete storage states $r$ are valid at the [API](application-programming-interface.md) boundary. Construction must establish it, and each completed operation must preserve it. Internal steps may temporarily violate it only while that state is inaccessible to observers; callbacks or concurrent access would require further reasoning.[Reading 13, How to Establish Invariants: creation, preservation and absence of representation exposure](6-005-software-construction-spring-2016/reading-13-abstraction-functions-and-rep-invariants.md)

The short proof pattern is [mathematical induction](mathematical-induction.md) on the number of completed calls: the initial state satisfies $I$; every permitted transition from an $I$-state ends in an $I$-state; hence every state observable through the [API](application-programming-interface.md) satisfies $I$. An unrestricted external write falls outside this argument.

## ↑ Ancestors (4)

1. [Abstract data type](abstract-data-type.md)
2. [Encapsulation (computer programming)](encapsulation-computer-programming.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (10)

- [Abstract data type](abstract-data-type.md)
- [Abstraction function](abstraction-function.md)
- [Bounded queue with encapsulation](bounded-queue-with-encapsulation.md)
- [Circular buffer indices](circular-buffer-indices.md)
- [Correct operations through an abstraction function](correct-operations-through-an-abstraction-function.md)
- [Encapsulation (computer programming)](encapsulation-computer-programming.md)
- [Representation exposure](representation-exposure.md)
- [Representation independence](representation-independence.md)
- [Representation invariant](representation-invariant.md)
- [Unreduced rational representation](unreduced-rational-representation.md)
