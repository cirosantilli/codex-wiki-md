<h1 id="6/b/v/solution">Solution</h1>

↑ **Parent:** [V](../v.md)

**Permitted; returns `"BC"`.** The receiver's [static type](../../../../../../static-type.md) is `C`, but the argument's [static type](../../../../../../static-type.md) is only `B`. Thus `show(C)` is inapplicable; among `show(A)` and `show(B)`, the latter is more specific. Its implementation is `C.show(B)`, whose superclass call returns `"B"` before `"C"` is appended. The argument happens to reference a `C` object, but [method overloading](../../../../../../method-overloading.md) uses its static type.

## ↑ Ancestors (13)

1. [V](../v.md)
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
