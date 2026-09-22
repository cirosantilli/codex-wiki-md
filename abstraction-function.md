# Abstraction function

↑ **Parent:** [Abstract data type](abstract-data-type.md)

An [abstraction function](abstraction-function.md) maps a valid concrete representation to its abstract value. Write $R_{\mathrm{valid}}=\{r:I(r)\}$ and $\alpha:R_{\mathrm{valid}}\to Q$. Different storage states can denote the same abstract value. Correct implementation requires both preservation of the [representation invariant](representation-invariant.md) and agreement with the specified operation after applying the [abstraction function](abstraction-function.md); preserving a length bound alone would not prove first-in, first-out behavior.

The [representation invariant](representation-invariant.md) answers "is this storage state allowed?" The [abstraction function](abstraction-function.md) answers "which value does it represent?" Thus $I(r)$ is a truth value, whereas $\alpha(r)$ is a value of the [abstract data type](abstract-data-type.md). Treating $\alpha$ as a [partial function](partial-function.md) on all storage states, or as a [function](function-split.md) defined on $R_{\mathrm{valid}}$ only, expresses the same restriction. The [abstraction function](abstraction-function.md) may forget storage details, and need not be executable code: its purpose is to connect an implementation to its [formal specification](formal-specification.md).[Rep Invariant and Abstraction Function: representation space, abstract space, partial AF and boolean RI](6-005-software-construction-spring-2016/reading-13-abstraction-functions-and-rep-invariants.md)

This distinction makes [functional correctness](functional-correctness.md) manageable one operation at a time. The [unreduced rational representation](unreduced-rational-representation.md) below separates valid storage from mathematical meaning; [correct operations through an abstraction function](correct-operations-through-an-abstraction-function.md) then checks whether an implementation performs the promised [addition](addition.md). For an example with hidden mutable storage and failure cases, the [bounded queue with encapsulation](bounded-queue-with-encapsulation.md) supplies a different [abstraction function](abstraction-function.md), reading an occupied prefix of an [array](array-data-structure.md) as a [sequence](sequence.md).

**Table of contents**

- [Unreduced rational representation](unreduced-rational-representation.md)
- [Correct operations through an abstraction function](correct-operations-through-an-abstraction-function.md)

## ↑ Ancestors (4)

1. [Abstract data type](abstract-data-type.md)
2. [Encapsulation (computer programming)](encapsulation-computer-programming.md)
3. [Computer science](computer-science-split.md)
4. [Codex Wiki](split.md)

## ← Incoming links (8)

- [Abstract data type](abstract-data-type.md)
- [Abstraction function](abstraction-function.md)
- [Bounded queue with encapsulation](bounded-queue-with-encapsulation.md)
- [Circular buffer](circular-buffer.md)
- [Circular buffer operation trace](circular-buffer-operation-trace.md)
- [Correct operations through an abstraction function](correct-operations-through-an-abstraction-function.md)
- [Representation independence](representation-independence.md)
- [Unreduced rational representation](unreduced-rational-representation.md)
