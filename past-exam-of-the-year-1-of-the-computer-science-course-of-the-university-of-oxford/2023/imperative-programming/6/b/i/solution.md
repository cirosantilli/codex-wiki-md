<h1 id="6/b/i/solution">Solution</h1>

↑ **Parent:** [I](../i.md)

**Permitted; returns `"AB"`.** The receiver's [static type](../../../../../../static-type.md) is `A`, which offers `show(A)`. The argument also has [static type](../../../../../../static-type.md) `A`, so that signature is selected. All three variables refer to the same object of [runtime type](../../../../../../runtime-type.md) `C`; the most-derived implementation of `show(A)` is inherited from `B`. Its `super.show(o)` calls `A.show(A)`, producing `"A"`, and it appends `"B"`. `C` overrides `show(B)`, not this selected signature.

## ↑ Ancestors (13)

1. [I](../i.md)
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
