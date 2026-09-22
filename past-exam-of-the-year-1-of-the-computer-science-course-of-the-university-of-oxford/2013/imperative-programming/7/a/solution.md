<h1 id="7/a/solution">Solution</h1>

↑ **Parent:** [A](../a.md)

An ordinary call such as the unqualified `f` inside `A.g` uses [dynamic dispatch](../../../../../dynamic-dispatch.md) on the receiver. Thus `c.g` enters `A.g`, but its call to `f` reaches `C.f`. In contrast, `B.h` explicitly invokes `super.f`, which continues after `B` and therefore reaches `A.f`. Finally `A.k` dynamically dispatches its call to `h`, reaching `B.h` again. The output is
```
g in A, f in C
h in B, f in A
k in A, h in B, f in A
```
Hence

$$
\boxed{g:\ A\to C,\qquad h:\ B\to A,\qquad k:\ A\to B\to A.}
$$

These arrows describe the method bodies entered in order, not the [class inheritance](../../../../../class-inheritance.md) relation. An inherited method continues to use the dynamic receiver for ordinary calls; it does not acquire the defining [software class](../../../../../class-programming.md) as a new receiver.

## ↑ Ancestors (12)

1. [A](../a.md)
2. [7](../../7.md)
3. [Imperative programming](../../../imperative-programming-split.md)
4. [2013](../../../split.md)
5. [Past exam of the year 1 of the computer science course of the University of Oxford](../../../../split.md)
6. [Year 1 of the computer science course of the University of Oxford](../../../../../year-1-of-the-computer-science-course-of-the-university-of-oxford.md)
7. [Computer science course of the University of Oxford](../../../../../computer-science-course-of-the-university-of-oxford.md)
8. [Undergraduate course of the University of Oxford](../../../../../undergraduate-course-of-the-university-of-oxford.md)
9. [Course of the University of Oxford](../../../../../course-of-the-university-of-oxford.md)
10. [University of Oxford](../../../../../university-of-oxford-split.md)
11. [List of universities](../../../../../list-of-universities.md)
12. [Codex Wiki](../../../../../split.md)
