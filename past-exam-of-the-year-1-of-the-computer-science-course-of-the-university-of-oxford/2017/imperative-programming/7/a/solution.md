<h1 id="7/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

The three printed lines are:

```
g in A, f in C
h in B, f in A
k in A, h in B, f in A
```

The inherited `A.g` makes an ordinary virtual call to `f`, selecting `C.f` by [dynamic dispatch](../../../../../dynamic-dispatch.md). `B.h` instead invokes `super.f`, which selects the next implementation after `B`, namely `A.f`. Finally, `A.k` makes an ordinary virtual call to `h`, selecting `B.h` and its already determined result. A `super` call is not redirected back to the most-derived override.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [7](../../7.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2017](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
