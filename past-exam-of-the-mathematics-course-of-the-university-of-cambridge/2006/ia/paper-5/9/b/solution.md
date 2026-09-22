<h1 id="9/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

An immutable library value such as `java.lang.String` can be a [final class in Java](../../../../../../final-class-in-java.md). No class can extend it, so a client receiving a `String` cannot secretly receive a subclass that changes the behavior of its methods. This protects assumptions about value semantics in code using strings as keys or trusted identifiers.

**The benefit is a closed implementation contract.** Without `final`, subclasses might override methods inconsistently or introduce behavior incompatible with the library's intended guarantees. Making a class final does not by itself make its fields immutable; a correct immutable implementation also controls its state. The cost is that clients cannot customize it by inheritance and must instead use composition or a different abstraction.

## ↑ Ancestors (11)

1. [B](../b.md)
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
