<h1 id="6/b/ii/solution">Solution</h1>

↑ **Parent:** [Ii](../ii.md)

**Permitted; returns `"AB"`.** Through a receiver of [static type](../../../../../../static-type.md) `A`, only `show(A)` is visible. The argument's [static type](../../../../../../static-type.md) `C` is a [subtype](../../../../../../subtyping.md) of `A`, so it can be passed to that method. [Dynamic dispatch](../../../../../../dynamic-dispatch.md) selects `B.show(A)` on the receiver object, exactly as in part (i). The argument's more specific type cannot expose overloads absent from the receiver's [static type](../../../../../../static-type.md).

## ↑ Ancestors (13)

1. [Ii](../ii.md)
2. [B](../../b.md)
3. [6](../../../6.md)
4. [Imperative programming](../../../../imperative-programming-split.md)
5. [2023](../../../../split.md)
6. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../../split.md)
7. [Year 1 of the computer science course of the University of Oxford](../../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
8. [Computer science course of the University of Oxford](../../../../../../computer-science-course-of-the-university-of-oxford.md)
9. [Undergraduate course of the University of Oxford](../../../../../../undergraduate-course-of-the-university-of-oxford.md)
10. [Course of the University of Oxford](../../../../../../course-of-the-university-of-oxford.md)
11. [University of Oxford](../../../../../../university-of-oxford-split.md)
12. [List of universities](../../../../../../list-of-universities.md)
13. [Codex Wiki](../../../../../../split.md)
