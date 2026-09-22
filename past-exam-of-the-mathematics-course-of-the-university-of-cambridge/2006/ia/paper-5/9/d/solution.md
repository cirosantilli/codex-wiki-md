<h1 id="9/d/solution">Solution</h1>

↑ **Parent:** [D](../d.md)

A growable-array library should store its backing [Java array](../../../../../../java-array.md) and logical size in [private fields in Java](../../../../../../private-field-in-java.md). Public methods such as `add`, `get` and `remove` can enforce bounds and keep the size consistent with the stored elements. The representation can later change without requiring clients to modify direct field accesses.

**The benefit is preserving invariants through encapsulation.** If clients could assign the size or replace the backing [Java array](../../../../../../java-array.md) directly, they could create negative sizes, report elements that do not exist, or modify entries without the library's checks. Accessor methods should not expose a mutable backing object indiscriminately, since a private field alone does not prevent that indirect route. Private fields also do not provide a general security boundary against privileged reflection or native code; the point here is ordinary library access discipline.

## ↑ Ancestors (11)

1. [D](../d.md)
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
