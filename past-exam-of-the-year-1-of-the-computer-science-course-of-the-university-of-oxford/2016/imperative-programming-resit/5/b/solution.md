<h1 id="5/b/solution">Solution</h1>

↑ **Parent:** [B](../b.md)

The output is **`YXWX`**, without a newline. Apply [overload selection followed by dynamic dispatch](../../../../../overload-selection-followed-by-dynamic-dispatch.md) separately to each call:

- `c.m(a)` selects the `m(A)` signature because the argument's [static type](../../../../../static-type.md) is `A`. The receiver is a `D` at runtime, so its override prints `Y`.
- `d.m(b)` selects `m(B)`. `D.m(B)` explicitly calls the inherited implementation with `super.m(o)`, giving `X`.
- `e.m(a)` selects `C.m(A)`, giving `W`.
- `e.m(b)` selects `C.m(B)`, giving `X`.

Although `a` actually refers to a `B`, that [runtime type](../../../../../runtime-type.md) does not select another overload. [Dynamic dispatch](../../../../../dynamic-dispatch.md) chooses the implementation of the already selected signature on the receiver.

## ↑ Ancestors (12)

1. [B](../b.md)
2. [5](../../5.md)
3. [Imperative programming (resit)](../../../imperative-programming-resit-split.md)
4. [2016](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
