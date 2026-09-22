<h1 id="5/c/solution">Solution</h1>

↑ **Parent:** [C](../c.md)

An [abstract data type](../../../../../abstract-data-type.md) specifies **a set of abstract values and the operations on them, including their observable behavior, independently of their concrete representation**. Its operation signatures say what can be requested; its laws or preconditions and postconditions say what those requests mean.

For example a [stack](../../../../../stack-data-structure.md) can be specified by an empty value, `push`, `pop`, and `isEmpty`, with `pop(push(x,s))` returning `x` and leaving `s`. A [linked list](../../../../../linked-list.md) and an [array](../../../../../array-data-structure.md) can implement the same [abstract data type](../../../../../abstract-data-type.md) if clients observe the same specified behavior. [Encapsulation](../../../../../encapsulation-computer-programming.md) hides the representation, while a [representation invariant](../../../../../representation-invariant.md) describes which internal states are valid and an [abstraction function](../../../../../abstraction-function.md) explains which abstract value each valid internal state represents. An [abstract class](../../../../../abstract-class.md) is a language mechanism; it is not by itself a full [abstract data type](../../../../../abstract-data-type.md) specification.

## ↑ Ancestors (12)

1. [C](../c.md)
2. [5](../../5.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
