<h1 id="9/e/solution">Solution</h1>

↑ **Parent:** [E](../e.md)

A collections library can specify a `List<E>` [Java interface](../../../../../../java-interface.md), with different implementations such as `ArrayList<E>` and `LinkedList<E>`. A method accepting `List<E>` can iterate or access elements according to the documented list contract without requiring one particular storage representation. Each implementation may also extend its own appropriate class superclass.

**The benefit is separating a usable contract from its implementation.** A parameter restricted to a concrete `ArrayList<E>` would exclude a [linked list](../../../../../../linked-list.md) implementation and unnecessarily expose the storage choice. Requiring all providers to extend one concrete class would couple them to its implementation and consume [Java](../../../../../../java-programming-language.md)'s single class-inheritance relationship. Interfaces permit multiple implemented contracts, though clients must rely on the stated contract rather than assuming every optional operation is supported or has the same [time complexity](../../../../../../time-complexity.md).

## ↑ Ancestors (11)

1. [E](../e.md)
2. [9](../../9.md)
3. [Paper 5](../../../paper-5-split.md)
4. [Ia](../../../split.md)
5. [2006](../../../../split.md)
6. [Past exam of the mathematics course of the University of Cambridge](../../../../../split.md)
7. [Mathematics course of the University of Cambridge](../../../../../../mathematics-course-of-the-university-of-cambridge.md)
8. [Course of the University of Cambridge](../../../../../../course-of-the-university-of-cambridge.md)
9. [University of Cambridge](../../../../../../university-of-cambridge-split.md)
10. [List of universities](../../../../../../list-of-universities.md)
11. [Codex Wiki](../../../../../../split.md)
