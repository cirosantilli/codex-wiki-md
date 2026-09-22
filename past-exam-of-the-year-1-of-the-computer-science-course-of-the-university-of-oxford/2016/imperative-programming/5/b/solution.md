<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

**The output is `YY`, with no newline.** The variable `a` has [static type](../../../../../static-type.md) `A`, although its [runtime type](../../../../../runtime-type.md) is `B`. Both `c.m(a)` and `d.m(a)` therefore select the signature `m(A)` at compile time. The `m(B)` alternative is not applicable to an argument whose [static type](../../../../../static-type.md) is merely `A`.

Both receivers refer to the same `D` object. [Dynamic dispatch](../../../../../dynamic-dispatch.md) then invokes `D`'s override of the already selected `m(A)` signature, printing `Y` twice. The [static type](../../../../../static-type.md) `C` of `c` changes the visible member set, but both signatures are visible through either receiver in this example. [Overload selection followed by dynamic dispatch](../../../../../overload-selection-followed-by-dynamic-dispatch.md) does not select an overload from the argument's [runtime type](../../../../../runtime-type.md).

## ↑ Ancestors (12)

1. [B](../b.md)
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
