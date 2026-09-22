<h1 id="6/b/iv/solution">Solution</h1>

↑ **Parent:** [Iv](../iv.md)

**Permitted; returns `"BC"`.** Through [static type](../../../../../../static-type.md) `B`, both `show(A)` and `show(B)` accept an argument of type `C`; [method overloading](../../../../../../method-overloading.md) selects the more specific `show(B)`. The receiver's [runtime type](../../../../../../runtime-type.md) is `C`, so [dynamic dispatch](../../../../../../dynamic-dispatch.md) invokes `C.show(B)`. Its `super.show(o)` calls `B.show(B)`, returning `"B"`, and the override appends `"C"`. The `show(C)` overload is not visible through receiver type `B`.

## ↑ Ancestors (13)

1. [Iv](../iv.md)
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
