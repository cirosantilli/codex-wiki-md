<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The [ML exception type](../../../../../../ml-exception-type.md) `exn` contains exception packets and is an extensible datatype: an `exception` declaration introduces a fresh constructor, optionally with an argument. For example:
```
exception Empty;
exception BadIndex of int;
```
`Empty` has type `exn`, and `BadIndex` has type `int -> exn`. These packets are ordinary values which can be passed, returned or stored. `raise` propagates a packet; the resulting expression can have whatever result type its surrounding context requires, because normal evaluation does not return from the raise.

In [exception handling](../../../../../../exception-handling.md), `expression handle pattern => recovery` evaluates the recovery for a matching exception packet and otherwise propagates the packet outward. The normal expression and recovery must have the same result type. Handlers are dynamically nested, and exceptions raised in the recovery are not handled again by that same handler. A variable pattern catches every packet, whereas a constructor pattern selects a particular exception. Separate fresh exception declarations create distinct identities even if their printed names coincide; exception rebinding instead aliases an existing constructor. **`exn` packages exceptional information; `raise` and `handle` determine its control-flow effect.**

## ↑ Ancestors (11)

1. [B](../b.md)
2. [5](../../5.md)
3. [Paper 5](../../../paper-5-split.md)
4. [Ia](../../../split.md)
5. [2007](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
